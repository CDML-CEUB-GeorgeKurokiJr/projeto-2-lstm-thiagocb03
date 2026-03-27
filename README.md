# 🌍 Geopolitical Interdependence: LSTM/GRU Financial Modeling

Este repositório contém um estudo avançado de séries temporais focado no **Estreito de Ormuz** como um ponto de pressão global. A análise utiliza redes neurais profundas para correlacionar a logística energética com a viabilidade econômica de commodities industriais.

## 📋 Resumo do Projeto
A tese central propõe que a instabilidade no fluxo de petróleo e GNL (Gás Natural Liquefeito) através de Ormuz impacta diretamente o custo de produção e o preço de mercado de metais críticos. O modelo busca quantificar essa defasagem temporal entre o choque energético e a resposta do setor de mineração e siderurgia.

## 🛠️ Stack Tecnológica
* **Linguagem:** Python
* **Framework de Deep Learning:** PyTorch
* **Modelos:** LSTM (Long Short-Term Memory) e GRU (Gated Recurrent Unit)
* **Dados:** APIs financeiras (Yahoo Finance) e indicadores macroeconômicos
* **Visualização:** Matplotlib / Seaborn

## 📈 Ativos Monitorados
O modelo realiza projeções multivariadas para os seguintes clusters:
* **Energia:** Saudi Aramco, Chevron (CVX), Petróleo Brent/WTI.
* **Metais e Mineração:** Ma'aden (Arábia Saudita), Rio Tinto, Vale, Minério de Ferro.
* **Logística Geopolítica:** Foco em produtores do Catar, Emirados Árabes e Omã.

## 🧠 Arquitetura do Modelo
O notebook implementa uma abordagem de aprendizado profundo para lidar com a volatilidade:
1.  **Normalização:** Escalonamento de dados para convergência eficiente.
2.  **Janelamento (Sliding Window):** Criação de sequências temporais para predição.
3.  **Camadas Recorrentes:** Comparação de performance entre células LSTM e GRU.
4.  **Otimização:** Uso de *Adam Optimizer* e *Mean Squared Error (MSE)* para ajuste de pesos.

## 🚀 Como Utilizar
1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/nome-do-repo.git](https://github.com/seu-usuario/nome-do-repo.git)
    ```
2.  **Instale as dependências:**
    ```bash
    pip install torch pandas numpy matplotlib yfinance
    ```
3.  **Execute o Notebook:**
    Abra o arquivo `LSTM_Financas_PyTorch_Thiago_(1).ipynb` no Jupyter ou Google Colab.

---
**Autor:** Thiago Castro Barreto RA: 22301452
**Tópicos:** Finanças Quantitativas, Geopolítica, Deep Learning, PyTorch.
