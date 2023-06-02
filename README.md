# Olá!

<div align="justify">

Esse repositório visa exemplificar a criação de um currículo legível (para humanos e robôs) em Markdown, além da sua conversão para PDF.

## Dependências

* [Pandoc](https://pandoc.org/)
* texlive-latex-base
* texlive-latex-recommended 
* texlive-latex-extra

Para instalar as dependências, no Ubuntu/Debian/Pop!_OS, use, no terminal:

```shell
sudo apt install pandoc texlive-latex-base texlive-latex-recommended texlive-latex-extra
```

## Editar o currículo e gerar versão em PDF

Você pode editar o currículo utilizado como exemplo (meu currículo) e gerar a versão em PDF utilizando, no terminal:

```shell
pandoc currículo.md -o currículo.pdf
```

Você também pode executar o script buildPDF.sh, disponível no repositório, para gerar, em lote, mais de uma versão do seu currículo, usando, no terminal:

```shell
./buildPDF.sh
```

## Contato

Qualquer dúvida, sinta-se a vontade em entrar em contato comigo **por email** em felipenldev@gmail.com.
  
</div>
