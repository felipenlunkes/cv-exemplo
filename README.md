# Olá!

<div align="justify">

Esse repositório visa exemplificar a criação de um currículo legível (para humanos e robôs) em Markdown, além da sua conversão para PDF.

## Dependências

* [Pandoc](https://pandoc.org/)
* texlive-latex-base
* texlive-latex-recommended 
* texlive-latex-extra

Para instalar as dependências, no Ubuntu/Debian/Pop!_OS (ou no WLS2 para Windows 10 e 11), use, no terminal:

```shell
sudo apt install pandoc texlive-latex-base texlive-latex-recommended texlive-latex-extra
```

> É possível realizar a conversão para PDF no Windows, mas você precisará instalar os pacotes adicionais manualmente (`texlive-latex-base`, `texlive-latex-recommended` e `texlive-latex-extra`).
  
## Editar o currículo e gerar versão em PDF

Você pode editar o currículo utilizado como exemplo (meu currículo) e gerar a versão em PDF.

Durante a edição, tenha em mente:

* Use `$\hrulefill$` como `<hr>`. A tag `<hr>` não é suportada, e para isso, entramos com uma tag LaTeX;
* Use `<div align="justify">` para justificar o texto. A centralização (`<div align="center">`) não parece funcionar, entretanto;
* Você pode alterar os parâmetros de fonte, no cabeçalho do arquivo, bem como a formatação e recuo da página;
* Adicione um link para seu LinkedIn, GitHub e redes sociais profissionais (evite redes sociais voltadas a seu lado pessoal, como Instagram pessoal, mas use seu Instagram profissional, se tiver);
* Adicione seus projetos mais relevantes separados por linguagem, framework ou tecnologia.

Após a edição, converta o arquivo para o formato PDF utilizando, no terminal:

```shell
pandoc currículo.md -o currículo.pdf
```

Você também pode executar o script buildPDF.sh, disponível no repositório, para gerar, em lote, mais de uma versão do seu currículo, usando, no terminal:

```shell
./buildPDF.sh
```

> Esse script é útil para automatizar a conversão de mais de um currículo. O ideal é que você construa um currículo personalizada para cada área/vaga.

## Contato

Qualquer dúvida, sinta-se a vontade em entrar em contato comigo **por email** em felipenldev@gmail.com.
  
</div>
