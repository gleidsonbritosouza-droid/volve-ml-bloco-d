# Bloco D - Tema D2: Previsão de Produção (Arps vs. Deep Learning)

Repositório individual desenvolvido por **Gleidson Henrique Brito de Souza** no âmbito do Trabalho Computacional da disciplina PPGGF0123 na UFPA, integrado ao Bloco D (Engenharia de Reservatório - Campo de Volve).

## 📌 Pergunta de Pesquisa
> *"Quando o deep learning supera Arps, e por quanto tempo à frente a previsão continua confiável?"*

## 🛠️ Metodologia e Etapas
1. **Análise Exploratória (EDA) e Limpeza de Dados:**
   - Leitura da base de dados do campo de Volve (`Daily Production Data`) via Databricks Volumes.
   - Filtragem de dias produtivos ativos e construção da coluna de tempo acumulado (`DIAS_PRODUCAO`).
2. **Baseline Tradicional:**
   - Ajuste do modelo de declínio exponencial e hiperbólico de **Arps** utilizando `scipy.optimize.curve_fit`.
3. **Próximas Etapas (Machine/Deep Learning):**
   - Implementação de modelos com XGBoost, LSTM e TCN.
   - Validação temporal estrita (últimos 20% do histórico de produção) e *walk-forward*.
   - Análise de incerteza (P10, P50, P90) e explicabilidade com SHAP.

## ⚙️ Requisitos do Ambiente (`requisitos.txt`)
- pandas
- numpy
- matplotlib
- scipy
- openpyxl
