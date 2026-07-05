Predição de Risco em Gestações com Machine Learning

Sobre o Projeto

Este projeto aborda a implementação e comparação de 6 algoritmos de Machine Learning para a previsão do risco em gestações. O objetivo principal é analisar a capacidade preditiva desses modelos para auxiliar no diagnóstico médico, classificando a gravidez em três níveis: baixo risco, médio risco e alto risco.  Utilizamos uma base de dados clínicos de gestantes de unidades de saúde de Bangladesh, o que nos exigiu uma análise cuidadosa de fatores socioeconômicos que influenciam os registros.  

O que desenvolvemos e aprendemos:

Análise e Tratamento de Dados: O dataset conta com 6 características vitais (Idade, Pressão Sistólica, Pressão Diastólica, Glicose, Temperatura Corporal e Frequência Cardíaca). Para explorar ao máximo os algoritmos, criamos três variações da base de dados: Original, Refinada (com normalização MinMaxScaler e remoção de duplicatas) e Refinada + SMOTE (para lidar com o desbalanceamento das classes gerando dados sintéticos).  

Modelagem e Otimização: Treinamos e avaliamos seis modelos diferentes: Multi-Layer Perceptron (MLP), Regressão Logística, Support Vector Machine (SVM), Árvore de Decisão, Random Forest e XGBoost. Utilizamos técnicas de validação Hold-Out e K-Fold, além de otimizar os hiperparâmetros de todos os modelos através de Grid Search.  Explicabilidade com SHAP: Aplicamos a biblioteca SHAP (SHapley Additive exPlanations) para entender o impacto de cada característica nas decisões dos modelos, trazendo transparência para os resultados clínicos.  

Conclusão e Resultados: Observamos que a preservação dos dados originais, mesmo com desbalanceamento, foi mais vantajosa do que realizar cortes excessivos. Os modelos baseados em árvores de decisão foram os mais eficazes. O melhor desempenho geral foi obtido pelo Random Forest no Dataset Original com validação K-Fold, alcançando Acurácia de 85%, F1 Score de 85%, Precisão de 85%, Recall de 85% e AUC de 98%.  

Membros da Equipe:

Arthur  
Cauã  
Dakró  
Estevão dos Santos Mello  
Leonardo  
Marcelo  
João  
Nícolas  

Dataset utilizado no trabalho:

Maternal Health Risk Data (MHRD, Bangladesh BD). Disponível no Kaggle: https://www.kaggle.com/datasets/csafrit2/maternal-health-risk-data
