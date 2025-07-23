# Análise e Modelagem de Casos de Dengue no Brasil com Inteligência Computacional 🦟

Este repositório contém a implementação de um projeto voltado à análise e modelagem de dados sobre a Dengue no Brasil. O estudo incluiu abordagens supervisionadas e não supervisionadas, sendo elas:
 - Previsão de surtos com base na série histórica por meio de regressão preditiva.
 - Clusterização de métricas agregadas por municípios para a identificação de correlação entre perfis socioclínicos e regionais.

Este projeto foi desenvolvido no âmbito da disciplina de Inteligência Computacional em Saúde, ministrada pelo professor [Andre Pacheco](https://github.com/paaatcha). 

## Sumário
 - [Base de dados](#base-de-dados)
 - [Instruções de uso](#instruções-de-uso)
   - [Repositório e Dados](#repositório-e-dados)
   - [Ambiente Virtual](#ambiente-virtual)
   - [Dependências](#dependências)
   - [Execução](#execução)
 - [Notas](#notas)
 - [Contribuidores](#contribuidores)

## Base de dados
Os dados utilizados neste projeto foram obtidos a partir do portal OpenDataSUS, mantido pelo Departamento de Informática do Sistema Único de Saúde (DATASUS) do Ministério da Saúde do Brasil. A partir do conjunto de dados “Árboviroses/ Dengue”, foram obtidos registros referentes às notificações de dengue, conforme coletados pelo Sistema de Informação de Agravos de Notificação (SINAN).

Os arquivos, disponibilizados em formato CSV, organizam notificações individuais por ano. Cada linha da base de dados representa uma notificação individual de dengue, incluindo informações sobre sinais e sintomas clínicos, comorbidades, idade, sexo, raça/cor, escolaridade, datas de início dos sintomas, notificação e evolução do caso, além de local de residência e notificação. O dicionário de dados oficial do SINAN foi utilizado como referência para interpretação e padronização das variáveis incluídas na análise.

Tanto os **dados** como o **dicionário** podem ser encontrados [aqui](https://opendatasus.saude.gov.br/dataset/arboviroses-dengue).

## Instruções de uso
Por se tratarem de arquivos `.ipynb`, podem ser executados em diversos ambientes. Todavia, recomendamos fortemente a utilização do [JupyterLab](https://jupyter.org/install) ou da [extensão](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) do Jupyter para VSCode.

### Repositório e Dados
Faça o *download* do projeto:
```bash
git clone https://github.com/intel-comp-saude-ufes/2025-1-P1-analise-e-modelagem-de-casos-de-dengue-no-brasil.git && cd 2025-1-P1-analise-e-modelagem-de-casos-de-dengue-no-brasil
```
 - Faça o *download* dos *datasets* `.csv` de 2016 à 2025 [aqui](https://opendatasus.saude.gov.br/dataset/arboviroses-dengue).
 - Mova-os para o diretório [./data](./data/)

### Ambiente virtual
Crie um ambiente virtual para isolar as dependências do projeto.
```bash
python3 -m venv venv
```
```bash
source venv/bin/activate
```

### Dependências
Instale as dependências.
```bash
pip install -r requirements.txt
```
Caso opte pela utilização do JupyterLab:
```bash
pip install jupyterlab
```

### Execução
Se estiver usando a extensão do Jupyter para VSCode, basta abrir os arquivos e clicar em `Run All`. Caso esteja no JupyterLab, execute:
```bash
jupyter lab
```
e siga o mesmo procedimento.

## Notas
 - Para uma visão mais completa sobre o projeto, confira o [artigo]().
 - Confira também a apresentação em [vídeo]().
 - Os gráficos resultantes das análises serão gerados em [./charts](./charts/).
 - É recomendável que execute os scripts em um computador com pelo menos **16GB RAM**.
 - Os detalhes de implementação estão documentados nos códigos.

## Contribuidores
 - [João Paulo Moura Clevelares](https://github.com/vortex2jm)
 - [Vinícius Cole de Amorim](https://github.com/viniciuscole)
 - [Thamya Vieira Hashimoto Donadia](https://github.com/thamyadonadia?tab=repositories)
