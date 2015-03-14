# Alterações na página inicial #
Os detalhes sobre como se juntar ao grupo constam na página inicial do
projeto.

## Promova o grupo ##
http://groups.google.com.br/group/vimbook/manage_promote

# Introdução #

## Estrutura do diretório de trabalho ##

A estrutura (diretório) atual do SVN do projeto está assim:

```
|-- branches
|-- tags
|-- trunk
|   |-- AUTHORS
|   |-- COPYING
|   |-- README
|   `-- src
|       |-- Makefile
|       |-- img
|       |   |-- setas.png
|       |   `-- vimlogo.png
|       |-- vimbook.tex
`-- wiki
    |-- CoisasAadicionarNoLivro.wiki
    |-- EstilodeEscrita.wiki
    |-- ManualSubversion.wiki
    `-- TableOfContents.wiki
```

## Fluxo de trabalho usando o SVN ##

O fluxo básico de trabalho dos envolvidos será mais ou menos como descrito a
seguir.

Primeiramente é preciso fazer o _checkout_ inicial; este passo é feito
normalmente apenas uma única vez. A dinâmica de trabalho então concentra-se no
ciclo:

1) **svn update** (atualiza o diretório de trabalho para a versão mais recente)

2) **Edição** do projeto através da _modificação/adição_ de arquivos e **teste** das alterações (verificar o PDF resultante)
  * Adicionou um novo arquivo fonte? Então use o comando `svn add`

3) **Submeter** as alterações realizadas (`svn commit -m 'Descrição das alterações'`)
  * Alguém mexeu no mesmo arquivo neste interim e o svn acusou conflito? Não se preocupe, problemas de conflito virtualmente só ocorrem quando as alterações são feitas no mesmo trecho do arquivo. Dê um **svn update** para instruir o svn a incorporar as mudanças do outro usuário nas suas; cheque então o arquivo e confirme se está correto (caso não esteja modifique-o), teste o PDF, e finalmente submeta de novo as alterações (_commit_).

4) Retorne ao _Passo **1**_ e repita o ciclo para novas modificações

### Observações ###

Em princípio deve-se colocar os arquivos descompactados. Não coloque os arquivos temporários gerados pelo LaTeX.

No diretório 'src' fica os arquivos fontes necessários para gerar o "binário", neste caso o PDF. Assim como os binários de arquivos executáveis, não acho apropriado colocarmos o PDF sob o controle do SVN; é melhor publicarmos apenas nos _releases_ oficiais.


## Coisas a adicionar/modificar no livro ##

CoisasAadicionarNoLivro


## Como formatar o Wiki ##

Adicione seu conteúdo. Formate-o assim:
```
  * Text in *bold* or _italic_
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages

=Heading1=
==Heading2==
===Heading3===

*bold*     _italic_
`inline code`
escape: `*`

Indent lists 2 spaces:
  * bullet item
  # numbered list

{{{
verbatim code block
}}}

Horizontal rule
----

WikiWordLink
[http://domain/page label]
http://domain/page

|| table || cells ||
```

Mais exemplos [aqui](http://code.google.com/p/support/wiki/WikiSyntax).