#  Análise Exploratória e Preditiva de Dados Acadêmicos Sobre Evasão Escolar

Repositório reservado para a implementação da EDA e modelo preditivo como etapa avaliativa da parte prática do Trabalho de Conclusão de Curso em Análise e Desenvolvimento de Sistemas do Instituto Federal da Bahia, Campus Salvador. 

## Instruções para reproduzir localmente

**1. Clone o repositório e crie o ambiente virtual:**
```bash
git clone <url-do-repositorio>
cd previsao_evasao
python -m venv venv
venv\Scripts\activate   # Windows
```

**2. Instale as dependências:**
```bash
pip install -r requirements.txt
```

**3. Baixe os dados:**
Os dados estão disponíveis em:
- [Dados de matrícula](https://dados.gov.br/dados/conjuntos-dados/plataforma-nilo-pecanha-pnp--microdados-matriculas)

- [Dados de eficiência acadêmica](https://dados.gov.br/dados/conjuntos-dados/plataforma-nilo-pecanha-pnp---microdados-eficiencia-academica)

Clique na aba `Recursos` e baixe os arquivos CSV referentes ao ano de **2023**. Em seguida, crie a estrutura de pastas abaixo e mova os arquivos para `data/raw/`:

```
data/
├── raw/
│   ├── microdados_matriculas_2023.csv
│   └── microdados_eficiencia_academica_2023.csv
└── processed/   ← criada automaticamente ao executar os notebooks
```

## Estrutura do projeto

```
previsao_evasao/
├── data/
│   ├── raw/          # Dados brutos do PNP/SISTEC (não versionados)
│   └── processed/    # Dados processados gerados pelos notebooks (não versionados)
├── notebooks/
│   ├── 01_tratamento_matriculas.ipynb
│   ├── 02_tratamento_eficiencia.ipynb
│   └── 03_validacao_merge.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```
