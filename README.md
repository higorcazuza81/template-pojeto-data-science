# Estrutura de Diretórios para Projetos de Data Science

## Visão Geral

Este repositório oferece uma estrutura padrão para organização de projetos de Data Science. A estrutura foi desenhada para ser flexível e adequada a diferentes tipos de projetos, garantindo clareza, reprodutibilidade e fácil colaboração. Este README também fornece exemplos de documentos que podem ser armazenados em cada diretório.

## Estrutura de Diretórios

```plaintext
    project-name/
    │
    ├── README.md              # Descrição geral do projeto, instruções de configuração e execução
    ├── data/
    │   ├── raw/               # Dados brutos, diretamente do fornecedor
    │   ├── processed/         # Dados processados, prontos para análise
    │   ├── external/          # Dados de fontes externas, não brutos, mas complementares
    │   └── interim/           # Dados intermediários durante o processo de limpeza e transformação
    │
    ├── notebooks/             # Jupyter Notebooks para exploração e análises iniciais
    │   ├── 01-data-exploration.ipynb
    │   └── 02-modeling.ipynb
    │
    ├── scripts/               # Scripts de Python para manipulação de dados, treinamento de modelos, etc.
    │   ├── data_preparation.py
    │   ├── feature_engineering.py
    │   └── model_training.py
    │
    ├── src/                   # Código-fonte do projeto, incluindo módulos reutilizáveis e funções
    │   ├── __init__.py        # Arquivo que torna o diretório um pacote Python
    │   ├── data_loader.py     # Funções para carregar e pré-processar dados
    │   ├── train_model.py     # Código para treinar modelos
    │   └── evaluate_model.py  # Código para avaliar modelos
    │
    ├── tests/                 # Testes unitários e de integração para o código
    │   ├── test_data_loader.py
    │   ├── test_train_model.py
    │   └── test_evaluate_model.py
    │
    ├── results/               # Resultados das análises, como gráficos, tabelas e relatórios
    │   ├── figures/
    │   └── reports/
    │
    ├── environment/           # Arquivos relacionados ao ambiente, como conda environment e requirements
    │   ├── environment.yml    # Arquivo de configuração do ambiente conda
    │   ├── requirements.txt   # Lista de pacotes pip (para compatibilidade)
    │   └── setup.py           # Script para configurar o pacote se necessário
    │
    └── .gitignore             # Arquivo para especificar quais arquivos/pastas não devem ser versionados pelo git
```
## Descrição das Pastas

- **data/**: Diretório onde todos os dados do projeto são armazenados.
  - **raw/**: Dados brutos, que não foram processados. Exemplo: `dataset.csv`.
  - **processed/**: Dados que foram processados e estão prontos para análise. Exemplo: `cleaned_data.csv`.
  - **external/**: Dados de fontes externas que complementam o dataset principal. Exemplo: `external_data.xlsx`.
  - **interim/**: Dados intermediários durante o processo de ETL (Extract, Transform, Load). Exemplo: `interim_data.csv`.

- **notebooks/**: Diretório para armazenar notebooks Jupyter usados para a exploração de dados, desenvolvimento de modelos, e visualizações preliminares. Exemplo: `01-data-exploration.ipynb`.

- **scripts/**: Diretório para scripts Python que executam tarefas específicas como preparação de dados, engenharia de features, e treinamento de modelos. Exemplo: `data_preparation.py`.

- **src/**: Diretório contendo o código-fonte do projeto. Este código geralmente é modular e pode ser reutilizado. Exemplo: `data_loader.py`.

- **tests/**: Diretório para testes unitários e de integração, assegurando a qualidade do código. Exemplo: `test_data_loader.py`.

- **results/**: Diretório para armazenar os resultados das análises, como gráficos, relatórios, e tabelas geradas. Exemplo: `analysis_plot.png`.

- **environment/**: Contém arquivos de configuração do ambiente, como `environment.yml` para configuração com conda, e `requirements.txt` para instalação de pacotes com pip.

- **.gitignore**: Arquivo para listar arquivos e diretórios que não devem ser versionados.
  
## Como Usar

Para utilizar essa estrutura em seus projetos:

### 1. Clone o repositório para sua máquina local:
   ```bash
      git clone https://github.com/seu-usuario/estrutura-data-science.git
   ```
### 2. Renomeie o diretório clonado para o nome do seu projeto:
   ```bash
   mv estrutura-data-science/ nome-do-seu-projeto/
   ```
### 3. Personalize o README e a estrutura de diretórios conforme necessário.

Exemplo de README.md:

```markdown
    # Projeto de Análise de Dados

    Este projeto tem como objetivo analisar dados de vendas de uma empresa e prever as vendas futuras.

    ## Estrutura de Diretórios

    - **data/**: Dados brutos, processados e intermediários.
    - **notebooks/**: Notebooks Jupyter para exploração de dados.
    - **scripts/**: Scripts Python para preparação de dados e treinamento de modelos.
    - **src/**: Código-fonte do projeto.
    - **tests/**: Testes unitários e de integração.
    - **results/**: Resultados das análises.
    - **environment/**: Configuração do ambiente.

    ## Configuração

    1. Instale os pacotes necessários:
    ```bash
    conda env create -f environment/environment.yml
    ```
    2. Ative o ambiente conda:
    ```bash
        conda activate nome-do-ambiente
        ```
    3. Execute os scripts e notebooks conforme necessário.

    ## Contribuições

    Contribuições são bem-vindas! Por favor, abra uma issue ou envie um pull request com sugestões ou melhorias.

    ## Licença

    Este projeto é licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

    ## Contato

    - **Nome:** SeuNome
    - **Email:** EndereçoDeEmail@exemplo.com
    - **LinkedIn:** [linkedin.com/in/nome](https://www.linkedin.com/in/nome)
```
   
### 4. Comece a adicionar seus dados, notebooks, scripts e código-fonte ao projeto.

## Contribuições

Contribuições são bem-vindas! Por favor, abra uma issue ou envie um pull request com sugestões ou melhorias.

### Agradecimentos

Este projeto contou com a contribuição de:

- [Janaína Cazuza](https://github.com/janainacazuza/janainacazuza)

## Licença

Este projeto é licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Contato

- **Nome:** Higor Cazuza
- **Email:** higorcazuza@gmail.com
- **LinkedIn:** [linkedin.com/in/higorcazuza](https://www.linkedin.com/in/higorcazuza)




