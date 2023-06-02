# Olá!

<div align="justify">

Esse repositório visa exemplificar a criação de um currículo legível (para humanos e robôs) em Markdown, além da sua conversão para PDF. Esse formato é útil para oferecer um currículo sucinto, sem distrações e que pode ser processado por mecanismos automatizados de sites de cadastro e análise de currículo (já testei diversas vezes durante a minha busca por emprego).

## Dependências

* [Pandoc](https://pandoc.org/)
* texlive-latex-base
* texlive-latex-recommended 
* texlive-latex-extra
* Um arquivo Markdown contendo seu currículo (pode usar [esta](CV.md) versão do meu currículo como exemplo). ⚠️ Leia abaixo como formatar o documento!

Para instalar as dependências, no Ubuntu/Debian/Pop!_OS (ou no WLS2 para Windows 10 e 11), use, no terminal:

```shell
sudo apt install pandoc texlive-latex-base texlive-latex-recommended texlive-latex-extra
```

> É possível realizar a conversão para PDF no Windows, mas você precisará instalar os pacotes adicionais manualmente (`texlive-latex-base`, `texlive-latex-recommended` e `texlive-latex-extra`).
  
## Editar e formatar o currículo

Você pode editar o currículo utilizado como exemplo (meu currículo) e gerar a versão em PDF.

Durante a edição, tenha em mente:

* Use `$\hrulefill$` como `<hr>`. A tag `<hr>` não é suportada, e para isso, entramos com uma tag LaTeX;
* Use `<div align="justify">` para justificar o texto. A centralização (`<div align="center">`) não parece funcionar, entretanto;
* Você pode alterar os parâmetros de fonte, no cabeçalho do arquivo, bem como a formatação e recuo da página;
* Adicione um link para seu `LinkedIn`, `GitHub` e demais `redes sociais profissionais` (evite redes sociais voltadas a seu lado pessoal, como Instagram ou Twitter pessoais, mas use seu Instagram ou Twitter profissionais, se tiver);
* Adicione seus projetos mais relevantes separados por linguagem, framework ou tecnologia. Tente sempre adicionar links para repositórios públicos, caso se trate de software livre.
  - Para isso, adicione o nome do projeto entre `[]` seguindo do link entre parênteses, sem espaço, como abaixo:
  
```markdown
* [Projeto 1](https://github.com/felipenlunkes/projeto-1)
```

# Gerar versão em PDF
  
Após a edição, converta o arquivo para o formato PDF utilizando, no terminal:

```shell
pandoc currículo.md -o currículo.pdf
```

Você também pode executar o script [buildPDF.sh](buildPDF.sh), disponível no repositório, para gerar, em lote, mais de uma versão do seu currículo, usando, no terminal:

```shell
./buildPDF.sh
```

> Esse script é útil para automatizar a conversão de mais de um currículo. O ideal é que você construa um currículo personalizada para cada área/vaga.

## Ir além
  
Você também pode criar um currículo online sempre atualizado utilizando o GitHub Pages. Basta criar um repositório, criar um arquivo index.md com seu currículo em Markdown e ativar o GitHub Pages. Assim, a cada alteração, você sempre terá um currículo atualizado. E você pode adicionar links para as versões em PDF, que também podem ser adicionadas neste mesmo repositório. Aqui vai um exemplo, a minha versão online do currículo: [CV Felipe Lunkes](https://felipenlunkes.github.io/cv/).
  
## Contato

Qualquer dúvida, sinta-se a vontade em entrar em contato comigo **por email** em felipenldev@gmail.com.
  
</div>
