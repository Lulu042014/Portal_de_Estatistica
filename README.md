# Portal de Estatística e Ciência de Dados

Portal web interativo com conteúdo introdutório e tutoriais de Estatística e Ciência de Dados, desenvolvido como projeto de extensão da **Universidade Federal do Ceará (UFC) — Campus de Itapajé**.

🔗 **Site publicado:** https://lulu042014.github.io/Portal_de_Estatistica/

## Sobre o projeto

O portal busca facilitar a transição entre a teoria estatística e sua aplicação prática em código (R e Python), oferecendo conteúdo acessível para estudantes de ensino médio, graduação e para a comunidade externa.

Coordenação: **Prof. Dr. Hitalo Joseferson Batista Nascimento**

Para mais detalhes sobre justificativa, metodologia, organização das equipes e próximos passos, veja a página [Sobre o Projeto](https://lulu042014.github.io/Portal_de_Estatistica/sobre.html) no site.

## Conteúdo

- Fundamentos de Ciência de Dados
- Fundamentos de Programação
- Ferramentas e Linguagens
- Introdução a R
- Introdução a Estatística e Probabilidade
- Estatística Descritiva
- Probabilidade
- Inferência Estatística
- Pré-processamento e Limpeza de Dados
- Visualização de Dados

## Tecnologias

- [Quarto](https://quarto.org/) — geração do site
- R e Python — conteúdo e exemplos executáveis (histogramas, regressões, testes de hipótese, pipelines de pré-processamento, simulações Monte Carlo)
- Git / GitHub — versionamento
- GitHub Pages — publicação

## Rodando localmente

**Pré-requisitos:**

- [Quarto CLI](https://quarto.org/docs/get-started/)
- R, com os pacotes `knitr`, `rmarkdown`, `reticulate`, `ggplot2` e `dplyr`
- Python, com os pacotes `jupyter`, `nbformat`, `ipykernel`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy` e `scikit-learn`

> ⚠️ Se os blocos de código Python derem erro de `ModuleNotFoundError` ao renderizar (mesmo com os pacotes instalados), confira se o kernel Jupyter usado pelo `reticulate` aponta para o Python certo: `jupyter kernelspec list`, e edite o `kernel.json` correspondente para usar o caminho completo do interpretador Python do seu ambiente.

```bash
git clone https://github.com/Lulu042014/Portal_de_Estatistica.git
cd Portal_de_Estatistica
quarto render      # gera o site em _site/
quarto preview      # visualiza localmente com hot reload
```

## Publicando atualizações

```bash
quarto publish gh-pages
```

## Estrutura do repositório

```
├── _quarto.yml                    # configuração do site e navbar
├── .gitignore                     # ignora cache do Quarto, .Rproj.user, _site, etc.
├── index.qmd                      # página inicial
├── sobre.qmd                      # sobre o projeto
├── FCD.qmd                        # Fundamentos de Ciência de Dados
├── FP.qmd                         # Fundamentos de Programação
├── FL.qmd                         # Ferramentas e Linguagens
├── r.qmd                          # Introdução a R
├── IEP.qmd                        # Introdução a Estatística e Probabilidade
├── descritiva.qmd                 # Estatística Descritiva
├── PD.qmd                         # Probabilidade
├── IF.qmd                         # Inferência Estatística
├── PLD.qmd                        # Pré-processamento e Limpeza de Dados
├── visualizacao.qmd               # Visualização de Dados
└── apresentacoes_e_documentos/    # materiais de apoio do projeto
```

## Equipe

Projeto de extensão com 8 alunos organizados em quatro frentes: Conteúdo Teórico, Conteúdo Aplicado, Simulações e Plataforma/Deploy.

## Licença

Nenhuma licença definida ainda.