# 🏹 Tupi or Not Tupi: Análise de Saúde e Nutrição Indígena

![Status](https://img.shields.io/badge/Status-Finalizado-success)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![License](https://img.shields.io/badge/License-MIT-green)

> "Análise dos determinantes da saúde e nutrição de crianças indígenas a partir dos bancos de dados SIASI."

## 📍 Sobre o Projeto

Este projeto tem como objetivo analisar os dados do **SIASI (Sistema de Informação da Atenção à Saúde Indígena)** para compreender o cenário nutricional e de crescimento de crianças indígenas no Brasil (2019-2022).

Através de técnicas de Ciência de Dados, buscamos identificar padrões geográficos, fatores de risco para desnutrição e aplicar modelos preditivos para auxiliar na identificação de vulnerabilidades.

## 🎯 Objetivos

* **Consolidação de Dados:** Unificar bases dispersas (Vigilância Alimentar, Acompanhamento, Pré-natal) em um *dataset* robusto.
* **Análise Geoespacial:** Mapear a distribuição de indicadores nutricionais (Peso/Idade e Altura/Idade) pelos DSEIs e municípios.
* **Inferência Estatística:** Validar hipóteses sobre o impacto do aleitamento e sexo no desenvolvimento infantil.
* **Modelagem Preditiva:** Utilizar **Random Forest** para classificar riscos de déficit de crescimento (Baixa Estatura).

---

## 🛠️ Tecnologias Utilizadas

O projeto foi desenvolvido em **Python**, utilizando as seguintes bibliotecas:

* **Manipulação de Dados:** `pandas`, `numpy`
* **Visualização:** `matplotlib`, `seaborn`, `plotly`
* **Geoprocessamento:** `geopandas`, `geobr`
* **Estatística:** `scipy` (Teste T, Qui-Quadrado)
* **Machine Learning:** `scikit-learn` (Random Forest, GridSearch, StratifiedKFold)

---

## 📊 Pipeline do Projeto

### 1. Engenharia de Dados
* Limpeza de valores nulos e padronização de variáveis categóricas.
* *Type casting* e tratamento de datas.
* Criação de variáveis (Feature Engineering), como cálculo de idade exata e categorização de desfechos nutricionais.

### 2. Análise Exploratória (EDA) & Geográfica
Realizamos uma análise profunda da distribuição demográfica e nutricional.
* **Descoberta:** Identificação da "dupla carga de má nutrição" (coexistência de baixo peso e sobrepeso em diferentes clusters geográficos).
* **Mapas Coropléticos:** Visualização interativa dos municípios com maiores índices de problemas nutricionais.

### 3. Testes de Hipóteses
* **Teste T:** Confirmou diferença estatisticamente significativa entre as alturas médias de meninos e meninas.
* **Qui-Quadrado:** Avaliou a associação entre o tipo de aleitamento e o estado nutricional.

### 4. Machine Learning (Classificação)
Desenvolvimento de um modelo de **Random Forest** para prever o risco de **Baixa Estatura para a Idade**.
* **Otimização:** Uso de *Grid Search* e *Cross-Validation* (10-fold).
* **Seleção de Features:** Redução de dimensionalidade focando nas 20 variáveis mais importantes para evitar *overfitting*.
* **Resultado:** O modelo final alcançou alta acurácia e consistência na identificação dos casos de risco.

---

## 📂 Estrutura do Repositório

```text
├── data/                  # Bases de dados (não incluídas no repo por privacidade)
├── notebooks/
│   └── tupi_or_not_tupi.ipynb  # Notebook principal com todo o pipeline
├── images/                # Gráficos e mapas gerados
├── README.md              # Documentação do projeto
└── requirements.txt       # Dependências

```

---

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone [https://github.com/seu-usuario/nome-do-repo.git](https://github.com/seu-usuario/nome-do-repo.git)

```


2. Instale as dependências:
```bash
pip install -r requirements.txt

```


*(Certifique-se de instalar bibliotecas geoespaciais como `geopandas` e `geobr` corretamente para o seu SO)*.
3. Execute o Jupyter Notebook:
```bash
jupyter notebook notebooks/tupi_or_not_tupi.ipynb

```

---

## 👥 Equipe

Projeto desenvolvido para a disciplina de Introdução à Ciência de Dados (ICD - UFMG).

* **[Lívia Caroline](https://github.com/Livia-CRPereira)**
* **[Letícia Ruas](https://github.com/LeticiaRodr)**
* **[Letícia Rosa](https://github.com/leticiarosaff)**
* **[Sophia Vieira](https://github.com/sophiaevieira)**

---

<div align="center">
<sub>Built with 💜 and Data Science</sub>
</div>

```

```

