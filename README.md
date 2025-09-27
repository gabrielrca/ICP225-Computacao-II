# ICP225 - Computação II

Este repositório contém o material didático da disciplina **ICP225 - Computação II**, oferecida pelo **Instituto de Computação da UFRJ**.

O conteúdo foi desenvolvido por mim (Gabriel Caldas) em **LaTeX/Beamer**, com o objetivo de apoiar as aulas e servir como referência para os alunos.  
Os slides seguem o conteúdo programático da disciplina, abordando tópicos como programação orientada a objetos, herança, polimorfismo, tratamento de exceções, persistência de dados, bibliotecas científicas, entre outros.

## Sugestões, erros ou informaçoes
Caso encontre algum erro, queira sugerir alguma coisa ou deseje pedir alguma informação, entre em contato! :)

gabrielcaldas AT ic.ufrj.br

## Estrutura

- `ICP225-Listas` → Listas de exercícios da disciplina  
- `ICP225-Slides` → Slides organizados por semana/tema  
- `ICP225-Codigo` → Códigos-fonte utilizados como exemplo nas aulas 
## Observações

Este repositório está em constante atualização.  
O uso é recomendado para alunos matriculados na disciplina, bem como demais interessados em programação orientada a objetos com Python.

## Como utilizar:

Para utilizar este repositório você deve clonar e compilar o Latex localmente. 

Os passos abaixo são os que eu utilizo para fazer a compilação local usando CachyOS (distro baseada em Arch)

Obs: Para ouras distro, eu nunca fiz (se souber fazer, me fala que eu atualizo aqui), para Mac e Windows (...)

Obs2: Dá pra zipar e usar no overleaf também.

### 1. Para instalar o Latex:
```bash
sudo pacman -S texlive-basic texlive-latex texlive-latexextra texlive-fontsextra texlive-langportuguese texlive-binextra texlive-pictures texlive-mathscience
```

### 2. Para instalar o pearl (que é necessário para autoidentação no vscodium)
```bash
sudo pacman -S perl-yaml-tiny perl-file-homedir perl-file-which perl-capture-tiny
```

Feito isso, adicione `/usr/bin/latexindent` no Vscodium para ativar a auto identação do latex da seguinte forma: 

- Insale o `LaTeX Workshop` no VSCodium
- Após instalar, edite o `settings.json` com o seguinte:

```bash
"latex-workshop.formatting.latexindent.path": "/usr/share/texmf-dist/scripts/latexindent/latexindent.pl",
  "latex-workshop.latexindent.modifyLineBreaks": true,
  "editor.wordWrap": "on",
  "editor.formatOnSave": true,
  "[latex]": {
    "editor.formatOnSave": true
  },
  "latex-workshop.formatting.latex": "latexindent",
```