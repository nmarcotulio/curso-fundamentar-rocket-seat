# Aula 7/8 - A Cascata / Especificidade

## A Cascata (cascading)

A escolha do browser de qual regra aplicar, caso haja muitas regras para o mesmo elemento

* Seu estilo é lido de cima para baixo, porém é considerado a base mais forte nas aplicações

É levado em consideração 3 fatores

1. Origem do Estilo
2. Especificidade
3. Importância

### Origem do Estilo
inline -> tag style -> tag link
(mais forte) ao (mais fraco)

### Especificidade
É um cálculo matemático, onde, cada tipo de seletor e origem do estilo, possuem valores a serem considerados.
Muda a ideia da cascata, agora o que importa é o valor.
Se tem o mesmo valor, então novamente será a cascata

0. Universal selector, combinators e negation pseudo class (:not())
1. Element type selector e pseudo-elements (::before, ::after)
10. Classes e attribute selectors ([type:"radio"])
100. ID selector
1000. Inline

### A regra !important
* cuidado, evite o uso
* não é considerado uma boa prática
* quebra o fluxo natural da cascata

