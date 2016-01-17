## Onde obter o pdf mais recente?

O projeto foi recem migrado para o github e ainda não há uma versão em pdf disponível, no momento você pode clonar o repositório e compilar o livro usando o LaTeX.

Você pode clonar este repositório com o comando:

```
git clone git@github.com:voyeg3r/vimbook.git
```

## Para gerar o livro

### PDF

Você deve ter instalado o LaTeX e o mesmo deve usar codificação utf8.

Para gerar o livro em PDF entre no diretório `src` e execute o comando:

```
make
```

Se tudo correr bem você terá o livro `vimbook.pdf`. Mova o arquivo pdf para um local seguro e limpe o repositório usando o comando:

```
make clean
```

### ePUB

É possível gerar o livro no formato `ePUB` utilizando o [pandoc](http://pandoc.org/).

No Ubuntu, utilize os seguintes comandos para gerar o arquivo ePUB:

```
sudo apt-get install pandoc
pandoc -s vimbook.tex -o vimbook.epub
```

## Como contribuir com o projeto?

Um novo canal de comunicação será disponibilizado, por enquanto sugestóes podem ser enviadas via pull request ou issues.
