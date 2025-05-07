# 💳 FraudSpotter: detecção inteligente de fraudes com análise de custos

Problema: Fraudes em transações financeiras representam um desafio crescente, gerando perdas significativas para empresas e clientes. A detecção eficiente de fraudes é vital para minimizar esses impactos.

## 📌 Objetivo

Este projeto explora a detecção de fraudes em transações financeiras utilizando técnicas de balanceamento de dados e o algoritmo XGBoost. O foco principal é reduzir os custos operacionais causados por previsões incorretas, considerando o impacto financeiro de falsos positivos e falsos negativos.

## 📂 Dataset

- **Fonte:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Descrição:** Conjunto de dados contendo transações com cartão de crédito realizadas por clientes europeus em setembro de 2013. As features (V1 a V28) foram transformadas por PCA para garantir privacidade.

## 🔍 Etapas do projeto

1. **Análise exploratória de dados (EDA)**
   - Visualização inicial dos dados
   - Entendendo a distribuição das classes da variável alvo
   - Analisando a correlação das variáveis explicativas com a variável alvo

2. **Pré-processamento**
   - Divisão da base de dados em conjunto de treino e teste
   - Estratégias para lidar com o desbalanceamento

3. **Ajuste dos modelos e extração de métricas**
   - Modelagem com dados originais (baseline)
   - Modelagem com o parâmetro scale_pos_weight
   - Modelagem com SMOTE
   - Comparação gráfica do desempenho dos modelos

4. **Interpretação dos resultados**
   - Análise das métricas extraídas dos modelos
   - Análise das Curvas ROC e Precision-Recall
   - Comparação entre correlação e importância das variáveis

5. **Otimização dos hiperparâmetros com GridSearchCV**

6. **Análise dos custos dos erros de classificação**
   - Discussão dos resultados da análise de custos


## 💡 Principais resultados

- As técnicas de balanceamento **melhoraram significativamente o desempenho na identificação de fraudes**.
- O modelo que utilizou a base dedados balanceada via **SMOTE** apresentou o **menor custo total** entre as abordagens testadas.
- A análise de custo demonstrou que a análise apenas das métricas tradicionais não captura totalmente o impacto financeiro das previsões incorretas.

## ✅ Conclusão

O projeto demonstrou que a análise orientada por custo é essencial em cenários críticos como detecção de fraudes. Técnicas de balanceamento de dados, quando combinadas com algoritmos robustos como o XGBoost, podem melhorar significativamente a eficácia operacional do sistema antifraude.

## 🛠️ Tecnologias utilizadas

- Python
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost

---

## Observações adicionais:

* Os códigos e visualizações geradas neste projeto podem ser encontrados no notebook `FraudSpotter.ipynb`.
* Sinta-se à vontade para entrar em contato caso tenha alguma dúvida ou sugestão.

Espero que este projeto seja útil e informativo!
