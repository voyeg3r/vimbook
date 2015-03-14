# Introdução #

Definir um estilo de escrita é fundamental para que o trabalho, especialmente os colaborativos, fique coeso. Este documento visa definir as _regras de estilo_ e também, para os casos mais relaxados, as _recomendações_ de escrita.


# Regras de estilo #

## Regras básicas ##

  * Escrever na forma **impessoal**. Isto é, em vez de "_você deve_ ..." (2ª pessoa) ou "_nós devemos_ ..." (3ª pessoa), escrever "**deve-se** ...".
  * Evitar _estrangeirismo_ sempre quando não ficar forçoso.
  * Palavras estrangeiras devem ser escritas em _itálico_. Use `\textit{expressão}` no LaTeX.

## Escrita de combinação de teclas ##

> Usar `Modificador-tecla`. Por exemplo:
    * `Ctrl-a`: modificador **Ctrl** junto com a tecla **a**
    * `Shift-u`: modificador **Shift** junto com a tecla **u** (no entanto, prefira usar apenas a letra maiúscula **U**, a não ser que se queira destacar o uso do `Shift`)
    * `Ctrl-Alt-c`: modificadores **Ctrl** e **Alt** juntos com a tecla **c**
    * `Ctrl-a-b`: modificador **Ctrl** junto com as teclas **a** e **b**

> Letra _minúscula_ é diferente de letra _maiúscula_. Assim, a tecla **J**, por exemplo, tem o mesmo significado que `Shift-j`, mas prefira a primeira versão.

## Formatação do ambiente _verbatim_ ##

> Os conteúdos dentro do ambiente _verbatim_ (`\begin{verbatim} ... \end{verbatim}`) devem ter um deslocamento de **5 espaços** em relação ao começo da linha. Há uma exceção, porém: quando o conteúdo em questão for um trecho de um texto sendo usado para demonstrar algum comando do Vim; neste caso não se usa espaçamento, pois estes podem comprometer a correta funcionalidade do comando (p.e. os comandos `^` e `0`, do modo normal, têm significado distintos dependendo da presença ou ausência de espaços no início da linha).

> Quando o conteúdo da descrição de um elemento no verbatim transpor a margem direita, deve-se continua a descrição na linha abaixo, utilizando o mesmo alinhamento da descrição. Uma dica, dentro do verbatim, a última coluna preenchida deve ser menor ou igual a 66.

## Notas para o LaTeX ##

> Não se utiliza \\ ou \newline quando se utiliza dois parágrafos separados por uma linha em branco. Isso é um "erro" em LaTeX (usa-se uma coisa ou outra).
> Preferencialmente, utiliza-se uma linha em branco para separar dois parágrafos.

> O LaTeX não vai dar dois ENTERs. A forma de "fazer isso" é  utilizando \\`[10mm]` para especificar um tamanho maior para o espaçamento entre duas linhas, mas aí fica assim

Parágrafo 1 \\`[10mm]`
Parágrafo 2, logo abaixo do 1 dentro do código, mas 10 mm abaixo, no pdf gerado. O tamanho é sua escolha.

O uso de \\`[10mm]` ou qualquer outro tamanho que seja deve ser justificado pela necessidade de melhoria visual.

> Não é recomendado ter espaços em branco, acentos ou pontuações e labels do código LaTeX.

> É recomendo diferenciar os labels por tipo, utilizando caracteres diferenciadores, por convenção, ch:label, sec:label, subsec:label, fig:label, eq:label, tb:label, para respectivamente capítulos, seções, subseções, figuras, equações e tabelas, onde 'label' representa o label específico de cada capítulo, seção, etc.

> Exemplo: \section{Para que serve essa seção ?}
> > \label{sec:paraqueserveessasecao}


> Abreviações ou palavras chaves que sejam de fácil correlação também podem ser utilizadas, ou uso ou não de caracteres maiúsculos também é opcional.

> O mais importante é não usar espaços, caracteres especiais, acentos, etc, para não prejudicar programas que ajudam no autocompletar de expressões e/ou para não prejudicar quem escreve o código em UTF-8 em ambientes cujo o locale NÃO seja UTF-8.

# Recomendações #

  * Seguir as novas regras da língua portuguesa em função da mudança ortográfica--veja [Um Guia Prático da Nova Ortografia](http://www.livrariamelhoramentos.com.br/Guia_Reforma_Ortografica_Melhoramentos.pdf) (em PDF) para uma referência rápida acerca das mudanças.