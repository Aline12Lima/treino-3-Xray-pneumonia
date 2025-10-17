


## 🧠 Principais Descobertas: A Análise dos Erros

A análise de cluster sobre os **59 erros de classificação** (16 Falsos Negativos e 43 Falsos Positivos) revelou três padrões de falha comportamentais distintos:
### 🔹 Cluster 1: O "Ponto Cego"
Composto por todos os 16 Falsos Negativos.  
O modelo estava **altamente confiante em seu erro**, com uma probabilidade média de predição de pneumonia de apenas **27.7%**.
### 🔹 Cluster 2: O "Alarme Falso Confiante"
Composto por 20 Falsos Positivos.  
O modelo também estava **altamente confiante em seu erro**, prevendo pneumonia com uma probabilidade média de **87.7%** em imagens normais.
### 🔹 Cluster 0: O "Erro Ambíguo"
Composto pelos 23 Falsos Positivos restantes.  
O modelo estava **menos confiante em seu erro**, com uma probabilidade média de **62.3%**, indicando **casos de fronteira**.

> 🔍 A análise visual com mapas de atenção (**CBAM**) demonstrou que a principal falha do modelo — especialmente no *"Ponto Cego"* — não é de **localização** (o modelo frequentemente foca na área correta), mas sim de **interpretação** (ele subestima a relevância das características patológicas que observa).
"""



