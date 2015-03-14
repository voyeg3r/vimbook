Iniciando o vim em modo fullscreen

If you want to start in fullscreen mode add this to your vimrc:
source: http://amix.dk/blog/viewEntry/19403
```
if has("gui_running")
  set fuoptions=maxvert,maxhorz
  au GUIEnter * set fullscreen
endif
```

## Abrindo código de páginas web no gvim ##
http://vivaotux.blogspot.com/2009/06/exibindo-o-codigo-fonte-das-paginas-web.html

indentar em modo normal, use duas vezes igualdade


tip: http://vim.wikia.com/wiki/VimTip478

## anotações do dia 21 de abril ##
```
 >i{  ........... indenta o conteúdo do bloco atual (posicione sobre { de abertura)
 [d ............. mostra definição de função antes do cursor
 ]d ............. mostra definição de função após o cursor
 [D ............. mostra todas as definições
 ]i ............. mostra definição de variável 
 ]I ............. (testar) mostrar todas as definições de variável
 [<Ctrl-D> ...... salta para definição de função
```

## alterações sugeridas em 4 de abril de 2009 ##
Na tabela contida na página 14 adicionar as letras 'o' e 'O' como atalhos
para entar no modo de inserção.

Abrir mais espaço antes e depois da tabela

Na página  69 juntar os últimos parágrafos

"kp      - print macro k


## Inclusão de uma seção enumerate ##
na seção: 10.2.1 Dicionáario português segundo o acordo ortográfico
vou colocar oportunamente um ambiente 'enumerate'.

## Como fazer o vim reconhecer automaticamente o compilador? ##
**http://vim.wikia.com/wiki/Autoselect_the_right_compiler_using_the_filetype**

## Sugestões do Mitre para o livro ##
Alterando a mensagem original para ficar apenas com o que ainda não está feito.

Há muita informação, muito concentrada, ou seja, falta fluência.
Falta dinâmica e didática.

Estou trabalhando nisso.

J. F. Mitre

```
ESTE TRECHO (COM POSSÍVEIS MODIFICAÇÕES) TALVEZ VENHA A FAZER PARTE DO 
CAPÍTULO SOBRE A LINGUAGEM DE SCRIPT DO VIM
Quando nos acostumamos um pouco com o vim percebemos que, diferentemente
da maioria dos editores ele possui uma linguagem de programação própria, 
é bem verdade que alguns processadores de texto suportam macros e escripts
como é o caso do Microsoft Word\circledR, mas sua "linguagem de programação"
 interna, não é nada amigável. 
```

```
Estive lendo sobre como renderizar melhor o pdf
procurando no google por: "latex better render pdf"
http://www.cc.gatech.edu/gvu/ccg/resources/latex2pdf.html
http://www.softwarelivre.ufsc.br/pipermail/gufsc/2004-October/000738.html
```

## python no vim ##
fonte: http://blog.sontek.net/2008/05/11/python-with-a-modular-ide-vim/
```
$ ctags -R -f ~/.vim/tags/python.ctags /usr/lib/python2.5/
and then in your .vimrc

set tags+=$HOME/.vim/tags/python.ctags
autocmd FileType python set omnifunc=pythoncomplete#Complete
inoremap <Nul> <C-x><C-o>

syn match pythonError "^\s*def\s\+\w\+(.*)\s*$" display
syn match pythonError "^\s*class\s\+\w\+(.*)\s*$" display
syn match pythonError "^\s*for\s.*[^:]$” display
syn match pythonError “^\s*except\s*$” display
syn match pythonError “^\s*finally\s*$” display
syn match pythonError “^\s*try\s*$” display
syn match pythonError “^\s*else\s*$” display
syn match pythonError “^\s*else\s*[^:].*” display
syn match pythonError “^\s*if\s.*[^\:]$” display
syn match pythonError “^\s*except\s.*[^\:]$” display
syn match pythonError “[;]$” display
syn keyword pythonError         do
```

## Como arrumar um parágrafo ##
```
em modo normal gqap
```


```
Diretório do google sobre o vim (fontes de pesquisa)
http://directory.google.com/Top/Computers/Software/Editors/Vi/
```

Setar automaticamente o diretório do buffer como padrão
(na seção personalização)
```
set autochdir 
" quando esta opção está ativa alguns plugins podem não funcionar
```

Escrever sobre o comando
```
 :dig
```


Voltar para TableOfContents