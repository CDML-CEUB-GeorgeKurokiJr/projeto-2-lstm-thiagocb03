#  Análise de Interdependência Geopolítica

##Modelagem via LSTM/GRU para o Mercado de Petróleo e Metais

- **Premissa Central do Estudo:** 

 O **Estreito de Ormuz** atua como um "ponto de pressão" único no comércio global. A nossa tese propõe que a instabilidade logística nesta região não afeta apenas o escoamento de energia (Petróleo), mas dita diretamente a viabilidade econômica da produção de commodities industriais (Metais).

## Objetivos da Modelagem
Através da combinação de redes neurais profundas (**LSTM e GRU**), este estudo busca:

1. **Quantificar a Defasagem Temporal:** Entender quanto tempo leva para um choque no setor energético impactar o preço dos metais.

2. **Medir a Força da Correlação:** Identificar o grau de interpendência entre esses dois aglomerados (clusters) aparentemente distintos.

3. **Projeção Multivariada:** Gerar estimativas de curto prazo para ativos críticos como Aramco, Chevron, Ma'aden e Rio Tinto.

## Estrutura Técnica do Pipeline
A análise está dividida em dois fluxos principais de dados:

- **Fluxo 1 (Energia):** Foco em Petróleo Brent/WTI e gigantes do setor (Aramco/CVX).

- **Fluxo 2 (Metais):** Foco em Minério de Ferro e Siderurgia (Ma'aden/Rio Tinto).

# 1. O Ponto de Intersecção: Geopolítica e Logística
**O Estreito de Ormuz: O "Gargalo" da Estabilidade Global**

O Estreito de Ormuz é a prova máxima de que a **Logística é refém da Geografia.** Com apenas **33 km de largura**, este ponto focal condensa uma importância desproporcional para o equilíbrio do planeta através de três pilares fundamentais:

## A. O Pulmão Energético e Industrial

- **Fluxo de Energia:** Por este canal transitam **20% do petróleo mundial**, o combustível essencial para o transporte e a infraestrutura global.

- **Hub de Metais:** O canal consolidou-se como o eixo de escoamento de metais críticos (como o **alumínio**), peças-chave para a tecnologia de ponta e a transição energética.

## B. A Simbiose Econômica: Energia + Produção
Existe uma **correlação direta** entre a estabilidade do Estreito e o custo dos materiais industriais:

- **Intensidade Energética:** A fundição de metais depende de energia barata. Países da região utilizam o gás natural local para alimentar suas indústrias. Tensões em Ormuz elevam o preço da energia, impactando o custo do metal instantaneamente no mercado mundial.

- **Logística de Via Dupla:** O canal é a artéria vital para navios graneleiros que transportam **alumina** (matéria-prima) para as refinarias locais e exportam o **metal processado** para os mercados globais.

## C. Vulnerabilidade Geopolítica
Dada a sua estreiteza física, qualquer instabilidade política (como o controle exercido pelo Irã ou conflitos regionais) cria um **efeito cascata:**

 *"O fechamento ou a simples ameaça em Ormuz trava o escoamento físico e dispara os preços globais por pura incerteza especulativa."*

# 2. Mercados Geograficamente Participantes

Os países que operam diretamente neste "cluster" e dependem do Estreito para ambos os mercados são principalmente:

| Mercado (País) | Participação no Petróleo / Gás | Participação nos Metais (Destaque) |
| :--- | :--- | :--- |
| **Emirados Árabes (EAU)** | Grande exportador (Abu Dhabi). | Gigante global no Alumínio (Emirates Global Aluminium). |
| **Irã** | Detém a costa norte do Estreito; reservas massivas. | Grande produtor regional de Aço e Cobre. |
| **Arábia Saudita** | Escoa parte da produção via Golfo (embora tenha portos no Mar Vermelho). | Investimento massivo em Ouro, Fosfato e Alumínio (**Ma'aden**). |
| **Catar** | Maior exportador de GNL (Gás Natural Liquefeito) do mundo via Ormuz. | Produção de Alumínio de alta pureza (**Qatalum**). |
| **Omã** | Controla a costa sul do Estreito (Musandam). | Exportador de Cromita, Ferro e Cobre. |

# 3. Dinâmica dos Aglomerados (Clusters)

**O Aglomerado do Petróleo: O Termômetro da Energia**

Para que o modelo compreenda a volatilidade de Ormuz, definimos o **Cluster de Energia** como o "driver" primário. A lógica científica aqui é clara: a instabilidade no Estreito gera um **"Prêmio de Risco"** imediato nos preços do barril (Brent) e do Gás Natural.

Como a maioria das commodities metálicas é negociada em dólares, a flutuação do petróleo impacta o câmbio global e, por consequência, os preços na London Metal Exchange (LME), criando um efeito cascata que o nosso modelo LSTM/GRU deve mapear.

###Ativos Sentinelas do Cluster:

**Saudi Aramco (2222.SR):** A maior petrolífera do mundo e o ativo definitivo para este estudo. Como sua infraestrutura depende criticamente do escoamento pelo Golfo Pérsico, qualquer tensão geopolítica em Ormuz reflete instantaneamente em seu valor de mercado.

**TotalEnergies (TTE):** Escolhida por sua exposição massiva ao GNL (Gás Natural Liquefeito) e petróleo no Catar e Emirados Árabes. Ela representa o capital global e o fluxo físico de energia que atravessa o Estreito diariamente.

# 4. O Aglomerado dos Metais: A "Eletricidade Sólida"

Enquanto o primeiro cluster foca na fonte de energia, o **Aglomerado de Metais** foca no produto final da industrialização regional. A região do Golfo consolidou-se como um hub global de Alumínio por uma razão física simples: o alumínio é, na prática, **"eletricidade sólida"**.

O modelo LSTM/GRU processa esta dependência através de um ciclo de três etapas que o Estreito de Ormuz torna vulnerável:

1. **Conversão Energética:** O gás natural extraído próximo ao Estreito é convertido em eletricidade de baixo custo.

2. **Eletrólise:** Essa energia alimenta as cubas de fundição, transformando a alumina em metal.

3. **Escoamento Global:** O metal resultante é exportado via Ormuz para as indústrias da Ásia e Europa.

###Ativos Sentinelas da Indústria:

- **Ma'aden (1211.SR):** A gigante da mineração da Arábia Saudita. Ela opera em toda a cadeia de alumínio, ouro e cobre. No contexto deste estudo, é o "par perfeito" para a Aramco, pois permite à rede neural aprender como as oscilações no custo da energia impactam diretamente as margens da mineração.

- **Rio Tinto (RIO):** Gigante global e operadora de diversas joint-ventures de alumínio. Ela representa a oferta global de metais e a sensibilidade do setor industrial aos choques logísticos e energéticos que ocorrem no gargalo de Ormuz.

# 5. Configuração de Ativos para a Rede LSTM

Para que o modelo capture tanto o impacto regional quanto o reflexo global das tensões no Estreito de Ormuz, selecionamos um mix estratégico de ativos "âncora" e ativos "globais".

### **Tabela de Ativos para a Rede LSTM**

| Ativo | Ticker (Yahoo Finance) | Aglomerado | Por que usar? |
| :--- | :--- | :--- | :--- |
| **Saudi Aramco** | 2222.SR | **Petróleo** | Representa a oferta bruta e o risco geopolítico local. |
| **TotalEnergies** | TTE | **Petróleo** | Representa o fluxo global de energia e GNL via Ormuz. |
| **Ma'aden** | 1211.SR | **Metais** | Representa a transformação industrial e o custo de energia. |
| **Rio Tinto** | RIO | **Metais** | Representa a oferta mundial e a sensibilidade logística global. |

### 🎯 Objetivos da Configuração

Esta seleção foi desenhada para garantir que a rede **LSTM** capture de forma integrada:

* **Raízes Regionais:** O fechamento de ativos com operações críticas no Golfo (`2222.SR` e `1211.SR`).
* **Reflexo Global:** A dinâmica de preços de gigantes multinacionais (`TTE` e `RIO`).
* **Sincronia de Mercado:** Juntos, esses ativos servem como o **reflexo financeiro do Estreito de Ormuz**, permitindo que o modelo identifique padrões de contágio entre os setores de energia e mineração.

#  6. O Ponto Cego Geopolítico
### O Risco do Calendário Assíncrono (Domingos e Sextas)

Um dos maiores desafios deste modelo é lidar com a **desconexão de calendários** entre as bolsas do Golfo e as bolsas Ocidentais. O Estreito de Ormuz não "fecha" no final de semana, e ignorar essa dinâmica criaria um "ponto cego" na rede neural.

#### **A Importância da Continuidade de Dados:**

* **O Domingo na Arábia Saudita:** No Golfo, o domingo é o primeiro dia útil da semana. Se um evento crítico ocorre no sábado em Ormuz, a **Saudi Aramco (2222.SR)** reage imediatamente no domingo. Se deletarmos o domingo para "padronizar" com o mercado americano, a rede neural só veria o impacto na segunda-feira, perdendo a **Causalidade Imediata**.
* **A Sexta-feira no Ocidente:** É o dia em que os traders globais ajustam suas posições de proteção (*Hedge*) contra riscos de fim de semana. Sem os dados de sexta, o modelo perde o "Sentimento de Risco" capturado pela **Total (TTE)** e **Rio Tinto (RIO)**.

> **Decisão Técnica:** Para evitar a perda de correlação, o pipeline de dados foi desenhado para preencher as lacunas (*Forward Fill*), garantindo que a **LSTM** sempre tenha uma visão contínua dos movimentos de preço, independentemente do fuso horário da bolsa de origem.

#  7. Setup e Sincronização: A Base do Modelo LSTM

Este estágio estabelece o ecossistema computacional (**PyTorch, NumPy, Pandas**) e define os três pilares críticos para a integridade dos tensores que alimentarão a rede neural. Sem este rigor técnico, a correlação entre o Petróleo e os Metais seria perdida em ruídos de processamento.

### **Os Três Pilares da Integridade de Dados**

#### **1. Sincronização Multimercado (O Ponto Sensível)**
Devido à natureza assíncrona das bolsas (Golfo vs. Ocidente), a extração via `yfinance` gera lacunas temporais inerentes.
* **Ação:** O alinhamento rigoroso via `pd.concat` é seguido por um tratamento de valores nulos (`NaN`). Isso evita que a rede processe datas inexistentes em um dos mercados, o que causaria "alucinações" no aprendizado de máquina.

#### **2. Normalização de Dados (MinMaxScaler)**
Ativos como **Saudi Aramco** e **Rio Tinto** operam em escalas de preço e volatilidade completamente distintas.
* **Ação:** Aplicamos o `MinMaxScaler` em todas as *features* (preços e indicadores técnicos). Isso garante que a rede aprenda **padrões de movimento e correlação**, e não seja enviesada por magnitudes nominais de preço.

#### **3. Gestão de Hardware (Device Management)**
Para garantir a performance e evitar erros de execução (Runtime Errors):
* **Ação:** Implementamos a lógica de `device management`, movendo tensores e modelos para o mesmo barramento de memória (seja **CPU** ou **GPU/CUDA**). A paridade entre os dados e a arquitetura é fundamental para a estabilidade do treinamento.

> **Nota Técnica:** A consistência entre a escala dos dados de entrada e a função de ativação da última camada da rede é o que permite a convergência do erro (Loss) de forma suave.

#  8. A Quebra da Sequência Temporal (Impacto em LSTM/GRU)

As redes neurais recorrentes, como **LSTM** (Long Short-Term Memory) e **GRU** (Gated Recurrent Unit), operam sob o princípio da **continuidade temporal**. Para essas arquiteturas, a ordem e o espaçamento dos dados não são apenas detalhes, mas a base de sua memória interna.

#### **O Perigo dos "Buracos" Artificiais**

* **Distorção de Vizinhança:** Se ignorarmos a Sexta-feira (Ocidente) e o Domingo (Golfo), criamos uma lacuna artificial. Para a rede, o fechamento de quinta-feira e a abertura de segunda-feira parecerão vizinhos imediatos. Na realidade, houve um intervalo de **72 horas** de eventos geopolíticos latentes que o modelo deixaria de "sentir".
* **Impacto nos Indicadores Técnicos:** Indicadores como **Média Móvel (SMA/EMA)** e **RSI** (Índice de Força Relativa) dependem de uma janela constante de tempo para serem precisos. Uma sequência interrompida distorce o cálculo da volatilidade e do momento, gerando sinais falsos de compra ou venda.



> **Conclusão Lógica:** Ao mantermos a sequência intacta (via preenchimento de lacunas), garantimos que os estados ocultos (*hidden states*) da LSTM capturem a **inércia real** do mercado, permitindo que o modelo "lembre" do risco acumulado durante o final de semana no Estreito de Ormuz.

#  9. Preparação do Ambiente (Setup de Dependências)

Antes de iniciarmos a extração de dados e a arquitetura da rede, precisamos garantir que o ambiente do Google Colab possua as bibliotecas de última geração para processamento financeiro e Deep Learning.

!pip install yfinance matplotlib scikit-learn torch --quiet

# 10. Importação do Arsenal Tecnológico

Nesta etapa, carregamos as ferramentas que transformarão os dados brutos de mercado em tensores processáveis pela nossa rede neural. Cada biblioteca cumpre um papel fundamental na arquitetura:

* **Manipulação de Dados:** `Pandas` e `NumPy` para o tratamento das séries temporais assíncronas.
* **Visualização:** `Matplotlib` para o monitoramento da convergência da *Loss* e tendências de preço.
* **Deep Learning (PyTorch):** O motor principal do modelo, incluindo as camadas de rede (`nn`) e os carregadores de dados (`DataLoader`).
* **Pré-processamento:** `MinMaxScaler` para garantir a normalização técnica discutida anteriormente.

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import yfinance as yf
from sklearn.preprocessing import MinMaxScaler
import torch
import torch.nn as nn
from torch.utils.data import Dataset, DataLoader

#  11. Engenharia de Features: Construindo a "Assinatura" do Mercado

Para que a rede **LSTM/GRU** não apenas "veja" o preço, mas "entenda" o contexto geopolítico, aplicamos uma lógica de extração de características através da função `add_indicators`. Ela gera uma assinatura comportamental para cada ativo, transformando dados brutos em sinais de entrada de alta relevância.

### **Os Pilares da Assinatura Comportamental:**

* **Tendência (SMA/EMA):** Médias Móveis Simples e Exponenciais. Atuam como um filtro que remove o "ruído" volátil das notícias diárias, permitindo que o modelo identifique o **movimento estrutural** de preços causado por tensões prolongadas no Estreito.
* **Momentum (RSI):** O Índice de Força Relativa mede a velocidade e a força da variação de preço. No nosso contexto, funciona como um medidor do **"Pânico do Mercado"**, sinalizando níveis de sobrecompra ou sobrevenda decorrentes de choques externos.
* **Target (Close):** O preço de fechamento é mantido como a variável dependente final, servindo de âncora para o aprendizado e a validação das previsões da rede.

# --- FUNÇÃO DE INDICADORES OTIMIZADA PARA REDES NEURAIS ---

def add_indicators(df, col='Close', window=14):
    """
    Calcula indicadores técnicos estruturados para entrada em modelos de Deep Learning.
    O uso de EWM (Exponential Weighted) em vez de médias simples nos osciladores
    ajuda a suavizar a transição de dados e acelera a convergência do gradiente.
    """

    # 1. Médias Móveis (Captura de Tendência Estrutural)
    df[f'SMA_{window}'] = df[col].rolling(window=window).mean()
    df[f'EMA_{window}'] = df[col].ewm(span=window, adjust=False).mean()

    # 2. RSI (Oscilador de Momentum - Método de Wilder para estabilidade)
    delta = df[col].diff()
    gain = delta.clip(lower=0)
    loss = -delta.clip(upper=0)

    # Nota: O uso de ewm (Exponential Weighted) evita "saltos" bruscos
    # nos dados de treino, estabilizando o aprendizado da LSTM.
    avg_gain = gain.ewm(alpha=1/window, min_periods=window, adjust=False).mean()
    avg_loss = loss.ewm(alpha=1/window, min_periods=window, adjust=False).mean()

    rs = avg_gain / (avg_loss + 1e-9) # Adição de epsilon para evitar divisão por zero
    df[f'RSI_{window}'] = 100 - (100 / (1 + rs))

    # Opcional: Descomente a linha abaixo para normalizar o RSI entre 0 e 1,
    # o que pode otimizar ainda mais o desempenho do Adam Optimizer.
    # df[f'RSI_{window}'] = df[f'RSI_{window}'] / 100.0

    return df

# 12. A Engenharia da Memória: Sincronização via Forward Fill (ffill)

Para que a rede **LSTM/GRU** compreenda a causalidade entre o Golfo e o Ocidente, substituímos a exclusão de dados (`.dropna()`) por uma técnica de preenchimento inteligente: o **Forward Fill (`.ffill()`)**.

### **A. O Desafio do Alinhamento de Calendários**
Ao unir os dados com `pd.concat(axis=1)`, o Pandas cria uma linha para cada data única global. Isso gera lacunas inevitáveis:
* **Domingo:** A **Saudi Aramco** opera, mas a **TotalEnergies** (Paris) gera um valor nulo (`NaN`).
* **Sexta-feira:** A **TotalEnergies** opera, mas as bolsas do Golfo geram um valor nulo (`NaN`).

### **B. A Mecânica do Forward Fill (`ffill`)**
O comando `ffill()` instrui o modelo: *"Se encontrar um valor nulo, mantenha o último preço de fechamento conhecido"*.

**Exemplo Prático:**
1. **Sexta-feira:** TotalEnergies fecha a **60€**.
2. **Domingo:** A Aramco sobe **2%** em Riade devido a uma tensão em Ormuz. A Total está fechada.
3. **Ação do ffill:** O sistema assume que a Total "vale" os mesmos **60€** no domingo.



### **C. Por que isso é vital para a Rede Neural?**

* **Continuidade dos Indicadores (RSI/SMA):** Indicadores técnicos exigem janelas de tempo constantes. O `ffill` impede "saltos" matemáticos artificiais que confundiriam o gradiente da rede.
* **Causalidade Geopolítica:** A rede agora "enxerga" que a Aramco se moveu no domingo enquanto a Total estava estática. Na segunda-feira, ao abrir, a rede já possui a **memória do movimento prévio**, permitindo identificar se um ativo antecipa o outro.
* **Volume de Treinamento:** Ganhamos aproximadamente **20% mais dados** úteis, evitando o desperdício de informações críticas ocorridas em sextas e domingos.

# 13. Matriz de Experimentos: Mercados Iguais vs. Diferentes

Para validar a eficácia da rede em capturar o risco geopolítico de Ormuz, a arquitetura foi dividida em um **Duelo de Cenários**. O objetivo é descobrir se a rede aprende melhor quando os ativos estão sob a mesma regra de calendário ou quando precisam lidar com o "delay" global.

### **Distribuição das 8 Redes Neurais**

| Mercado | Tipo de Cenário | Tickers (Exemplo) | Desafio Técnico da Rede |
| :--- | :--- | :--- | :--- |
| **PETRÓLEO** | Mercados Diferentes | `2222.SR` + `TTE` | Lidar com o fuso Riade/Paris e o impacto do domingo. |
| **PETRÓLEO** | Mercados Iguais | `XOM` + `CVX` | Capturar a correlação pura na NYSE (Petróleo Americano). |
| **METAIS** | Mercados Diferentes | `1211.SR` + `RIO` | Analisar o Aço Chinês/Saudita vs. Minério Global. |
| **METAIS** | Mercados Iguais | `FCX` + `RIO` | Comparar Cobre vs. Ferro (Ambos sob o calendário NYSE). |

### 🎯 Por que essa divisão é genial?

1. **Isolamento de Variáveis:** Nas redes de "Mercados Iguais", o modelo foca 100% na correlação de preços. Nas de "Mercados Diferentes", o modelo é forçado a aprender a **interdependência temporal**.
2. **Benchmark de Robustez:** Se a performance nos "Mercados Diferentes" for próxima aos "Iguais", provamos que o tratamento de dados (**ffill**) e a memória da **LSTM/GRU** são capazes de neutralizar o caos dos fusos horários.
3. **Visão Setorial:** Cobrimos os dois pilares que sustentam a economia global através de Ormuz: Energia (Petróleo) e Infraestrutura (Metais).

##  13.1. Bloco A: Cenários de Mercados Diferentes (O Desafio de Ormuz)

Este é o coração do projeto. Aqui, as 4 redes restantes enfrentam o "Ponto Cego" dos calendários assíncronos. É onde testamos se a nossa engenharia de dados via **Forward Fill** realmente permite que a LSTM antecipe movimentos.

### **Configuração do Experimento:**
* **Petróleo (Riade/Paris):** `2222.SR` (Aramco) + `TTE` (TotalEnergies).
* **Metais (Riade/Global):** `1211.SR` (Ma'aden) + `RIO` (Rio Tinto).

> **O que a rede deve aprender:** A lidar com o "delay" de 72 horas do final de semana e com a abertura antecipada de Riade aos domingos. O objetivo é capturar a **transmissão de risco** que viaja entre o Golfo Pérsico e os centros financeiros globais.

### Aglomerado de Petróleo 

**Extração e Sincronização (Petróleo - Mercados Diferentes)**

# --- FLUXO 1: AGEROMERADO DE PETRÓLEO (MERCADOS DIFERENTES) ---
tickers_1 = ['2222.SR', 'TTE']
dfs_1 = []

for t in tickers_1:
    # 1. Download Seguro (auto_adjust=False para manter Close/Adj Close originais)
    df_raw = yf.download(t, start='2019-01-01', end='2026-03-22', progress=False, auto_adjust=False)
    df = df_raw.copy()

    # 2. Limpeza de MultiIndex (Garante compatibilidade se houver mais de um nível nas colunas)
    if isinstance(df.columns, pd.MultiIndex):
        df.columns = df.columns.get_level_values(0)

    # 3. Seleção de Coluna e Limpeza de Duplicatas
    # Usamos Adj Close se disponível, senão Close.
    col_to_use = 'Adj Close' if 'Adj Close' in df.columns else 'Close'

    # Criamos o DataFrame focado na coluna alvo e removemos colunas duplicadas acidentais
    df = df[[col_to_use]].copy()
    df.columns = [f'{t}_Close']
    df = df.loc[:, ~df.columns.duplicated()]

    # 4. Adição de Indicadores (SMA, EMA, RSI)
    # Importante: O cálculo ocorre ANTES da concatenação para evitar interferência entre ativos
    df = add_indicators(df, col=f'{t}_Close', window=14)
    dfs_1.append(df)

# 5. CONCATENAÇÃO, ALINHAMENTO E LIMPEZA
# ffill(): Preenche feriados/fins de semana com o último preço disponível
# dropna(): Remove as primeiras 14 linhas (onde os indicadores são NaN)
data_petro_dif = pd.concat(dfs_1, axis=1).ffill().dropna()

# 6. MAPEAMENTO DINÂMICO DOS ALVOS (Target Indices)
# Identifica em quais colunas estão os preços de fechamento (serão as saídas 'y' da rede)
target_cols_1 = [col for col in data_petro_dif.columns if '_Close' in col]
target_indices_1 = [data_petro_dif.columns.get_loc(c) for c in target_cols_1]

print(f"✓ Fluxo 1 Concluído: {data_petro_dif.shape[0]} linhas e {data_petro_dif.shape[1]} colunas.")
print(f"Índices das Colunas Alvo: {target_indices_1} (Nomes: {target_cols_1})")

**Normalização Técnica (Escalonamento Min-Max)**

- Ele é crucial porque "achata" as escalas de preços (que podem estar em dezenas ou centenas) para o intervalo $[0, 1]$, facilitando a convergência matemática do otimizador da rede neural.

# --- NORMALIZAÇÃO: FLUXO 1 (PETRÓLEO DIFERENTE) ---

# 1. Isolamento e Cópia
df_para_escala_1 = data_petro_dif.copy()

# 2. Scaler com Nome Único (O "tradutor" exclusivo deste fluxo)
scaler_petro_dif = MinMaxScaler()

# 3. Ajuste e Transformação
# O scaler aprende o min/max de cada uma das 8 colunas (Preços e Indicadores)
scaled_petro_dif = scaler_petro_dif.fit_transform(df_para_escala_1)

# 4. Diagnóstico de Segurança
print(f"=== Diagnóstico de Escala: Fluxo 1 (Petróleo) ===")
print(f"✓ Shape do Array Escalado: {scaled_petro_dif.shape}")
print(f"✓ Colunas Alvo (Y) neste fluxo: {target_indices_1}")
print(f"✓ Valor Máximo Escalado: {scaled_petro_dif.max():.2f} | Mínimo: {scaled_petro_dif.min():.2f}")
print("-" * 60)

**Engenharia de Janelamento Temporal (Sliding Window)**
- Esta função é o coração do aprendizado temporal: ela transforma uma tabela estática em um formato "3D" (Amostras, Tempo, Variáveis) que permite à rede neural enxergar o movimento dos preços ao longo de 60 dias antes de tomar uma decisão.

# --- BLOCO ESSENCIAL: DEFINIÇÃO DA FUNÇÃO DE SEQUENCIAMENTO ---

def create_multivariate_sequences(data, seq_len, target_indices):
    """
    Transforma o array plano em janelas temporais (3D) para a LSTM.
    data: O array escalado (0-1)
    seq_len: Tamanho da memória (ex: 60 dias)
    target_indices: Quais colunas queremos prever (ex: [0, 4])
    """
    X, y = [], []
    for i in range(seq_len, len(data)):
        # Pega a janela do passado (60 dias)
        # X shape: (60, 8) -> 60 dias, 8 colunas de dados
        X.append(data[i-seq_len:i])

        # Pega os preços reais de HOJE para os ativos alvo
        # y shape: (2,) -> Preço da Aramco e da Total no dia i
        y.append(data[i, target_indices])

    return np.array(X), np.array(y)

**Janelamento e Separação de Dados (Treino vs. Teste)**
- Aplicação da função de janelamento especificamente aos dados de Petróleo e realiza a divisão cronológica. Em séries temporais, nunca usamos train_test_split aleatório, pois precisamos que o modelo aprenda o passado para prever o futuro.

# --- APLICAÇÃO DA JANELA TEMPORAL: FLUXO 1 (PETRÓLEO) ---

# 1. Configuração da janela (60 dias de histórico)
seq_len = 60

# 2. Criação das sequências usando as variáveis exclusivas do Fluxo 1
X1, y1 = create_multivariate_sequences(scaled_petro_dif, seq_len, target_indices_1)

# 3. Divisão Treino/Teste Cronológica (80/20)
split_1 = int(0.8 * len(X1))

X1_train, X1_test = X1[:split_1], X1[split_1:]
y1_train, y1_test = y1[:split_1], y1[split_1:]

# 4. Verificação Final de Dimensões
print(f"=== Dimensões Finais: Fluxo 1 (Petróleo) ===")
print(f"✓ X1_train: {X1_train.shape} (Amostras, Dias, Features)")
print(f"✓ y1_train: {y1_train.shape} (Amostras, Ativos Alvo)")
print(f"✓ Data de início do Teste: {data_petro_dif.index[split_1 + seq_len].date()}")
print("-" * 60)

**Processamento e Mapeamento de Sequências**
- Note que ele consolida o processamento das sequências do Fluxo 1, garantindo que o mapeamento das colunas alvo esteja correto antes de enviarmos os dados para a arquitetura de Tensores do PyTorch.

# --- FLUXO 1: PROCESSAMENTO DE SEQUÊNCIAS ---

# 1. MAPEAMENTO DE ALVOS
# Identifica as colunas de fechamento para os 2 ativos
target_cols_p_dif = [col for col in data_petro_dif.columns if 'close' in col.lower()]
targets_petro_dif = [data_petro_dif.columns.get_loc(c) for c in target_cols_p_dif]

# 2. CONFIGURAÇÃO DA JANELA (60 dias de memória)
seq_len = 60
X1, y1 = create_multivariate_sequences(scaled_petro_dif, seq_len, targets_petro_dif)

# 3. DIVISÃO TREINO/TESTE (80/20 Cronológica)
split = int(0.8 * len(X1))
X1_train, X1_test = X1[:split], X1[split:]
y1_train, y1_test = y1[:split], y1[split:]

# --- VERIFICAÇÃO DE SEGURANÇA ---
print("=== Verificação de Dimensões (Fluxo 1: Petróleo) ===")
print(f"✓ Entrada (X1_train): {X1_train.shape} -> [Janelas, Dias, Features]")
print(f"✓ Saída (y1_train): {y1_train.shape} -> [Janelas, Ativos]")
print("-" * 60)

**Classe Dataset (Ponte PyTorch)**
- Aqui definimos a estrutura que o PyTorch exige para ler os dados. Transformamos seus arrays NumPy em Tensores, que são os objetos matemáticos que a GPU consegue processar para treinar a rede neural.

class TimeSeriesDataset(Dataset):
    def __init__(self, X, y):
        self.X = torch.tensor(X, dtype=torch.float32)
        self.y = torch.tensor(y, dtype=torch.float32)
    def __len__(self):
        return len(self.X)
    def __getitem__(self, idx):
        return self.X[idx], self.y[idx]

**Instanciação dos DataLoaders (Gerenciamento de Lotes)**
- Os DataLoaders são os "Orquestradores de Fluxo" da rede neural: eles organizam os dados em pequenos grupos (batches) para que a GPU processe a informação de forma eficiente, sem sobrecarregar a memória e melhorando a estabilidade do aprendizado.

# --- INSTANCIAÇÃO DOS DATALOADERS (FLUXO 1) ---

# 1. Criar os conjuntos de dados PyTorch
train_ds1 = TimeSeriesDataset(X1_train, y1_train)
test_ds1 = TimeSeriesDataset(X1_test, y1_test)

# 2. Criar os DataLoaders (Gerenciadores de Lotes)
# batch_size=32: O modelo verá 32 exemplos de 60 dias antes de ajustar os pesos
# shuffle=True no treino: Impede que a rede decore a ordem cronológica
train_loader1 = DataLoader(train_ds1, batch_size=32, shuffle=True)
test_loader1 = DataLoader(test_ds1, batch_size=32)

print(f"✓ DataLoaders do Fluxo 1 configurados com sucesso!")
print(f"✓ Total de lotes para treino: {len(train_loader1)}")

**Visualização de Alvos e Auditoria de Escala**
- É a fase de Auditoria Visual. Antes de treinar a rede, precisamos garantir que os alvos (preços) estão corretamente normalizados e que o "alinhamento" entre a Saudi Aramco e a TotalEnergies faz sentido matemático.

# --- VISUALIZAÇÃO DOS ALVOS (FLUXO 1: PETRÓLEO) ---

tickers_label = ['Saudi Aramco (2222.SR)', 'TotalEnergies (TTE)']
colors = ['forestgreen', 'royalblue']

# Criamos a figura com 2 subplots
fig, axs = plt.subplots(1, 2, figsize=(15, 6))
fig.suptitle('Distribuição dos Alvos de Petróleo - 100 dias (y1_train Normalizado)', fontsize=16)

# IMPORTANTE: Usamos y1_train (específico do Fluxo 1)
for i in range(len(tickers_label)):
    ax = axs[i]
    # Plota as primeiras 100 amostras de cada coluna do y1_train
    ax.plot(y1_train[:100, i], color=colors[i], label='Normalizado', linewidth=2)
    ax.set_title(f'Ativo: {tickers_label[i]}')
    ax.set_xlabel('Amostra (Dias)')
    ax.set_ylabel('Valor (0-1)')
    ax.grid(True, alpha=0.3)
    ax.legend(loc='upper right')

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# Print para conferência técnica (Validação dos 2 alvos do Fluxo 1)
print("=== Conferência Técnica: Aglomerado Petróleo (Fluxo 1) ===")
for i, ticker in enumerate(tickers_label):
    # Verificação estatística para garantir que o MinMaxScaler funcionou (deve estar entre 0 e 1)
    print(f"{ticker}: min={y1_train[:, i].min():.4f}, max={y1_train[:, i].max():.4f}, média={y1_train[:, i].mean():.4f}")

**Configuração do Motor de Treinamento (LSTM + GRU)**

Nesta etapa, definimos as diretrizes matemáticas que o modelo seguirá para aprender. Escolhemos o otimizador **Adam**, amplamente reconhecido por sua eficiência em convergir em problemas de séries temporais complexas.

 **Componentes da Configuração:**
1.  **Input Size Dinâmico:** O modelo detecta automaticamente o número de colunas (8 no total: Preço + 3 indicadores para cada um dos 2 ativos).
2.  **Hardware Acceleration (GPU):** O código verifica se há uma placa de vídeo disponível (`cuda`) para acelerar o cálculo dos gradientes.
3.  **Loss Function (MSE):** Utilizamos o Erro Quadrático Médio, que penaliza severamente erros grandes, forçando o modelo a ser mais preciso.

# --- ARQUITETURA DO MODELO: FLUXO 1 (PETRÓLEO) ---

class LSTM_GRU_Model(nn.Module):
    def __init__(self, input_size, hidden_lstm=64, hidden_gru=32, output_size=2):
        super().__init__()

        # 1. Camada LSTM: Foco em memória de longo prazo
        self.lstm1 = nn.LSTM(input_size=input_size,
                            hidden_size=hidden_lstm,
                            batch_first=True)

        # 2. Camada GRU: Foco em padrões recentes e eficiência
        self.gru = nn.GRU(input_size=hidden_lstm,
                         hidden_size=hidden_gru,
                         batch_first=True)

        # 3. Dropout (Opcional): Previne que a rede decore o ruído do mercado
        self.dropout = nn.Dropout(0.2)

        # 4. Camada Linear de Saída: Transforma os neurônios em 2 preços (Aramco e Total)
        self.fc = nn.Linear(hidden_gru, output_size)

    def forward(self, x):
        # x shape: [batch, seq_len, input_size]

        # Passa pela LSTM
        out_lstm, _ = self.lstm1(x)

        # Passa pela GRU (entrada é a saída da LSTM)
        out_gru, _ = self.gru(out_lstm)

        # Captura apenas o estado final da sequência (o "resumo" dos 60 dias)
        last_step = out_gru[:, -1, :]

        # Aplica dropout e gera a predição final
        final_output = self.fc(self.dropout(last_step))

        return final_output

print("✓ Classe LSTM_GRU_Model definida para saída multivariada (2 ativos).")

**Setup Técnico do Motor Neural**

Nesta etapa, preparamos o ambiente de execução. O diferencial aqui é o **Mapeamento Dinâmico**: o modelo não é rígido; ele identifica sozinho quantas variáveis (features) existem no aglomerado de petróleo para configurar sua camada de entrada.

**Destaques da Configuração:**
* **MSE (Mean Squared Error):** Escolhido como "juiz" do modelo. Como estamos lidando com preços de commodities sensíveis, o MSE penaliza erros maiores com mais intensidade, forçando a rede a buscar uma precisão cirúrgica.
* **Otimizador Adam:** Atua como o "instrutor" da rede, ajustando os pesos de forma adaptativa. É ideal para o mercado de petróleo, pois lida bem com dados ruidosos e voláteis.

# --- INICIALIZAÇÃO DO MODELO: FLUXO 1 (PETRÓLEO) ---

# 1. Detectar o número de colunas (features) automaticamente do FLUXO 1
# Esperado: 8 (2 ativos * [Close, SMA, EMA, RSI])
input_size_1 = X1_train.shape[2]

# 2. Definir o dispositivo (GPU ou CPU)
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")

# 3. Inicializar o Modelo Híbrido específico para Petróleo
# output_size=2 porque prevemos Aramco e Total simultaneamente
model_petro = LSTM_GRU_Model(input_size=input_size_1, output_size=2).to(device)

# 4. Função de Perda (MSE para Regressão)
criterion_petro = nn.MSELoss()

# 5. Otimizador (Adam) - focado nos parâmetros do model_petro
optimizer_petro = torch.optim.Adam(model_petro.parameters(), lr=0.001)

print(f"=== Configuração do Modelo (Fluxo 1) ===")
print(f"✓ Dispositivo: {device}")
print(f"✓ Input Size: {input_size_1} | Output Size: 2")
print(f"✓ Modelo pronto para o Aglomerado de Petróleo.")
print("-" * 60)

**Loop de Treinamento e Monitoramento de Convergência**

Chegamos à fase onde a rede neural "estuda" os dados de petróleo. O processo é dividido em duas fases repetidas por 50 ciclos (épocas):
1.  **Fase de Treino:** O modelo tenta prever os preços e ajusta seus pesos internos via *Backpropagation* a cada erro.
2.  **Fase de Validação:** O modelo é testado em dados que ele nunca viu. Se o erro de validação começar a subir enquanto o de treino cai, o sistema detecta o Overfitting.

**Mecânica de Checkpoint:**

O código utiliza `deepcopy` para salvar o estado da rede no exato momento em que ela atinge o **menor erro de validação**. Isso garante que, ao final das 50 épocas, teremos a "versão de ouro" do modelo, e não apenas o resultado da última rodada.

# --- LOOP DE TREINAMENTO: FLUXO 1 (PETRÓLEO) - IMPRESSÃO 1 EM 1 ---

from copy import deepcopy

# 1. Reset de métricas para este fluxo específico (Fluxo 1)
best_val_loss_1 = float('inf')
best_model_state_1 = None
train_losses_1, val_losses_1 = [], []

print(f"Iniciando Treinamento: Fluxo 1 (Petróleo)")
print(f"Device: {device} | Ativos: Saudi Aramco e TotalEnergies")
print("-" * 60)

for epoch in range(1, 51):
    # --- FASE DE TREINO ---
    model_petro.train()
    batch_losses = []

    for xb, yb in train_loader1: # Loader específico do Fluxo 1
        xb, yb = xb.to(device), yb.to(device)

        optimizer_petro.zero_grad()
        preds = model_petro(xb)
        loss = criterion_petro(preds, yb)

        loss.backward()
        optimizer_petro.step()
        batch_losses.append(loss.item())

    train_loss = np.mean(batch_losses)

    # --- FASE DE VALIDAÇÃO ---
    model_petro.eval()
    val_batch_losses = []
    with torch.no_grad():
        for xb, yb in test_loader1: # Loader específico do Fluxo 1
            xb, yb = xb.to(device), yb.to(device)
            preds = model_petro(xb)
            v_loss = criterion_petro(preds, yb)
            val_batch_losses.append(v_loss.item())

    val_loss = np.mean(val_batch_losses)
    train_losses_1.append(train_loss)
    val_losses_1.append(val_loss)

    # --- IMPRESSÃO ÉPOCA POR ÉPOCA (1 EM 1) ---
    print(f"Epoch {epoch:02d}/50 | Train Loss: {train_loss:.6f} | Val Loss: {val_loss:.6f}")

    # 2. Salvar o Melhor Checkpoint (Menor Val Loss)
    if val_loss < best_val_loss_1:
        best_val_loss_1 = val_loss
        best_model_state_1 = deepcopy(model_petro.state_dict())

# 3. Restaurar o melhor modelo após o fim das 50 épocas
if best_model_state_1:
    model_petro.load_state_dict(best_model_state_1)
    print("-" * 60)
    print(f"Treinamento Concluído! Melhor Val Loss (Petróleo): {best_val_loss_1:.6f}")

# Plot das curvas de aprendizado
plt.figure(figsize=(10, 4))
plt.plot(train_losses_1, label='Erro de Treino', color='forestgreen')
plt.plot(val_losses_1, label='Erro de Validação', linestyle='--', color='royalblue')
plt.title('Curvas de Aprendizado - Setor de Petróleo (Fluxo 1)', fontsize=12)
plt.xlabel('Época')
plt.ylabel('MSE Loss')
plt.legend()
plt.grid(True, alpha=0.3)
plt.show()

**OBS:** Se a linha azul (Validação) estiver próxima da verde (Treino), sua rede aprendeu as correlações geopolíticas com sucesso. Se a azul subir demais, a rede está tentando "decorar" o mercado.

**Avaliação Multivariada: Real vs. Previsto**

Nesta etapa, validamos o desempenho preditivo do modelo híbrido. O diferencial aqui é a **reconstrução da escala original**. Como a rede operou em um espaço matemático entre 0 e 1, precisamos "traduzir" esses sinais de volta para as moedas correspondentes de cada mercado.

**Destaques da Implementação:**
1.  **Modo de Avaliação (`.eval()`):** Desativa o Dropout para garantir que a rede use todo o seu potencial aprendido.
2.  **Inversão de Escala de Precisão:** A função reconstrói a matriz original de 8 colunas para garantir que a desnormalização do `MinMaxScaler` seja matematicamente exata.
3.  **Visualização Comparativa:** Plotamos o "Gabarito" (Real) contra a "Aposta" (Previsto) para medir visualmente a aderência da curva.

- Chegamos ao momento da verdade: a Inferência e Desnormalização. Aqui, pedimos para a rede neural "olhar" para os dados de teste (que ela nunca viu no treino) e projetar os preços.

- O ponto técnico mais crítico aqui é a função get_inverse_prices. Como o Scaler foi treinado com 8 colunas (preços + indicadores), precisamos criar uma "matriz dummy" para reverter a escala corretamente e obter os valores reais em Riyal Saudita (SAR) e Euro (EUR).

# --- AVALIAÇÃO MULTIVARIADA: REAL VS PREVISTO (FLUXO 1: PETRÓLEO) ---

model_petro.eval()
all_preds_1 = []
all_actuals_1 = []

with torch.no_grad():
    for xb, yb in test_loader1: # Loader específico do Fluxo 1
        xb = xb.to(device)
        out = model_petro(xb) # Gera as 2 predições simultâneas
        all_preds_1.append(out.cpu().numpy())
        all_actuals_1.append(yb.numpy())

# Transformar listas em arrays numpy
preds_scaled_1 = np.concatenate(all_preds_1, axis=0)
actuals_scaled_1 = np.concatenate(all_actuals_1, axis=0)

# --- FUNÇÃO DE DESNORMALIZAÇÃO (Ajustada para o Scaler do Fluxo 1) ---
def get_inverse_prices(scaled_data, scaler_obj, target_indices):
    # Criamos uma matriz vazia com o mesmo número de colunas original (ex: 8)
    dummy = np.zeros((len(scaled_data), scaler_obj.n_features_in_))

    # Preenchemos apenas as colunas que correspondem aos preços de fechamento
    for i, idx in enumerate(target_indices):
        dummy[:, idx] = scaled_data[:, i]

    # Invertemos a escala para voltar aos valores em SAR e EUR
    inverse = scaler_obj.inverse_transform(dummy)

    # Retornamos apenas as colunas desnormalizadas dos ativos
    return [inverse[:, idx] for idx in target_indices]

# Obter preços finais (Desnormalizados) usando os objetos do Fluxo 1
# Note que passamos scaler_petro_dif e targets_petro_dif
preds_final_1 = get_inverse_prices(preds_scaled_1, scaler_petro_dif, targets_petro_dif)
actuals_final_1 = get_inverse_prices(actuals_scaled_1, scaler_petro_dif, targets_petro_dif)

# --- PLOTAGEM DOS 2 GRÁFICOS LADO A LADO ---
tickers_label = ['Saudi Aramco (2222.SR)', 'TotalEnergies (TTE)']
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Avaliação Fluxo 1: Preço Real vs. Previsto (SAR e EUR)', fontsize=18)

for i in range(len(tickers_label)):
    ax = axs[i]
    # Plotamos o Real vs Previsto para cada ativo
    ax.plot(actuals_final_1[i], label='Real (Histórico)', color='forestgreen', linewidth=1.5)
    ax.plot(preds_final_1[i], label='Previsto (LSTM+GRU)', color='darkorange', linestyle='--', linewidth=1.5)

    ax.set_title(f'Ativo: {tickers_label[i]}', fontsize=14)
    ax.set_ylabel('Preço de Fechamento')
    ax.set_xlabel('Dias (Conjunto de Teste)')
    ax.legend()
    ax.grid(True, alpha=0.3)

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

**Diagnóstico de Saída: Integridade do Espaço Latente**

Este bloco realiza uma autópsia estatística nas predições puras da rede. O objetivo é garantir que o modelo não está apenas chutando a média, mas sim replicando a dinâmica de volatilidade do setor de petróleo.

#### **O que estamos validando aqui?**
* **Amplitude de Resposta:** Se a saída varia entre o Min e o Max de forma fluida, o modelo captou a "assinatura" do preço.
* **Ausência de Saturação:** Verificamos se os valores não estão "batendo no teto" (1.0) ou "no chão" (0.0), o que indicaria problemas na função de ativação final.
* **Sensibilidade Individual:** Confirmamos que a Aramco e a TotalEnergies possuem comportamentos distintos dentro da mesma rede.

Ele serve como uma Auditoria de Sanidade da Rede. Antes de confiar nos preços finais, olhamos para a "caixa preta" do modelo (os valores entre 0 e 1). Se o gráfico mostrar uma linha reta ou valores travados em 0 ou 1, saberíamos que a rede sofreu um colapso de gradiente.

# --- DIAGNÓSTICO DE SAÍDA: FLUXO 1 (PETRÓLEO) (SEM MÉDIA NO GRÁFICO) ---

tickers_label = ['Saudi Aramco (2222.SR)', 'TotalEnergies (TTE)']
colors = ['forestgreen', 'royalblue']

# Criamos a figura com 2 subplots (1x2)
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Diagnóstico Fluxo 1: Saída da Rede (Valores 0-1)', fontsize=16)

# IMPORTANTE: Usamos preds_scaled_1 (criado no bloco anterior de avaliação)
print("=== Relatório de Diagnóstico de Saída (Fluxo 1) ===")

for i in range(len(tickers_label)):
    ax = axs[i]

    # Plotamos as primeiras 100 predições do ativo i para ver a variação
    ax.plot(preds_scaled_1[:100, i], color=colors[i], label=f'Pred {tickers_label[i]}', linewidth=2)

    # Cálculo das métricas estatísticas da saída normalizada (mantido no relatório texto)
    p_mean = preds_scaled_1[:, i].mean()
    p_min, p_max = preds_scaled_1[:, i].min(), preds_scaled_1[:, i].max()

    # Configurações do eixo
    ax.set_title(f'Ativo: {tickers_label[i]}')
    ax.set_ylabel('Valor Normalizado (Saída do Modelo)')
    ax.set_xlabel('Amostra (Dias no Conjunto de Teste)')
    ax.grid(True, alpha=0.3)
    ax.legend(loc='upper right')

    # Print individual de diagnóstico técnico
    print(f"✓ {tickers_label[i]} -> Min: {p_min:.4f} | Max: {p_max:.4f} | Média: {p_mean:.4f}")

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

**Projeção de Tendência: Próximos 5 Dias Úteis**

Este bloco executa a **inferência recursiva**. O modelo utiliza a última janela real de 60 dias para projetar uma semana útil de mercado (5 dias). É o teste final da lógica de correlação entre a Saudi Aramco e a TotalEnergies.

#### **Destaques da Lógica de Projeção:**
1.  **Semente de Dados:** Capturamos o `tail(60)` do DataFrame original para garantir que a previsão parta do preço de fechamento mais recente.
2.  **Atualização de Vetor (Feedback Loop):** A cada passo, injetamos o preço previsto no vetor de entrada, "empurrando" a janela temporal para a frente.
3.  **Visualização com Anotação:** O gráfico inclui os valores exatos (`ax.annotate`) para facilitar a tomada de decisão ou análise de variação percentual esperada.

- Entramos na fase de Projeção Preditiva (Forecasting). Aqui o modelo para de olhar para o passado e tenta "desenhar" o futuro.

- O ponto técnico mais sofisticado aqui é a Recursão por Janela Deslizante (Sliding Window): a rede usa a sua própria previsão do "Dia +1" como dado de entrada para calcular o "Dia +2", e assim por diante. Isso demonstra a capacidade da LSTM/GRU de manter o estado da tendência.

# --- PREVISÃO FUTURA (5 DIAS): FLUXO 1 (PETRÓLEO) ---

model_petro.eval()
n_future = 5  # Projeção para a próxima semana útil
tickers_label = ['Saudi Aramco (2222.SR)', 'TotalEnergies (TTE)']
moedas = ['SAR', 'EUR']

# 1. Capturar a última janela real de 60 dias do dataframe de PETRÓLEO
last_sequence_raw = data_petro_dif.tail(seq_len).values
# Usamos o scaler específico do fluxo 1
last_scaled = scaler_petro_dif.transform(last_sequence_raw)

# Preparar o tensor inicial [1, 60, 8]
current_input = torch.tensor(last_scaled, dtype=torch.float32).unsqueeze(0).to(device)

future_preds_scaled = []

for _ in range(n_future):
    with torch.no_grad():
        # O modelo gera 2 saídas normalizadas simultâneas
        next_pred = model_petro(current_input)
        pred_vals = next_pred.cpu().numpy()[0]
        future_preds_scaled.append(pred_vals)

    # 2. Atualizar a sequência (Recursão)
    # Pegamos o vetor do último dia na janela
    new_entry = current_input[0, -1, :].cpu().numpy().copy()

    # Atualizamos apenas os preços de fechamento (Aramco e Total)
    # Nota: Indicadores (RSI, SMA) ficam constantes nesta simplificação
    for i, idx in enumerate(targets_petro_dif):
        new_entry[idx] = pred_vals[i]

    # 3. Deslocar a janela (Sliding Window)
    new_entry_tensor = torch.tensor(new_entry, dtype=torch.float32).view(1, 1, -1).to(device)
    current_input = torch.cat([current_input[:, 1:, :], new_entry_tensor], dim=1)

# --- DESNORMALIZAÇÃO ---
future_preds_scaled = np.array(future_preds_scaled)

def denormalize_projection(scaled_data, scaler_obj, target_indices):
    dummy = np.zeros((len(scaled_data), scaler_obj.n_features_in_))
    for i, idx in enumerate(target_indices):
        dummy[:, idx] = scaled_data[:, i]
    inv = scaler_obj.inverse_transform(dummy)
    return inv[:, target_indices]

future_prices = denormalize_projection(future_preds_scaled, scaler_petro_dif, targets_petro_dif)

# --- PLOTAGEM DOS GRÁFICOS ---
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle(f'Fluxo 1: Projeção de Petróleo para os Próximos {n_future} Dias', fontsize=18)

dias_futuros = range(1, n_future + 1)
colors_plot = ['forestgreen', 'royalblue']

for i in range(len(tickers_label)):
    ax = axs[i]
    ax.plot(dias_futuros, future_prices[:, i], marker='o', color=colors_plot[i],
            linestyle='--', linewidth=2, markersize=8)

    ax.set_title(f'Ativo: {tickers_label[i]}', fontsize=14)
    ax.set_ylabel(f'Preço Estimado ({moedas[i]})')
    ax.set_xlabel('Dias úteis à frente')
    ax.set_xticks(dias_futuros)
    ax.grid(True, alpha=0.3)

    for x, y in zip(dias_futuros, future_prices[:, i]):
        ax.annotate(f'{y:.2f}', (x, y), textcoords="offset points",
                    xytext=(0,12), ha='center', fontweight='bold', color=colors_plot[i])

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# --- TABELA RESUMO ---
print(f"\n--- Tabela de Previsões: Fluxo 1 ({n_future} dias) ---")
df_resumo = pd.DataFrame(future_prices, columns=tickers_label,
                         index=[f"Dia +{i+1}" for i in range(n_future)])
print(df_resumo.round(3))

**Persistência de Resultados: Setor de Petróleo**

Para garantir a integridade dos dados na etapa de comparação final (onde analisaremos todos os aglomerados simultaneamente), realizamos o backup dos resultados desnormalizados. Isso evita que o treinamento do próximo fluxo limpe a memória do que foi conquistado aqui.

**Por que o `.copy()` é essencial?**

No Python, se você apenas igualar as variáveis (`a = b`), você cria um ponteiro (referência). Se o valor de `b` mudar no próximo bloco, `a` também mudará. O método `.copy()` garante que os dados da Saudi Aramco e TotalEnergies sejam salvos em um novo espaço de memória, protegendo o seu histórico.

- Este passo é uma medida de Segurança de Memória e Persistência. Como o projeto lida com 17 blocos e múltiplos fluxos (Petróleo, Tecnologia, etc.), é vital "congelar" os resultados do Fluxo 1 em variáveis exclusivas antes que as variáveis genéricas (preds_final, actuals_final) sejam sobrescritas pelos próximos processamentos.

# --- SALVAMENTO ESPECÍFICO DO SETOR (PETRÓLEO - FLUXO 1) ---

# No seu código anterior, o resultado final está em 'future_prices'
# Criamos uma cópia real para evitar que a variável seja sobrescrita
preds_final_petro = future_prices.copy()

# Se você também quiser salvar os dados de validação do passado (se houver):
# actuals_final_petro = actuals_final.copy() # (Opcional, se existir no seu script)

print("✓ Backup de memória concluído: Projeção de Petróleo (future_prices) preservada.")

**Blindagem de Variáveis: Finalização do Setor de Petróleo**

Nesta etapa, realizamos o "congelamento" dos dados processados. Em Python, variáveis dentro de loops ou fluxos repetitivos tendem a ser sobrescritas. Ao criar nomes como `_fixed`, você garante que o seu Dashboard final consiga acessar os dados de Petróleo sem interferência dos próximos setores que serão treinados.

**Por que isso é crítico para o seu Colab?**
1.  **Imutabilidade:** O `preds_petro_fixed` não será alterado quando você rodar o "Fluxo 2".
2.  **Preparação para Correlação:** Com esses dados salvos separadamente, você poderá criar um gráfico final comparando, por exemplo, como o Petróleo (Aramco) se comportou em relação à Tecnologia (Apple/Nvidia) no mesmo período.

# --- FINALIZAÇÃO E SALVAMENTO DE VARIÁVEIS DE CONTROLE ---

# 'preds_petro_fixed' agora contém a projeção de 5 dias da Aramco e Total
preds_petro_fixed = future_prices.copy()

print("-" * 60)
print("SETOR DE PETRÓLEO (FLUXO 1) CONCLUÍDO E BLINDADO")
print("Dados prontos para correlação em: 'preds_petro_fixed'")
print("-" * 60)

### Aglomerado de Metais

**Coleta e Tratamento (Fluxo 2: Metais)**
- Nesta etapa, replicamos a robustez do tratamento de dados para o novo setor. O destaque vai para o Tratamento de MultiIndex, essencial para lidar com as mudanças recentes na API do yfinance, garantindo que apenas os preços de fechamento limpos entrem no pipeline.

# --- COLETA E TRATAMENTO: FLUXO 2 (METAIS) ---

tickers_metais = ['1211.SR', 'RIO']
dfs_metais = []

for t in tickers_metais:
    # Coleta de dados até a data atual de 2026
    df_raw = yf.download(t, start='2019-01-01', end='2026-03-22', progress=False)

    if df_raw.empty:
        print(f"Erro: Dados não encontrados para {t}")
        continue

    # Tratamento de MultiIndex (Padrão yfinance recente)
    if isinstance(df_raw.columns, pd.MultiIndex):
        df = df_raw.xs('Close', axis=1, level=0).copy()
        if t in df.columns:
            df = df[[t]]
    else:
        df = df_raw[['Close']].copy()

    # Nomeação única para evitar conflitos na concatenação
    col_name = f'{t}_Close'
    df.columns = [col_name]

    # Aplicação dos indicadores (SMA, EMA, RSI)
    df = add_indicators(df, col=col_name, window=14)
    dfs_metais.append(df)

# Concatenagem e Limpeza Específica do Fluxo 2
data_metais = pd.concat(dfs_metais, axis=1).ffill().dropna()

# Mapeamento de colunas alvo para o Fluxo 2
target_cols_metais = [col for col in data_metais.columns if 'close' in col.lower()]
target_indices_metais = [data_metais.columns.get_loc(c) for c in target_cols_metais]

print(f"=== Diagnóstico Fluxo 2: Metais ===")
print(f"✓ Shape final: {data_metais.shape}")
print(f"✓ Ativos detectados: {tickers_metais}")
print(f"✓ Índices das colunas Alvo: {target_indices_metais}")
print("-" * 60)
data_metais.tail()

**Normalização Específica (Fluxo 2: Metais)**
- Neste estágio, garantimos que todos os indicadores (RSI, SMA, EMA) e preços de fechamento do setor de mineração e metais estejam na mesma "língua" matemática (intervalo de 0 a 1).
- Aqui aplicamos o **Isolamento de Escal**a.
- É um passo crítico: as ações da **Ma'aden** (**1211.SR**) costumam cotar na casa dos **40-50 SAR**, enquanto a **Rio Tint**o (**RIO**) em Nova York pode estar na casa dos **60-70 USD**. Sem este `MinMaxScaler` exclusivo, a rede neural poderia dar um peso desproporcional ao ativo com o valor nominal mais alto, ignorando as variações percentuais do mais barato.

# 1. Criamos o Scaler exclusivo para o Aglomerado de Metais
scaler_metais_dif = MinMaxScaler()

# 2. Ajuste e Transformação usando o DataFrame específico de Metais
# IMPORTANTE: Garante que os preços da Ma'aden e Rio Tinto não se misturem com Petróleo
scaled_metais_dif = scaler_metais_dif.fit_transform(data_metais)

**Criação de Sequências Temporais (Fluxo 2: Metais)**

Nesta etapa, aplicamos a lógica de Janela Deslizante (Sliding Window) para o setor de Metais. Esta função atua como um "tradutor" que transforma uma tabela estática em um formato tridimensional $[Amostras, Tempo, Features]$, que é o único idioma que as camadas LSTM e GRU conseguem processar com eficiência.

def create_multivariate_sequences(data, seq_len, target_indices):
    X, y = [], []

    # O loop percorre os dados a partir do tamanho da janela (ex: 60 dias)
    for i in range(seq_len, len(data)):
        # X: Janela de 'seq_len' dias com todas as features (Preços + Indicadores)
        # Pega do índice i-seq_len até i (sem incluir o i)
        X.append(data[i-seq_len:i])

        # y: Os 2 valores de fechamento no dia exato 'i'
        # target_indices agora aponta para ['1211.SR_Close', 'RIO_Close']
        y.append(data[i, target_indices])

    return np.array(X), np.array(y)

**Divisão Cronológica e Estrutura de Tensores (Fluxo 2)**

**Por que 60 dias é o "Sweet Spot" para Metais? 🔬**

Diferente de ações de tecnologia (que podem reagir em 5 ou 10 dias), o setor de mineração (**Ma'aden e Rio Tinto**) é movido por **ciclos de commoditie**s e contratos de longo prazo. Uma janela de 60 dias (~3 meses de mercado) permite que a LSTM identifique:

- Se o minério de ferro ou metais básicos estão em uma tendência de exaustão.

- A formação de suportes e resistências em ciclos de médio prazo.

- Se um novo superciclo de alta está começando, filtrando ruídos diários irrelevantes.

Diferente de problemas comuns de IA onde os dados são sorteados aleatoriamente, em finanças a ordem dos fatos é sagrada. Se você usasse shuffle=True, estaria permitindo que o modelo "olhasse o futuro" para prever o passado (Data Leakage). Ao cortar os dados em 80% para treino e os últimos 20% para teste, estamos simulando um cenário real: o modelo aprende com o histórico antigo e tenta sobreviver aos meses mais recentes do mercado de metais.

- Nesta etapa, preparamos o "set de treinamento" e o "set de exame" para o aglomerado de Metais. A estrutura resultante é um tensor tridimensional, essencial para que a LSTM entenda a evolução do preço da Ma'aden e da Rio Tinto ao longo do tempo.

# 1. Configuração da janela temporal (60 dias de histórico para prever o próximo)
seq_len = 60
# CORREÇÃO: Usando os dados normalizados de metais (scaled_metais_dif)
X, y = create_multivariate_sequences(scaled_metais_dif, seq_len, target_indices_metais)

# 2. Divisão treino/teste (Cronológica: 80% treino, 20% teste)
# IMPORTANTE: Em séries temporais, nunca use shuffle=True.
split = int(0.8 * len(X))
X_train, X_test = X[:split], X[split:]
y_train, y_test = y[:split], y[split:]

# 3. Verificação de dimensões para o Aglomerado de Metais:
print("=== Verificação de Dimensões (Aglomerado de Metais) ===")
print(f"X_train shape: {X_train.shape}") # Esperado: (Amostras, 60, 8)
print(f"y_train shape: {y_train.shape}") # Esperado: (Amostras, 2) -> Alvos: 1211.SR e RIO

# Explicação das Dimensões:
# Amostras = Total de dias menos a janela de 60
# 60 = Dias de histórico (Lookback)
# 8 = Features totais (4 indicadores da Ma'aden + 4 da Rio Tinto)

**Estruturação do Dataset (PyTorch)**

Nesta etapa, encapsulamos os arrays de Metais em um objeto Dataset. Isso permite que o PyTorch gerencie a memória de forma inteligente e prepare os dados para o DataLoader, que lidará com os lotes (batches) durante o treinamento.

O que cada método faz?

- `__init__`: Converte os dados brutos em Tensores do PyTorch e define o tipo de dado (`float32`).

- `__len__`: Informa ao algoritmo quantas janelas de 60 dias existem no total.

- `__getitem__`: O "garçom" dos dados; ele entrega uma janela específica de 60 dias e seu respectivo alvo quando solicitado pela rede.

Como estamos trabalhando com poucos ativos (2 por fluxo), o consumo de memória RAM será mínimo, permitindo um processamento extremamente veloz no Colab.

class TimeSeriesDataset(Dataset):
    def __init__(self, X, y):
        self.X = torch.tensor(X, dtype=torch.float32)
        self.y = torch.tensor(y, dtype=torch.float32)
    def __len__(self):
        return len(self.X)
    def __getitem__(self, idx):
        return self.X[idx], self.y[idx]

**Fluxo de Dados: DataLoaders (Fluxo 2: Metais)**

Nesta etapa, configuramos os **iteradores** que alimentarão a arquitetura LSTM+GRU. O `DataLoader` automatiza o processo de entrega de dados para a GPU/CPU, garantindo que o modelo receba as informações de forma organizada e eficiente.

**Por que Batch Size 32?**

Um tamanho de lote de 32 é considerado o "padrão ouro" para séries temporais financeiras de médio porte. Ele oferece um equilíbrio ideal:

- **Estabilidade:** Evita flutuações bruscas na função de perda (Loss).

- **Eficiência:** Aproveita a aceleração de hardware sem sobrecarregar a memória.

- **Generalização:** Permite que o modelo aprenda tendências comuns entre os 32 períodos simultaneamente.

# --- DATALOADERS: FLUXO 2 (METAIS) ---

# 1. Instanciando o Dataset (Usando a classe TimeSeriesDataset)
train_ds = TimeSeriesDataset(X_train, y_train)
test_ds = TimeSeriesDataset(X_test, y_test)

# 2. Configurando os Loaders
# Nota: shuffle=False para manter a integridade da série temporal
batch_size = 32
train_loader = DataLoader(train_ds, batch_size=batch_size, shuffle=False)
test_loader = DataLoader(test_ds, batch_size=batch_size)

print("=== Checkpoint: DataLoaders (Metais) ===")
print(f"✓ Batches de Treino: {len(train_loader)}")
print(f"✓ Batches de Teste: {len(test_loader)}")
print(f"✓ Cada Batch: [32 amostras, 60 dias, 8 colunas]")

**Diagnóstico de Alvos: Metais Sauditas & Globais**

Nesta etapa, validamos a distribuição estatística dos preços de fechamento que a rede tentará prever. O uso de identidades visuais específicas (Cinza Ardósia para a Ma'aden e Vermelho Óxido para a Rio Tinto) ajuda a diferenciar o comportamento dos ativos: um focado no mercado interno saudita e outro na demanda industrial global.

**Por que realizar este diagnóstico?**

- **Validação de Escala:** Confirmamos se o `MinMaxScaler` atingiu os limites teóricos (0 e 1).

- **Análise de Tendência:** Verificamos se há "ruído" excessivo ou se os dados preservam as ondas de preço originais.

- **Sincronia Temporal:** Garantimos que ambos os ativos estão alinhados no mesmo eixo de amostras, fundamental para o aprendizado multivariado.

**Nota:** Se a **Rio Tinto** apresenta mais "serrilhados" (volatilidade) que a **Ma'aden**, isso reflete a exposição direta da RIO ao mercado de commodities de Londres/NY, enquanto a Ma'aden pode ter movimentos mais estruturais ligados ao plano Vision 2030. A rede neural usará exatamente essas diferenças para ajustar as "atenções" das camadas LSTM.

# 1. Ajuste dos Tickers e Identidade Visual (Metais Sauditas & Globais)
# Ticker 1211.SR é Ma'aden (Saudi Arabian Mining Company)
tickers_label = ['Ma\'aden (1211.SR)', 'Rio Tinto (RIO)']
colors = ['#708090', '#B22222'] # Cinza ardósia e Vermelho óxido (Minério)

# 2. Criação da Visualização (2 Subplots para análise individual)
fig, axs = plt.subplots(1, 2, figsize=(15, 6))
fig.suptitle('Fluxo 2: Distribuição dos Alvos de Metais (y_train Normalizado)', fontsize=16)

# Loop pelos 2 alvos do aglomerado de metais
for i in range(len(tickers_label)):
    ax = axs[i]
    # Plota as primeiras 100 amostras para verificar a tendência inicial
    ax.plot(y_train[:100, i], color=colors[i], label='Preço Normalizado', linewidth=2.5)

    ax.set_title(f'Ativo: {tickers_label[i]}')
    ax.set_xlabel('Amostras (Sequência Temporal)')
    ax.set_ylabel('Escala (0 a 1)')
    ax.grid(True, linestyle='--', alpha=0.5)
    ax.legend(loc='upper right')

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# 3. Conferência Estatística do Aglomerado de Metais
print("=== Conferência Técnica: Fluxo 2 (Metais) ===")
for i, ticker in enumerate(tickers_label):
    p_min = y_train[:, i].min()
    p_max = y_train[:, i].max()
    p_mean = y_train[:, i].mean()

    print(f"{ticker}:")
    print(f"  > Mínimo: {p_min:.4f}")
    print(f"  > Máximo: {p_max:.4f}")
    print(f"  > Média:  {p_mean:.4f}")

    # Alerta de Sanidade: Se min=0 e max=1, a normalização está perfeita.
    if np.isclose(p_min, 0, atol=0.1) and np.isclose(p_max, 1, atol=0.1):
        print("  [OK] Escala validada (0-1).")
    print("-" * 35)

**Arquitetura Híbrida: LSTM + GRU (Fluxo 2: Metais)**

Nesta etapa, definimos a rede neural recorrente que processará os 60 dias de histórico da **Ma'aden** e da **Rio Tint**o. O modelo opera em um esquema **Many-to-One:** ele observa uma sequência longa (60 dias) para extrair uma única previsão (o fechamento do dia seguinte).

**Por que combinar LSTM e GRU?**

- **LSTM (Camada 1):** Atua como o "filtro de longo prazo". Ela decide quais informações de meses atrás ainda são relevantes para o preço de hoje.

- **GRU (Camada 2):** Atua como o "refinador". Com menos portões lógicos que a LSTM, ela converge mais rápido e foca na dinâmica recente dos sinais vindos da camada anterior.

- **Many-to-One:** Ao selecionar `out_gru[:, -1, :]`, estamos dizendo à rede: "ignore os estados intermediários e use apenas a síntese final de todo o histórico para projetar os próximos preços".

Note que a `input_size` é **8**. Isso significa que a rede está "olhando" simultaneamente para o Preço, SMA, EMA e RSI de ambos os ativos antes de tomar qualquer decisão. É uma visão 360º do setor de mineração.

class LSTM_GRU_Model(nn.Module):
    def __init__(self, input_size, hidden_lstm=64, hidden_gru=32, output_size=2):
        super().__init__()

        # 1. Camada LSTM: Identifica ciclos longos (tendências de meses)
        # input_size = 8 (Ma'aden: 4 features + Rio Tinto: 4 features)
        self.lstm = nn.LSTM(input_size=input_size,
                            hidden_size=hidden_lstm,
                            batch_first=True)

        # 2. Camada GRU: Refina o aprendizado focando na volatilidade de curto prazo
        # Recebe os 64 sinais da LSTM e condensa em 32
        self.gru = nn.GRU(input_size=hidden_lstm,
                          hidden_size=hidden_gru,
                          batch_first=True)

        # 3. Camada de Saída (Densa/Linear)
        # Transforma os 32 neurônios da GRU nas 2 previsões de preço (Aço e Minério)
        self.fc = nn.Linear(hidden_gru, output_size)

    def forward(self, x):
        # x shape: (batch, 60, 8)

        # Passagem pela LSTM
        # out_lstm shape: (batch, 60, 64)
        out_lstm, _ = self.lstm(x)

        # Passagem pela GRU
        # out_gru shape: (batch, 60, 32)
        out_gru, _ = self.gru(out_lstm)

        # Seleção do estado final (Many-to-One)
        # Pegamos o output do último dia da janela de 60 dias (índice -1)
        last_time_step = out_gru[:, -1, :]

        # Projeção final para os 2 alvos: [1211.SR_Close, RIO_Close]
        final_output = self.fc(last_time_step)

        return final_output

**Setup do Treinamento: Hardware e Hiperparâmetros (Metais)**

Nesta etapa, conectamos a arquitetura do modelo ao hardware (GPU/CPU) e definimos as regras do jogo: como o erro será medido **(MSE**) e como os pesos serão ajustados **(Adam**).

**A Estratégia dos Hiperparâmetros:**

- `input_size = 8`: O modelo "enxerga" 8 sinais simultâneos (4 da Ma'aden + 4 da Rio Tinto).

- `MSELoss`: Ao elevar o erro ao quadrado, esta função força o modelo a ser extremamente cuidadoso com grandes variações, algo vital em commodities de alta volatilidade.

- `Learning Rate (0.001)`: É o passo de aprendizado. Nem tão rápido que ignore os detalhes, nem tão lento que nunca chegue à convergência.

# 1. Detecção Automática de Features (Aglomerado de Metais)
# O input_size captura as 8 colunas (4 da Ma'aden + 4 da Rio Tinto)
input_size = X_train.shape[2]

# 2. Definição do Hardware (Aceleração por GPU/CUDA se disponível)
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")

# 3. Inicialização do Modelo Híbrido (LSTM + GRU)
# O output_size=2 garante a previsão simultânea da Ma'aden (1211.SR) e da Rio Tinto (RIO)
model = LSTM_GRU_Model(input_size=input_size, output_size=2).to(device)

# 4. Função de Perda: MSE (Mean Squared Error)
# Ideal para metais: penaliza mais forte erros grandes na previsão de preços,
# forçando a rede a não ignorar picos de volatilidade nas commodities.
criterion = nn.MSELoss()

# 5. Otimizador: Adam (Adaptive Moment Estimation)
# Taxa de aprendizado inicial de 0.001. O Adam ajusta essa taxa para cada
# peso individualmente, excelente para lidar com o "ruído" do mercado financeiro.
optimizer = torch.optim.Adam(model.parameters(), lr=0.001)

print(f" Modelo Híbrido inicializado no dispositivo: {device}")
print(f" Input Size: {input_size} | Output Size: 2")

**Execução do Treinamento e Curvas de Convergência (Metais)**

Nesta etapa, o modelo "estuda" os 60 dias de histórico da **Ma'aden** e da **Rio Tinto** repetidamente. A cada época, ele tenta reduzir o erro **(MSE**) ajustando seus pesos internos através do otimizador Adam.

**Destaques da Implementação:**

- `model.train()` vs `model.eval()`: Comandos vitais que avisam ao PyTorch quando ele deve calcular gradientes e quando deve apenas prever (economizando memória e CPU).

- **Early Saving**: O código monitora a `val_loss`. Se o erro de validação parar de cair e começar a subir, o modelo "lembrará" do ponto exato onde foi mais eficiente.

- **Visualização de Convergência**: O gráfico final permite diagnosticar a saúde do treino. Se as duas curvas (Treino e Validação) descerem juntas, o aprendizado está saudável.

from copy import deepcopy

# 1. Configuração Inicial e Reset de Métricas
best_val_loss = float('inf')
best_model_state = None
train_losses, val_losses = [], []

print("Iniciando Treinamento do Aglomerado de Metais...")
print(f"Hardware: {device} | Ativos: Ma'aden (1211.SR) e Rio Tinto (RIO)")
print("-" * 70)

# Loop de 50 Épocas - Impressão 1 por 1
for epoch in range(1, 51):
    # --- FASE DE TREINO ---
    model.train()
    batch_losses = []

    for xb, yb in train_loader:
        xb, yb = xb.to(device), yb.to(device)

        optimizer.zero_grad()
        preds = model(xb)
        loss = criterion(preds, yb)
        loss.backward()
        optimizer.step()

        batch_losses.append(loss.item())

    train_loss = np.mean(batch_losses)

    # --- FASE DE VALIDAÇÃO ---
    model.eval()
    val_batch_losses = []

    with torch.no_grad():
        for xb, yb in test_loader:
            xb, yb = xb.to(device), yb.to(device)
            preds = model(xb)
            v_loss = criterion(preds, yb)
            val_batch_losses.append(v_loss.item())

    val_loss = np.mean(val_batch_losses)
    train_losses.append(train_loss)
    val_losses.append(val_loss)

    # LOG DE PROGRESSO: Imprimindo todas as épocas
    print(f"Epoch {epoch:02d}/50 | Erro Treino: {train_loss:.6f} | Erro Validação: {val_loss:.6f}")

    # 2. Checkpoint do melhor modelo (Early Saving)
    if val_loss < best_val_loss:
        best_val_loss = val_loss
        best_model_state = deepcopy(model.state_dict())

# 3. Restauração do melhor estado encontrado
if best_model_state:
    model.load_state_dict(best_model_state)
    print("-" * 70)
    print(f"Treinamento Concluído! Melhor Val Loss: {best_val_loss:.6f}")

# 4. Gráfico das Curvas de Aprendizado
plt.figure(figsize=(12, 5))
plt.plot(train_losses, label='Erro de Treino', color='#4F4F4F', linewidth=2)
plt.plot(val_losses, label='Erro de Validação', linestyle='--', color='#D2691E', linewidth=2)
plt.title('Curvas de Convergência - Evolução Época por Época', fontsize=14)
plt.xlabel('Época')
plt.ylabel('MSE Loss')
plt.legend()
plt.grid(True, alpha=0.3)
plt.show()

**Avaliação Multivariada e Desnormalização (Fluxo 2)**

Nesta etapa, o modelo processa os dados de teste (que ele nunca viu antes) e gera previsões simultâneas para os dois ativos. Em seguida, convertemos esses sinais matemáticos de volta para valores monetários reais.

**Destaques da Lógica:**

- `model.eval()`: Desliga camadas de regularização (como Dropout) para garantir previsões consistentes.

- **Matriz Fantasma**: O `scaler_metais_dif` espera 8 colunas (preços + indicadores). Ao preencher apenas as colunas de fechamento e inverter a escala, recuperamos os valores em SAR e USD.

- **Visualização Dual**: Plotamos dois gráficos lado a lado para observar se o modelo captura a correlação entre a mineração saudita e a global.

# 1. Avaliação Multivariada: Real vs Previsto para as 2 ações de Metais
model.eval()
all_preds = []
all_actuals = []

with torch.no_grad():
    for xb, yb in test_loader:
        xb = xb.to(device)
        out = model(xb) # Gera as 2 predições simultâneas (Ma'aden e Rio Tinto)
        all_preds.append(out.cpu().numpy())
        all_actuals.append(yb.numpy())

# Transformar listas em arrays numpy
preds_scaled = np.concatenate(all_preds, axis=0)
actuals_scaled = np.concatenate(all_actuals, axis=0)

# --- Função de Desnormalização para Aglomerado de Metais ---
def get_inverse_prices(scaled_data, current_scaler, current_target_indices):
    # Criamos uma matriz "fantasma" com o shape original (N amostras, 8 features)
    n_features = current_scaler.n_features_in_
    dummy = np.zeros((len(scaled_data), n_features))

    # Preenchemos apenas as colunas de fechamento (Close) nos índices corretos de Metais
    for i, col_idx in enumerate(current_target_indices):
        dummy[:, col_idx] = scaled_data[:, i]

    # Inverte a escala para voltar aos valores monetários originais
    inverse = current_scaler.inverse_transform(dummy)

    # Extrai apenas as colunas de preço desnormalizadas (SAR e USD)
    final_prices = []
    for col_idx in current_target_indices:
        final_prices.append(inverse[:, col_idx])

    return np.array(final_prices).T

# Obter preços finais (Desnormalizados usando as variáveis do Fluxo 2)
# IMPORTANTE: Usamos 'scaler_metais_dif' e 'target_indices_metais'
preds_final = get_inverse_prices(preds_scaled, scaler_metais_dif, target_indices_metais)
actuals_final = get_inverse_prices(actuals_scaled, scaler_metais_dif, target_indices_metais)

# --- Plotagem dos 2 Gráficos de Metais ---
tickers_label = ['Ma\'aden (1211.SR)', 'Rio Tinto (RIO)']
units = ['SAR', 'USD']
colors_real = ['#4F4F4F', '#4F4F4F'] # Cinza Escuro
colors_pred = ['#D2691E', '#D2691E'] # Âmbar/Bronze para Metais

fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Avaliação Fluxo 2: Preço Real vs. Previsto - Setor de Metais', fontsize=18)

for i in range(len(tickers_label)):
    ax = axs[i]
    ax.plot(actuals_final[:, i], label='Preço Real', color=colors_real[i], alpha=0.7, linewidth=2)
    ax.plot(preds_final[:, i], label='Previsão LSTM+GRU', color=colors_pred[i], linestyle='--', linewidth=1.5)

    ax.set_title(f'Ativo: {tickers_label[i]}', fontsize=14)
    ax.set_ylabel(f'Preço de Fechamento ({units[i]})')
    ax.set_xlabel('Tempo (Amostras de Teste)')
    ax.legend()
    ax.grid(True, alpha=0.3)

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

**O que observar nos resultados?**

1. **Aderência**: Se a linha tracejada segue a linha sólida com um pequeno atraso (*lag*), o modelo aprendeu a tendência, mas ainda depende muito do dia anterior.

2. **Captura de Picos**: Veja se a Rio Tinto (mais volátil) faz o modelo "sofrer" mais que a Ma'aden. Isso indica que o mercado global de metais tem ruídos macro que talvez exijam mais features no futuro.

**Diagnóstico de Variabilidade: A "Biópsia" da Rede (Metais)**

Nesta etapa, analisamos os valores brutos que saem da última camada linear do modelo (antes da desnormalização). O objetivo é garantir que a rede está "viva" e reagindo às nuances do mercado de minério e metais industriais.

**O que procurar neste diagnóstico? **

- **Variabilidade (Standard Deviation)**: Se o desvio padrão for muito baixo ($< 0.01$), a rede parou de tentar prever o futuro e está apenas "sobrevivendo" com a média.
- **Amplitude de Saída**: As predições devem ocupar uma faixa de valores similar aos dados de treino. Se a rede só prevê valores entre 0.45 e 0.46, ela está em um estado de sub-ajuste (*underfitting*).
- **Morfologia da Curva**: Procuramos por "serrilhados" ou ondas que mimetizam o comportamento real dos ativos.

# --- DIAGNÓSTICO: DISTRIBUIÇÃO DAS PREDIÇÕES NORMALIZADAS (METAIS) ---

# Tickers atualizados para o contexto de Metais
tickers_label = ['Ma\'aden (1211.SR)', 'Rio Tinto (RIO)']
colors = ['#4F4F4F', '#D2691E'] # Cinza Siderúrgico e Âmbar de Minério

# Criamos a figura com 2 subplots para diagnóstico individual
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Diagnóstico de Saída da Rede: Predições Normalizadas de Metais (0-1)', fontsize=16)

# preds_scaled são os valores brutos (0-1) que saíram da última camada Linear da rede
print("=== Relatório de Diagnóstico de Saída (Escala 0-1) - Metais ===")

for i in range(len(tickers_label)):
    ax = axs[i]

    # Plotamos as primeiras 100 predições para observar a "volatilidade" da rede
    # Se a linha estiver muito reta, a rede não está captando a variação temporal
    ax.plot(preds_scaled[:100, i], color=colors[i], label=f'Pred {tickers_label[i]}', linewidth=2)

    # Métricas estatísticas da saída normalizada (cruciais para detectar problemas)
    p_min, p_max = preds_scaled[:, i].min(), preds_scaled[:, i].max()
    p_mean = preds_scaled[:, i].mean()
    p_std = preds_scaled[:, i].std()

    ax.set_title(f'Ativo: {tickers_label[i]}')
    ax.set_ylabel('Valor Normalizado (Saída da Rede)')
    ax.set_xlabel('Amostras (Dias de Teste)')
    ax.grid(True, linestyle='--', alpha=0.5)
    ax.legend(loc='upper right')

    # Relatório técnico no console
    print(f"{tickers_label[i]}:")
    print(f"  > Amplitude: {p_min:.4f} até {p_max:.4f}")
    print(f"  > Média: {p_mean:.4f} | Desvio Padrão: {p_std:.4f}")

    # Alerta de sanidade: Desvio padrão muito baixo (< 0.01) indica sub-ajuste
    if p_std < 0.01:
        print("  ⚠️ AVISO: Baixa variabilidade nas predições. Verifique o aprendizado.")
    else:
        print("  ✅ Variabilidade detectada. A rede está tentando seguir a tendência.")
    print("-" * 50)

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

**Insight do Negócio**: No setor de Metais, é comum que o desvio padrão da **Rio Tinto (RIO)** seja ligeiramente superior ao da **Ma'aden (1211.SR**), dada a liquidez global e a exposição direta ao mercado de contratos futuros de Londres. Se o seu diagnóstico mostrar isso, o modelo está capturando a diferença de natureza entre os dois ativos.

**Projeção Multivariada: Janela Móvel de 5 Dias (Metais)**

Neste bloco, realizamos a projeção para a próxima semana útil. O modelo analisa a última janela real de 60 dias e gera, passo a passo, a tendência esperada para a **Ma'aden** (mencionada no código como Baoshan) e para a **Rio Tinto**.

**Como funciona o Mecanismo de Recursão? **

1. **Input Inicial**: Pegamos os últimos 60 dias reais do dataset.
2. **Primeira Previsão**: O modelo gera o preço para o dia $T+1$.
3. **Atualização da Janela**: Removemos o dia mais antigo ($T-60$) e inserimos a nossa própria previsão no final da fila.
4. **Repetição**: Usamos essa nova janela "híbrida" (59 dias reais + 1 previsto) para prever o dia $T+2$.

# --- Previsão Multivariada de 5 dias à frente (Baoshan & Rio Tinto) ---
model.eval()
n_future = 5  # Projeção para a próxima semana útil
tickers_label = ['Baoshan Steel (1211.SR)', 'Rio Tinto (RIO)']
moedas = ['SAR', 'USD'] # Baoshan em Riyals (Tadawul), Rio Tinto em Dólares
colors_plot = ['#4F4F4F', '#D2691E'] # Cinza Siderúrgico e Âmbar Minério

# 1. Preparação da última janela real disponível (Lookback de 60 dias)
# CORREÇÃO: Usamos os dados de metais (scaled_metais_dif) que já estão normalizados
# Isso evita o erro de chamar .tail() em um objeto que pode não ser o DataFrame correto
last_scaled = scaled_metais_dif[-seq_len:]

# Tensor inicial: Shape [1, 60, 8]
current_input = torch.tensor(last_scaled, dtype=torch.float32).unsqueeze(0).to(device)

future_preds_scaled = []

for _ in range(n_future):
    with torch.no_grad():
        # O modelo prevê os 2 fechamentos simultaneamente
        next_pred = model(current_input)
        pred_vals = next_pred.cpu().numpy()[0] # [Pred_Baoshan, Pred_Rio]
        future_preds_scaled.append(pred_vals)

    # 2. Mecanismo de Recursão (Auto-regressivo)
    # Criamos a entrada para o "amanhã" baseada na previsão de "hoje"
    new_entry = current_input[0, -1, :].cpu().numpy().copy()

    # Atualizamos apenas as colunas de FECHAMENTO (target_indices_metais)
    for i, idx in enumerate(target_indices_metais):
        new_entry[idx] = pred_vals[i]

    # 3. Sliding Window: Deslocamos a janela 1 dia para a frente
    new_entry_tensor = torch.tensor(new_entry, dtype=torch.float32).view(1, 1, -1).to(device)
    # Removemos o dia mais antigo (index 0) e adicionamos a nova predição no fim
    current_input = torch.cat([current_input[:, 1:, :], new_entry_tensor], dim=1)

# --- DESNORMALIZAÇÃO PARA VALORES MONETÁRIOS ---
future_preds_scaled = np.array(future_preds_scaled)

def denormalize_future(scaled_data, current_scaler, current_indices):
    n_features = current_scaler.n_features_in_
    dummy = np.zeros((len(scaled_data), n_features))
    for i, idx in enumerate(current_indices):
        dummy[:, idx] = scaled_data[:, i]
    # CORREÇÃO: Usamos explicitamente o scaler de metais
    inv = current_scaler.inverse_transform(dummy)
    return inv[:, current_indices]

# Obter preços finais
future_prices = denormalize_future(future_preds_scaled, scaler_metais_dif, target_indices_metais)

# --- PLOTAGEM DAS PROJEÇÕES LADO A LADO ---
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle(f'Projeção do Setor de Metais para os Próximos {n_future} Dias Úteis', fontsize=18)

dias_futuros = range(1, n_future + 1)

for i in range(len(tickers_label)):
    ax = axs[i]
    ax.plot(dias_futuros, future_prices[:, i], marker='o', color=colors_plot[i],
            linestyle='--', linewidth=2.5, markersize=10)

    ax.set_title(f'Estimativa: {tickers_label[i]}', fontsize=14, fontweight='bold')
    ax.set_ylabel(f'Preço ({moedas[i]})')
    ax.set_xlabel('Dias à frente (T+n)')
    ax.set_xticks(dias_futuros)
    ax.grid(True, linestyle=':', alpha=0.6)

    # Adicionar labels de valor exato sobre os pontos
    for x, y in zip(dias_futuros, future_prices[:, i]):
        ax.annotate(f'{y:.2f}', (x, y), textcoords="offset points",
                    xytext=(0,15), ha='center', fontsize=10, fontweight='bold', color=colors_plot[i])

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# --- TABELA DE DECISÃO ---
print(f"\n--- Resumo de Projeção: Aglomerado de Metais ---")
df_future = pd.DataFrame(future_prices, columns=tickers_label,
                         index=[f"Dia +{i+1}" for i in range(n_future)])
print(df_future.round(3))

**Persistência de Resultados e Métricas Finais (Metais)**

Nesta etapa, isolamos as predições desnormalizadas para o cálculo das métricas de erro. O **MAPE** (**Mean Absolute Percentage Erro**r) é a métrica favorita dos gestores de portfólio, pois traduz o erro do modelo em uma porcentagem clara (ex: "o modelo erra, em média, 1.5% do valor da ação").

**Por que o isolamento de dados é crítico?**
- **Integridade do Fluxo**: Separa os ativos em SAR (Ma'aden) e USD (Rio Tinto) de outros fluxos.

- **Auditabilidade**: Permite verificar o erro residual em cada ativo individualmente.

- **Preparação para o Dashboard**: Facilita a plotagem de tabelas comparativas no final do notebook.

# Salva os resultados específicos de Metais
preds_final_metais = preds_final.copy()
actuals_final_metais = actuals_final.copy()

**Consolidação e Persistência de Dados (Fluxo 2)**

Nesta etapa, garantimos a integridade dos dados para a análise comparativa final. O isolamento de variáveis é uma prática de **Clean Code** em Data Science que evita a contaminação de resultados entre diferentes ativos.

**Por que o isolamento é estratégico?**
- **Divergência de Moedas**: Mantemos os valores em** SAR** (Ma'aden) e **USD** (Rio Tinto) separados dos fluxos que usam outras paridades.

- **Análise Intersetorial**: Permite calcular correlações de erro. Se o modelo errar para cima em ambos os fluxos simultaneamente, pode indicar um fator macro (como o Dólar Global) que não foi totalmente capturado.

- **Segurança de Memória**: Evita que um novo treinamento de outro aglomerado sobrescreva os arrays `preds_final` genéricos.

# Garante que os resultados de metais fiquem salvos em variáveis exclusivas
preds_metais = preds_final.copy()
actuals_metais = actuals_final.copy()

print("✓ Resultados de Metais salvos. Prontos para a análise intersetorial.")

## Matriz de Correlação e Alinhamento de Dados - Mercados Diferentes 

Primeiro, vamos criar um DataFrame único que contenha os erros de previsão (ou os preços previstos) de ambos os aglomerados para o período de teste.

import seaborn as sns

# Petróleo: actuals_final_petro, preds_final_petro
# Metais: actuals_final_metais, preds_final_metais

# Criando um DataFrame de comparação (alinhando pelo tamanho do conjunto de teste)
# Nota: Use o menor tamanho entre os dois caso haja diferença de dias úteis
# Usamos o menor tamanho entre os dois conjuntos de teste
min_len = min(len(preds_final_petro), len(preds_final_metais))

# 2. Criando o DataFrame de comparação intersetorial
df_corr = pd.DataFrame({
    'Petroleo_Aramco': preds_final_petro[-min_len:, 0],
    'Petroleo_Total':  preds_final_petro[-min_len:, 1],
    'Metais_Baoshan':  preds_final_metais[-min_len:, 0],
    'Metais_RioTinto': preds_final_metais[-min_len:, 1]
})

# 3. Calculando a Matriz de Correlação de Pearson
corr_matrix = df_corr.corr()

# 4. Visualização com Heatmap
plt.figure(figsize=(10, 8))
sns.heatmap(corr_matrix,
            annot=True,
            cmap='RdYlGn',
            center=0,
            fmt=".2f",
            linewidths=0.5)

plt.title('Matriz de Correlação Intersetorial: Petróleo vs Metais', fontsize=14)
plt.show()

###2. Análise de Correlação de Retornos Previstos

Em finanças, a correlação de preços nominais pode ser espúria. É mais preciso correlacionar a **variação percentual (retornos)** que o modelo está prevendo.

# Calculando retornos diários das predições (Variação %)
df_retornos = df_corr.pct_change().dropna()

# Visualização de Dispersão (Scatter Plot com Linha de Regressão)
plt.figure(figsize=(14, 5))

# Comparando os "líderes" de cada cluster: Aramco vs Rio Tinto
plt.subplot(1, 2, 1)
sns.regplot(data=df_retornos, x='Petroleo_Aramco', y='Metais_RioTinto',
            scatter_kws={'alpha':0.4, 'color':'forestgreen'}, line_kws={'color':'red'})
plt.title('Retornos: Saudi Aramco vs Rio Tinto')
plt.grid(True, alpha=0.3)

# Comparando TotalEnergies vs Baoshan Steel
plt.subplot(1, 2, 2)
sns.regplot(data=df_retornos, x='Petroleo_Total', y='Metais_Baoshan',
            scatter_kws={'alpha':0.4, 'color':'royalblue'}, line_kws={'color':'red'})
plt.title('Retornos: TotalEnergies vs Baoshan Steel')
plt.grid(True, alpha=0.3)

plt.tight_layout()
plt.show()

print("=== Matriz de Correlação de Retornos (Variação %) ===")
print(df_retornos.corr().round(4))

###3. O que os resultados podem indicar?

- Alta Correlação Positiva (> 0.7): Indica que seus modelos estão capturando um fator macroeconômico comum (como a inflação global ou a força do dólar) que move tanto o setor de energia quanto o de materiais básicos.

- Correlação Próxima de Zero: Sugere que os aglomerados são independentes. Isso é excelente para a diversificação de carteira, pois o risco de um setor não afeta diretamente o outro.

- Divergência nas Projeções de 5 dias: Se a projeção do Petróleo for de alta e a de Metais for de baixa, você pode estar diante de um cenário de rotação de setor no mercado.

print("\n--- Guia de Interpretação ---")
# Lógica simples para ajudar no diagnóstico
avg_corr = df_retornos.corr().values[np.triu_indices_from(df_retornos.corr().values, k=1)].mean()

if avg_corr > 0.7:
    print("⚠️ ALTA CORRELAÇÃO: Os setores estão se movendo em bloco (Efeito Macro/Dólar).")
elif avg_corr < 0.3:
    print("✅ BAIXA CORRELAÇÃO: Boa diversificação. Os setores possuem dinâmicas independentes.")
else:
    print("ℹ️ CORRELAÇÃO MODERADA: Existe influência mútua, mas com espaço para movimentos individuais.")

##  13.2. Bloco B: Cenários de Mercados Iguais (Sincronia Total)

Neste grupo de 4 redes, eliminamos a variável "tempo/fuso horário" para focar exclusivamente na **Correlação de Ativos**. Como ambos operam na mesma janela da NYSE (Segunda a Sexta), o desafio da rede é puramente matemático.

### **Configuração do Experimento:**
* **Petróleo (NYSE):** `XOM` (ExxonMobil) + `CVX` (Chevron).
* **Metais (NYSE):** `FCX` (Freeport-McMoRan) + `RIO` (Rio Tinto).

> **O que a rede deve aprender:** Como o preço de uma gigante de energia ou mineração dita o ritmo da outra quando ambas reagem simultaneamente às mesmas notícias de abertura e fechamento do mercado americano.

### Aglomerado de Petróleo

**Aglomerado de Petróleo (XOM & TTE)**

Este bloco consolida os dados da **Exxon Mobil** e da **TotalEnergie**s. O ajuste principal aqui é garantir que, após a limpeza, os dados estejam prontos para alimentar o `MinMaxScaler`, gerando o objeto scaled.

# 1. Definição dos tickers para o Aglomerado de Petróleo (XOM e TTE no mesmo calendário)
tickers = ['XOM', 'TTE']
dfs = []

for t in tickers:
    # 2. Download dos dados (auto_adjust=False para manter consistência com nomes de colunas)
    df_raw = yf.download(t, start='2019-01-01', end='2026-03-22', progress=False, auto_adjust=False)

    # 3. Cópia para evitar avisos de SettingWithCopy e manipulação segura
    df = df_raw.copy()

    # 4. TRATAMENTO DE COLUNAS:
    # Remove nível de Ticker se o yfinance retornar MultiIndex
    if isinstance(df.columns, pd.MultiIndex):
        df.columns = df.columns.get_level_values(0)

    # 5. Seleção da coluna de Fechamento e Renomeação Única
    # Usamos 'Adj Close' por ser o padrão ouro para análise histórica, se disponível
    col_alvo = 'Adj Close' if 'Adj Close' in df.columns else 'Close'
    df = df[[col_alvo]].rename(columns={col_alvo: f'{t}_Close'})

    # 6. Limpeza de duplicatas acidentais no índice de colunas
    df = df.loc[:, ~df.columns.duplicated()]

    # 7. Aplicação dos Indicadores (SMA, EMA, RSI)
    # Cálculo isolado por ativo para evitar contaminação de médias móveis entre empresas
    df = add_indicators(df, col=f'{t}_Close', window=14)
    dfs.append(df)

# 8. CONCATENAÇÃO E SINCRONIZAÇÃO
# ffill(): Preenche eventuais gaps de feriados específicos de uma das bolsas
# dropna(): Remove as primeiras linhas (onde os indicadores ainda não possuem histórico suficiente)
data = pd.concat(dfs, axis=1).ffill().dropna()

# 9. MAPEAMENTO DOS ALVOS (Target Indices)
# Identifica a posição numérica das colunas de fechamento para a rede neural
target_cols = [col for col in data.columns if 'close' in col.lower()]
target_indices = [data.columns.get_loc(c) for c in target_cols]

print(f"✓ Colunas no DataFrame final: {data.columns.tolist()}")
print(f"✓ Índices das colunas Alvo: {target_indices}")
data.tail()

**Normalização Multivariada com Identificação Exclusiva**

Nesta etapa, criamos o objeto `scaler_petro_eq` e o array `scaled_petro_eq`. O sufixo **_petro_eq** (Petróleo Equitativo/Mesmo Mercado) garante que esses pesos e valores fiquem protegidos na memória do Python, permitindo que você rode outros fluxos simultaneamente sem conflitos.

# Inicialização do Scaler
scaler_petro_eq = MinMaxScaler()

#  Ajuste e Transformação
# O array 'scaled_petro_eq' recebe a normalização 0-1 automaticamente
scaled_petro_eq = scaler_petro_eq.fit_transform(data)

**Criação de Sequências Temporais (X e y)**

Nesta etapa, fatiamos o histórico em blocos de 60 dias ($X$) para prever o próximo dia ($y$). O uso de `target_indices` aqui é fundamental, pois garante que o modelo tente prever apenas os preços de fechamento (**XOM** e **TTE**), ignorando os indicadores técnicos no vetor de saída ($y$), mas usando-os como contexto no vetor de entrada ($X$).

**Validação Técnica:**

- **X_petro_eq**: Possui 3 dimensões, exatamente o que a camada `nn.LSTM` do PyTorch espera.

- **y_petro_eq**: Possui 2 dimensões (os dois preços de fechamento), permitindo que o modelo aprenda a correlação entre a Exxon e a TotalEnergies simultaneamente.

- **Independência**: Ao usar o sufixo `_petro_eq`, garantimos que estes dados não sejam confundidos com o Fluxo 1 (Petróleo Diferente) ou o Fluxo 2 (Metais).

def create_multivariate_sequences(data, seq_len, target_indices):
    X, y = [], []

    # Garantimos que os dados estejam no formato numpy array para fatiamento eficiente
    data_array = np.array(data)

    # O loop percorre os dados a partir do tamanho da janela (seq_len)
    for i in range(seq_len, len(data_array)):
        # X: Janela histórica (ex: 60 dias) com todas as 8 features (Close, SMA, EMA, RSI)
        # Captura todas as colunas das linhas de [i-seq_len] até [i-1]
        X.append(data_array[i-seq_len:i, :])

        # y: Os valores de fechamento (Target) de AMBOS os ativos no dia exato 'i'
        # O target_indices extrai apenas as colunas de 'Close' (XOM e TTE)
        y.append(data_array[i, target_indices])

    return np.array(X), np.array(y)

**DIVISÃO DE DADOS (TREINO E TESTE) - PETRÓLEO EQUITATIVO**

Este bloco realiza a partição dos dados garantindo a integridade da série temporal. Os dados são divididos em 80% para o aprendizado dos padrões históricos e 20% para a validação da capacidade preditiva do modelo em cenários inéditos.

**Destaques da Configuração:**

1. **Ordem Cronológica**: A divisão é feita por fatiamento linear (`split`), impedindo que o modelo "veja o futuro" durante o treinamento (vazamento de dados).
2. **Multivariedade**: O conjunto de dados carrega todas as 8 features (preços e indicadores) para a entrada ($X$), enquanto foca nos 2 preços de fechamento para a saída ($y$).
3. **Independência de Memória**: Utilizamos sufixos `_petro` para garantir que estes conjuntos de dados não sejam sobrescritos por outros aglomerados.

# --- CONFIGURAÇÃO DE JANELAS E DIVISÃO (PETRÓLEO) ---

# 1. Configuração da janela temporal (60 dias de histórico para prever o próximo)
seq_len = 60
X_petro, y_petro = create_multivariate_sequences(scaled_petro_eq, seq_len, target_indices)

# 2. Divisão treino/teste (80% para treino, 20% para validação/teste)
# Mantemos a ordem cronológica: os primeiros 80% treinam, os últimos 20% testam
split = int(0.8 * len(X_petro))
X_train_petro, X_test_petro = X_petro[:split], X_petro[split:]
y_train_petro, y_test_petro = y_petro[:split], y_petro[split:]

# --- VERIFICAÇÃO DE SEGURANÇA PARA O AGLOMERADO ATUAL ---
print(f"=== Verificação de Dimensões (XOM & TTE) ===")
print(f"✓ Shape de X_train_petro: {X_train_petro.shape}") # Esperado: (N, 60, 8)
print(f"✓ Shape de y_train_petro: {y_train_petro.shape}") # Esperado: (N, 2) -> 2 fechamentos alvo

# EXPLICAÇÃO DAS DIMENSÕES:
# N  = Número total de janelas sequenciais geradas (amostras)
# 60 = Timesteps (dias de histórico que a LSTM/GRU processa por vez)
# 8  = Features totais (XOM: Close, SMA, EMA, RSI + TTE: Close, SMA, EMA, RSI)
# 2  = Saídas da rede (Previsão do 'Close' simultâneo para os dois tickets)

**CLASSE CUSTOMIZADA PARA SÉRIES TEMPORAIS**

Este bloco define a estrutura de dados necessária para que o PyTorch consiga ler as janelas temporais de **XOM** e **TTE**. A classe converte os dados para tensores e permite o acesso indexado durante o treinamento.

#CLASSE CUSTOMIZADA PARA SÉRIES TEMPORAIS
class TimeSeriesDataset(Dataset):
    def __init__(self, X, y):
        # Conversão explícita para tensores float32 (Padrão exigido pelo PyTorch)
        self.X = torch.tensor(X, dtype=torch.float32)
        self.y = torch.tensor(y, dtype=torch.float32)

    def __len__(self):
        # Retorna o número total de janelas sequenciais
        return len(self.X)

    def __getitem__(self, idx):
        # Retorna um par (Janela de Histórico, Preços de Fechamento Alvo)
        return self.X[idx], self.y[idx]

**INSTANCIAÇÃO DOS DATASETS E DATALOADERS (PETRÓLEO)**

Nesta etapa, aplicamos a classe customizada aos dados de treino e teste e configuramos os `DataLoaders`. O uso de batches (lotes) de 32 permite que o modelo processe os dados de forma eficiente, otimizando o uso da memória e a estabilidade do treinamento.

**Destaques da Configuração:**
1. **Batch Processing**: Definimos o `batch_size = 32`, um equilíbrio ideal entre velocidade de processamento e convergência do erro.

2. **Generalização**: O `shuffle=True` no conjunto de treino garante que o modelo aprenda padrões técnicos e não apenas a ordem cronológica das janelas.

3. **Padronização**: As variáveis seguem o padrão `X_train_petro` e `y_train_petro` para evitar conflitos com outros aglomerados (Metais/Energia).

# INSTANCIAÇÃO DOS DATASETS (FLUXO PETRÓLEO: XOM & TTE)
train_ds = TimeSeriesDataset(X_train_petro, y_train_petro)
test_ds = TimeSeriesDataset(X_test_petro, y_test_petro)

# CONFIGURAÇÃO DOS DATALOADERS
# Batch size padronizado em 32 para estabilidade do treinamento
train_loader = DataLoader(train_ds, batch_size=32, shuffle=True)
test_loader = DataLoader(test_ds, batch_size=32)

**VALIDAÇÃO VISUAL E ESTATÍSTICA DOS ALVOS (PETRÓLEO)**

Este bloco permite visualizar as primeiras 100 amostras dos alvos (targets) para garantir que a normalização e a separação dos dados foram executadas corretamente. É uma etapa de segurança vital antes de iniciar o treinamento da rede neural.

Destaques da Validação:
- **Sincronia Temporal**: Verifica se as oscilações de **XOM** e **TTE** seguem o padrão esperado dentro do intervalo $[0, 1]$.
- **Rótulos Automáticos**: Os títulos dos gráficos são gerados dinamicamente com base na lista de tickers definida no início do código.
- **Check Estatístico**: O console exibe os valores mínimo, máximo e médio para confirmar que não há *outliers* ou erros de escala no `y_train_petro`.

# --- VISUALIZAÇÃO DOS ALVOS (Y_TRAIN): FLUXO PETRÓLEO ---

# Configuração de rótulos e cores para os ativos do aglomerado
tickers_label = [f"Ativo {i+1} ({t})" for i, t in enumerate(tickers)]
colors = ['forestgreen', 'royalblue']

# Criamos uma figura com 2 subplots (1 linha e 2 colunas)
fig, axs = plt.subplots(1, 2, figsize=(15, 6))
fig.suptitle(f'Distribuição dos Alvos do Aglomerado - Primeiras 100 Amostras (y_train_petro Normalizado)', fontsize=16)

# Iteramos sobre os subplots para plotar os dois alvos (targets) simultâneos
for i in range(len(tickers_label)):
    ax = axs[i]

    # Plota as primeiras 100 amostras (janelas) usando a variável exclusiva y_train_petro
    # O eixo y representa o valor normalizado (0 a 1) do preço de fechamento
    ax.plot(y_train_petro[:100, i], color=colors[i], label='Target Normalizado', linewidth=2)

    ax.set_title(f'Série Temporal: {tickers_label[i]}')
    ax.set_xlabel('Sequência de Amostras (Tempo)')
    ax.set_ylabel('Valor de Fechamento (Escala 0-1)')
    ax.grid(True, alpha=0.3)
    ax.legend(loc='upper right')

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# Print para conferência técnica e validação estatística dos alvos
print(f"=== Conferência Técnica: Estatísticas do Aglomerado (Petróleo) ===")
for i, ticker in enumerate(tickers_label):
    # Verificação se a normalização está correta (valores devem estar entre 0 e 1)
    v_min = y_train_petro[:, i].min()
    v_max = y_train_petro[:, i].max()
    v_med = y_train_petro[:, i].mean()
    print(f"{ticker}: min={v_min:.4f}, max={v_max:.4f}, média={v_med:.4f}")

**ARQUITETURA DO MODELO HÍBRIDO (LSTM + GRU)**

Nesta etapa, definimos a estrutura da rede neural profunda. A combinação de **LSTM** e **GRU** permite que o modelo capture tanto tendências de longo prazo (memória persistente) quanto variações bruscas de curto prazo (volatilidade recente), ideal para a correlação entre ativos como **XOM** e **TTE**.

**Destaques da Arquitetura:**
- **Camada LSTM**: Atua como o extrator primário de características, processando a sequência de 60 dias para identificar padrões cíclicos e tendências macro.

- **Camada GRU**: Refina a saída da LSTM, focando em ajustes rápidos e momentum, sendo computacionalmente mais eficiente para capturar dinâmicas recentes.

- **Saída Multivariada**: A camada linear final (`fc`) projeta os estados ocultos diretamente para 2 saídas, permitindo que a rede aprenda a correlação intrínseca entre os dois ativos simultaneamente.

# --- DEFINIÇÃO DA CLASSE DO MODELO ---

class LSTM_GRU_Model(nn.Module):
    def __init__(self, input_size, hidden_lstm=64, hidden_gru=32, output_size=2):
        super().__init__()

        # Camada LSTM: Processa a sequência temporal histórica
        # O input_size é 8 (2 tickets * 4 indicadores: Close, SMA, EMA, RSI)
        self.lstm1 = nn.LSTM(input_size=input_size,
                            hidden_size=hidden_lstm,
                            batch_first=True)

        # Camada GRU: Refina os padrões extraídos pela LSTM
        # Foca na dinâmica de curto prazo e variações recentes da série
        self.gru = nn.GRU(input_size=hidden_lstm,
                         hidden_size=hidden_gru,
                         batch_first=True)

        # Camada de Saída (Linear): Mapeia as características para as previsões
        # O output_size é 2 (previsão simultânea do fechamento de ambos os ativos)
        self.fc = nn.Linear(hidden_gru, output_size)

    def forward(self, x):
        # x shape de entrada: (batch, seq_len, 8)

        # Passagem pela LSTM - Captura memórias de longo prazo (Tendências)
        out_lstm1, _ = self.lstm1(x)
        # out_lstm1 shape: (batch, seq_len, hidden_lstm)

        # Passagem pela GRU - Captura volatilidade e ajustes rápidos (Momentum)
        out_gru, _ = self.gru(out_lstm1)
        # out_gru shape: (batch, seq_len, hidden_gru)

        # Selecionamos apenas o estado do ÚLTIMO passo temporal da sequência (T)
        # Este vetor contém a síntese de toda a janela para prever o próximo dia (T+1)
        last_time_step = out_gru[:, -1, :]

        # Geração das predições para os 2 ativos do aglomerado
        final_output = self.fc(last_time_step)  # Shape final: (batch, 2)

        return final_output

**CONFIGURAÇÃO TÉCNICA E INSTANCIAÇÃO DO MODELO (PETRÓLEO)**

Nesta etapa, preparamos o ambiente de execução e instanciamos os componentes críticos do treinamento. O modelo é alocado no hardware disponível (GPU/CPU) e configuramos as métricas de erro que guiarão o aprendizado da correlação entre os ativos.

**Destaques da Configuração:**
- **Detecção Automática**: O `input_size` é extraído diretamente do shape de treino, garantindo flexibilidade caso novos indicadores sejam adicionados.

- **Métrica de Erro (MSE)**: O Erro Quadrático Médio foca em minimizar grandes desvios, o que é vital para a estabilidade em previsões de fechamento financeiro.

- **Otimização Adaptativa**: O algoritmo **Adam** ajusta a taxa de aprendizado dinamicamente, facilitando a convergência em séries temporais com alta volatilidade.

# --- CONFIGURAÇÃO E INSTANCIAÇÃO: PETRÓLEO (XOM & TTE) ---

# Detectar o número de colunas (features) automaticamente
# O input_size será 8 (XOM: 4 + TTE: 4 indicadores)
input_size = X_train_petro.shape[2]

# Definir o dispositivo de processamento (GPU se disponível, senão CPU)
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")

# Inicializar o Modelo Híbrido (LSTM + GRU) exclusivo para Petróleo
# O output_size é 2 para prever simultaneamente o fechamento de ambos os ativos
model_petro_eq = LSTM_GRU_Model(input_size=input_size, output_size=2).to(device)

# Função de Perda (Loss Function)
# O MSE (Erro Quadrático Médio) é ideal para regressão de preços,
# pois penaliza erros maiores, buscando maior precisão no fechamento.
criterion = nn.MSELoss()

# Otimizador (Adam)
# Algoritmo de aprendizado adaptativo, eficiente para capturar a
# volatilidade e tendências em séries temporais financeiras.
optimizer = torch.optim.Adam(model_petro_eq.parameters(), lr=0.001)

# --- VERIFICAÇÃO DE INICIALIZAÇÃO ---
print(f"=== Status do Modelo: Petróleo (XOM/TTE) ===")
print(f"✓ Modelo inicializado no dispositivo: {device}")
print(f"✓ Parâmetros de Entrada (Features): {input_size}")
print(f"✓ Parâmetros de Saída (Targets): 2")
print("-" * 55)

**LOOP DE TREINAMENTO E CURVA DE APRENDIZADO (PETRÓLEO)**

Nesta etapa, o modelo processa repetidamente os dados históricos para aprender a correlação entre os ativos. Utilizamos uma estratégia de **Checkpoint**, onde o estado do modelo é salvo apenas quando o erro de validação diminui, garantindo que a versão final seja a mais precisa possível e evitando o *overfitting*.

**Destaques do Processamento**:
- **Backpropagation**: O otimizador ajusta os pesos da rede a cada *batch* baseado no erro quadrático médio (MSE).

- **Validação em Tempo Real**: A cada época, testamos o modelo em dados que ele não usou para treinar, monitorando a capacidade de generalização.

- **Restauração de Pesos**: Ao final das 50 épocas, o script restaura automaticamente os pesos do melhor momento do treinamento (`best_model_state`).

from copy import deepcopy

# --- CONFIGURAÇÃO INICIAL DO TREINAMENTO ---
best_val_loss = float('inf')
best_model_state = None
train_losses, val_losses = [], []

# Identificação dinâmica dos ativos para o log (XOM, TTE)
ativos_str = ", ".join(tickers)
print(f"Iniciando Treinamento do Aglomerado...")
print(f"Device: {device} | Ativos: {ativos_str}")
print("-" * 60)

for epoch in range(1, 51):
    model_petro_eq.train()
    batch_losses = []

    # Loop de Treinamento (Processamento por lotes/batches)
    for xb, yb in train_loader:
        xb, yb = xb.to(device), yb.to(device)

        optimizer.zero_grad()
        preds = model_petro_eq(xb)

        # O MSE compara as 2 previsões da rede com os 2 preços reais do aglomerado
        loss = criterion(preds, yb)

        loss.backward()
        optimizer.step()
        batch_losses.append(loss.item())

    train_loss = np.mean(batch_losses)

    # Fase de Validação (Teste com dados não vistos no treino)
    model_petro_eq.eval()
    val_batch_losses = []
    with torch.no_grad():
        for xb, yb in test_loader:
            xb, yb = xb.to(device), yb.to(device)
            preds = model_petro_eq(xb)
            v_loss = criterion(preds, yb)
            val_batch_losses.append(v_loss.item())

    val_loss = np.mean(val_batch_losses)
    train_losses.append(train_loss)
    val_losses.append(val_loss)

    # Monitoramento do progresso por época
    print(f"Epoch {epoch:02d}/50 | Train Loss: {train_loss:.6f} | Val Loss: {val_loss:.6f}")

    # Checkpoint: Salva o estado do modelo se houver melhora na validação
    if val_loss < best_val_loss:
        best_val_loss = val_loss
        best_model_state = deepcopy(model_petro_eq.state_dict())

# Restauração do melhor estado (Best Model Weights)
if best_model_state:
    model_petro_eq.load_state_dict(best_model_state)
    print("-" * 60)
    print(f"Treinamento concluído! Menor Val Loss alcançado: {best_val_loss:.6f}")

# --- VISUALIZAÇÃO DAS CURVAS DE APRENDIZADO (LOSS) ---
plt.figure(figsize=(10, 4))
plt.plot(train_losses, label='Erro de Treino', color='forestgreen', linewidth=2)
plt.plot(val_losses, label='Erro de Validação', linestyle='--', color='royalblue', linewidth=2)
plt.title(f'Histórico de Treinamento - Aglomerado {ativos_str}', fontsize=12)
plt.xlabel('Época')
plt.ylabel('MSE Loss (Normalizado)')
plt.legend()
plt.grid(True, alpha=0.3)
plt.show()

**AVALIAÇÃO MULTIVARIADA (REAL VS. PREVISTO)**

Nesta etapa final, o modelo é testado com dados que ele nunca viu. Realizamos a **desnormalização** para converter as previsões da rede neural de volta à escala monetária original, permitindo comparar o desempenho real de** XOM** e **TTE** contra as estimativas da arquitetura híbrida.

**Destaques da Avaliação**:
- **Inversão de Escala**: A função `get_inverse_prices` reconstrói a estrutura de 8 colunas para que o `scaler` funcione corretamente, extraindo apenas os preços de fechamento.

- **Visualização Dual**: O gráfico exibe simultaneamente os dois ativos do aglomerado, facilitando a identificação de momentos onde o modelo seguiu a tendência ou falhou em capturar a volatilidade.

- **Aferição de Valor**: O resumo final no console entrega os valores exatos do último dia do conjunto de teste, facilitando uma conferência rápida.

# --- AVALIAÇÃO MULTIVARIADA: REAL VS PREVISTO (XOM & TTE) ---

model_petro_eq.eval()
all_preds = []
all_actuals = []

with torch.no_grad():
    for xb, yb in test_loader:
        xb = xb.to(device)
        out = model_petro_eq(xb) # Gera as 2 predições simultâneas
        all_preds.append(out.cpu().numpy())
        all_actuals.append(yb.numpy())

# Transformar listas de batches em arrays numpy únicos
preds_scaled = np.concatenate(all_preds, axis=0)
actuals_scaled = np.concatenate(all_actuals, axis=0)

# --- FUNÇÃO DE DESNORMALIZAÇÃO CORRIGIDA ---
def get_inverse_prices(scaled_data, scaler, target_indices):
    # Matriz dummy com o mesmo número de colunas do scaler original (8)
    dummy = np.zeros((len(scaled_data), scaler.n_features_in_))

    # Inserimos os dados nas posições originais das colunas 'Close'
    for i, idx in enumerate(target_indices):
        dummy[:, idx] = scaled_data[:, i]

    # Invertemos a escala para retornar aos valores monetários reais
    inverse = scaler.inverse_transform(dummy)

    # Retornamos apenas as colunas desnormalizadas (os preços)
    return inverse[:, target_indices]

# Obter preços finais desnormalizados para o aglomerado de petróleo
preds_final = get_inverse_prices(preds_scaled, scaler_petro_eq, target_indices)
actuals_final = get_inverse_prices(actuals_scaled, scaler_petro_eq, target_indices)

# --- PLOTAGEM DOS GRÁFICOS DE DESEMPENHO ---
tickers_label = [f"Ativo: {t}" for t in tickers]
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle(f'Avaliação do Modelo: Preço Real vs. Previsto - Petróleo ({", ".join(tickers)})', fontsize=18)

for i in range(len(tickers_label)):
    ax = axs[i]
    ax.plot(actuals_final[:, i], label='Real (Histórico)', color='forestgreen', linewidth=1.5)
    ax.plot(preds_final[:, i], label='Previsto (LSTM+GRU)', color='darkorange', linestyle='--', linewidth=1.5)

    ax.set_title(f'{tickers_label[i]}', fontsize=14)
    ax.set_ylabel('Preço de Fechamento')
    ax.set_xlabel('Dias (Conjunto de Teste)')
    ax.legend()
    ax.grid(True, alpha=0.3)

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# Print de Verificação Final
print(f"=== Resumo da Avaliação Final (Petróleo) ===")
for i, t in enumerate(tickers):
    print(f"{t}: Último Real: {actuals_final[-1, i]:.2f} | Último Previsto: {preds_final[-1, i]:.2f}")

**DIAGNÓSTICO TÉCNICO DA CAMADA DE SAÍDA**

Antes de olhar os preços finais, analisamos a **assinatura bruta** que sai da rede neural. Este diagnóstico é fundamental para identificar comportamentos anômalos, como saturação de ativação (quando o modelo prevê sempre o mesmo valor) ou volatilidade excessiva na escala normalizada $[0, 1]$.

**O que observar neste diagnóstico**:
- **Amplitude**: Se os valores `Min` e `Max` estiverem muito próximos (ex: ambos em 0.5), o modelo não aprendeu a distinguir as variações e está "chutando" a média.

- **Dinâmica**: A linha deve apresentar oscilações que lembram o comportamento de um ativo financeiro, indicando que a combinação LSTM+GRU está capturando o momentum.

- **Sincronia**: Como são ativos correlacionados (**XOM** e **TTE**), as duas saídas devem apresentar padrões de movimento visualmente similares.

# --- DIAGNÓSTICO: DISTRIBUIÇÃO DAS PREDIÇÕES (SAÍDA BRUTA DA REDE) ---

# Geramos os labels dinamicamente a partir da lista de tickers original
tickers_label = [f"Ativo: {t}" for t in tickers]
colors = ['forestgreen', 'royalblue']

# Criamos a figura com 2 subplots para diagnóstico individual (1x2)
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Diagnóstico Técnico: Assinatura de Saída da Rede (Escala 0-1)', fontsize=16)

# preds_scaled contém os valores brutos que saíram da camada Linear final do modelo
print(f"=== Relatório de Diagnóstico de Saída (Aglomerado: {', '.join(tickers)}) ===")

for i in range(len(tickers_label)):
    ax = axs[i]

    # Plotamos as primeiras 100 predições para analisar a volatilidade da predição
    ax.plot(preds_scaled[:100, i], color=colors[i], label=f'Predição {tickers[i]}', linewidth=2)

    # Cálculo de métricas estatísticas da saída normalizada (antes da desnormalização)
    p_min, p_max = preds_scaled[:, i].min(), preds_scaled[:, i].max()
    p_mean = preds_scaled[:, i].mean()

    ax.set_title(f'Distribuição: {tickers_label[i]}')
    ax.set_ylabel('Valor Normalizado (Saída da Camada Linear)')
    ax.set_xlabel('Amostra (Dias no Conjunto de Teste)')
    ax.grid(True, alpha=0.3)
    ax.legend(loc='upper right')

    # Print de diagnóstico para verificar se há colapso de gradiente ou saturação
    print(f"{tickers[i]} -> Min: {p_min:.4f} | Max: {p_max:.4f} | Média: {p_mean:.4f}")

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

**Análise dos Resultados**:

Se a média `(p_mean`) estiver por volta de 0.5 e o `min/max` cobrirem uma faixa de pelo menos 0.2, o seu modelo está saudável e capturando a variância necessária para uma boa predição.

**Análise do Diagnóstico (XOM & TTE)**
- **Variância e Amplitude (Range)**: * Para **XOM**, a amplitude é de **0.3806** ($0.9361 - 0.5555$).
  - Para **TTE**, a amplitude é de **0.4471** ($0.9012 - 0.4541$).
  - *Veredito*: Como ambas as faixas estão bem acima de **0.2**, o modelo não está "preguiçoso". Ele está reagindo ativamente às mudanças do mercado e capturando quase **40-45%** de toda a escala dinâmica possível. Isso indica que a combinação LSTM+GRU está conseguindo diferenciar dias de alta de dias de baixa com clareza.

- **Centralidade (Média)**:

  - As médias (**0.65 e 0.60**) estão ligeiramente acima de 0.5, o que é perfeitamente normal. Isso reflete apenas que, no período de teste, os ativos de petróleo provavelmente tiveram um viés de preço em patamares um pouco mais elevados dentro da janela de normalização.

- **Ausência de Colapso de Gradiente**:

  - Se os valores de *Min* e *Max* fossem muito próximos (ex: Min 0.60 | Max 0.62), o modelo estaria sofrendo de "Saturação", entregando apenas a média móvel. Com a dispersão que você obteve, confirmamos que a **camada Linear fina**l está recebendo informações ricas das camadas recorrentes.


**PROJEÇÃO RECURSIVA DE 5 DIAS (XOM & TTE)**

Nesta etapa, utilizamos o modelo treinado para projetar os preços de fechamento para os próximos 5 dias úteis. A estratégia consiste em alimentar o modelo com a última janela de 60 dias reais e, a cada passo, atualizar essa janela com as próprias predições do modelo, criando um ciclo de feedback preditivo.

**Destaques da Lógica**:
- **Alimentação Dinâmica**: A cada iteração, o modelo "empurra" a janela temporal para frente, removendo o dia mais antigo e inserindo a nova estimativa.

- **Estabilidade de Indicadores**: Ao manter indicadores técnicos constantes e atualizar apenas o preço, você reduz o efeito de "ruído acumulado", comum em previsões recursivas longas.

- **Visualização Direta**: O gráfico apresenta pontos marcados e anotados com os valores exatos, facilitando a tomada de decisão ou a análise de tendência imediata.

# --- PREVISÃO MULTIVARIADA DE 5 DIAS (RECURSIVA) ---

model_petro_eq.eval()
n_future = 5  # Projeção para os próximos 5 dias úteis
tickers_label = [f"Ativo: {t}" for t in tickers]

# 1. Capturar a última janela real de 60 dias do dataframe de petróleo
last_sequence_raw = data.tail(seq_len).values
last_scaled = scaler_petro_eq.transform(last_sequence_raw)

# Preparar o tensor de entrada inicial [1, 60, 8]
current_input = torch.tensor(last_scaled, dtype=torch.float32).unsqueeze(0).to(device)

future_preds_scaled = []

for _ in range(n_future):
    with torch.no_grad():
        # O modelo gera 2 valores (fechamentos normalizados de XOM e TTE)
        next_pred = model_petro_eq(current_input)
        pred_vals = next_pred.cpu().numpy()[0]
        future_preds_scaled.append(pred_vals)

    # 2. Atualizar a sequência para a próxima iteração (Sliding Window)
    new_entry = current_input[0, -1, :].cpu().numpy().copy()

    # Atualizamos as colunas de 'Close' com os novos valores previstos
    for i, idx in enumerate(target_indices):
        new_entry[idx] = pred_vals[i]

    # 3. Deslocar a janela temporal (Shift left e append no final)
    new_entry_tensor = torch.tensor(new_entry, dtype=torch.float32).view(1, 1, -1).to(device)
    current_input = torch.cat([current_input[:, 1:, :], new_entry_tensor], dim=1)

# --- DESNORMALIZAÇÃO DOS RESULTADOS ---
future_preds_scaled = np.array(future_preds_scaled)

def denormalize_future(scaled_data, scaler, target_indices):
    dummy = np.zeros((len(scaled_data), scaler.n_features_in_))
    for i, idx in enumerate(target_indices):
        dummy[:, idx] = scaled_data[:, i]
    inv = scaler.inverse_transform(dummy)
    return inv[:, target_indices]

future_prices = denormalize_future(future_preds_scaled, scaler_petro_eq, target_indices)

# --- PLOTAGEM DOS GRÁFICOS DE PROJEÇÃO ---
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle(f'Projeção para os Próximos {n_future} Dias - Petróleo ({", ".join(tickers)})', fontsize=18)

dias_futuros = range(1, n_future + 1)
colors_plot = ['forestgreen', 'royalblue']

for i in range(len(tickers_label)):
    ax = axs[i]
    ax.plot(dias_futuros, future_prices[:, i], marker='o', color=colors_plot[i],
            linestyle='--', linewidth=2, markersize=8)

    ax.set_title(f'Projeção: {tickers[i]}', fontsize=14)
    ax.set_ylabel('Preço Estimado')
    ax.set_xlabel('Dias úteis à frente')
    ax.set_xticks(dias_futuros)
    ax.grid(True, alpha=0.3)

    # Labels com valores exatos
    for x, y in zip(dias_futuros, future_prices[:, i]):
        ax.annotate(f'{y:.2f}', (x, y), textcoords="offset points",
                    xytext=(0,12), ha='center', fontweight='bold')

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# --- TABELA RESUMO ---
print(f"\n--- Tabela de Previsões Futuras (Petróleo: {n_future} dias) ---")
df_future = pd.DataFrame(future_prices, columns=tickers,
                         index=[f"Dia +{i+1}" for i in range(n_future)])
print(df_future.round(2))

**Persistência de Resultados (Setor de Petróleo)**

Para garantir a integridade dos dados na etapa de comparação final, realizamos o backup dos resultados desnormalizados. Isso evita que o treinamento do próximo fluxo limpe a memória do que foi conquistado aqui.

**Por que o `.copy()` é essencial?**

No Python, se você apenas igualar as variáveis (`a = b`), você cria um ponteiro (referência). Se o valor de `b` mudar no próximo bloco, `a` também mudará. O método `.copy()` do NumPy garante que os dados da Saudi Aramco e TotalEnergies sejam salvos em um novo espaço físico de memória.

# --- SALVAMENTO ESPECÍFICO DO SETOR (PETRÓLEO) ---

# Salva os resultados desnormalizados para uso futuro em comparações
# Usamos .copy() para desvincular estas variáveis do fluxo principal
preds_final_petro = preds_final.copy()
actuals_final_petro = actuals_final.copy()

print("✓ Backup de memória concluído: Resultados brutos de Petróleo preservados.")

**Blindagem de Variáveis para Correlação Final**


Nesta etapa, realizamos o "congelamento" definitivo dos dados. Variáveis dentro de loops ou fluxos repetitivos tendem a ser sobrescritas facilmente. Ao criar nomes com o sufixo `_fixed`, garantimos que o seu Dashboard final acesse os dados de Petróleo sem interferência de setores como Tecnologia ou Metais.

**Vantagens da Blindagem**:

- **Imutabilidade**: O `preds_petro_fixed` permanecerá intacto mesmo que você reinicie o modelo para outro ativo.

- **Preparação para Cross-Asset**: Com esses dados salvos separadamente, você poderá cruzar a volatilidade do Petróleo com outros setores no futuro.

# --- FINALIZAÇÃO E SALVAMENTO DE VARIÁVEIS DE CONTROLE ---

# Criamos cópias explícitas para blindagem contra sobrescrita acidental
preds_petro_fixed = preds_final.copy()
actuals_petro_fixed = actuals_final.copy()

print("-" * 60)
print("SETOR DE PETRÓLEO CONCLUÍDO E BLINDADO")
print("Resultados disponíveis em: 'preds_petro_fixed'")
print("Pronto para o próximo aglomerado ou análise de correlação.")
print("-" * 60)

### Aglomerado de Metais

**Coleta e Processamento do Setor de Metais (RIO & FCX)**

Este bloco automatiza a coleta de dados históricos e a preparação técnica dos ativos **RIO (Rio Tinto)** e **FCX (Freeport-McMoRan)**, garantindo que ambos estejam perfeitamente alinhados para o modelo.

**Destaques da Execução**:
- **Sincronização NYSE**: Como ambos os ativos rodam no mesmo calendário (NYSE), o código garante que não existam datas "descasadas" entre as duas empresas.

- **Limpeza de Estrutura**: Resolve o problema de colunas duplicadas ou complexas que o Yahoo Finance gera ao baixar múltiplos tickers simultaneamente.

- **Enriquecimento de Dados**: Não utiliza apenas o preço de fechamento, mas injeta **Médias Móveis (SMA/EMA)** e **RSI** como variáveis auxiliares para ajudar a IA a entender a tendência e a força do mercado.

- **Tratamento de Lacunas**: Utiliza o `ffill()` (Forward Fill) para que feriados isolados ou falhas na transmissão de dados não interrompam a série temporal, mantendo a continuidade necessária para redes neurais.

- **Mapeamento de Alvos**: Define automaticamente quais colunas o modelo deve tentar "prever" (os preços de fechamento), separando-as das colunas que servem apenas como "dicas" (indicadores).

## Aglomerado de Metais (Mercados Ocidentais - NYSE)

# RIO (Rio Tinto) e FCX (Freeport-McMoRan) operam no mesmo calendário
tickers = ['RIO', 'FCX']
dfs = []

for t in tickers:
    # Coleta de dados
    df_raw = yf.download(t, start='2019-01-01', end='2026-03-22', progress=False)

    if df_raw.empty:
        print(f"Erro: Dados não encontrados para {t}")
        continue

    # TRATAMENTO SEGURO DE COLUNAS:
    if isinstance(df_raw.columns, pd.MultiIndex):
        df = df_raw['Close'][[t]].copy()
    else:
        df = df_raw[['Close']].copy()

    # Renomeação consistente
    col_name = f'{t}_Close'
    df.columns = [col_name]

    # Aplicação dos indicadores (SMA, EMA, RSI)
    df = add_indicators(df, col=col_name, window=14)
    dfs.append(df)

# Concatenagem com Forward Fill para cobrir eventuais feriados isolados
data = pd.concat(dfs, axis=1).ffill().dropna()

# Mapeamento de colunas alvo
target_cols = [col for col in data.columns if 'close' in col.lower()]
target_indices = [data.columns.get_loc(c) for c in target_cols]

print(f"=== Aglomerado de Metais (Mesmo Mercado) ===")
print(f"Shape final: {data.shape}")
print(f"Colunas: {data.columns.tolist()}")
data.tail()

**Normalização de Dados Multivariados (Escalonamento)**

Este bloco é fundamental para o desempenho de redes neurais (como LSTM e GRU). Ele transforma todos os valores brutos (preços e indicadores) para uma escala comum.

**O que está acontecendo no código**:

1. **Instanciação do MinMaxScaler**: O código utiliza o `MinMaxScaler()`, que é uma ferramenta estatística que comprime todos os dados do DataFrame original para um intervalo fixo (por padrão, entre 0 e 1).

2. **Ajuste e Transformação (`fit_transform`)**: * Fit: O "escalonador" analisa o valor mínimo e o valor máximo de cada uma das 8 colunas (Preços, SMAs, EMAs e RSIs de RIO e FCX).

- **Transform**: Ele aplica a fórmula matemática para converter os valores reais em decimais.

3. **Renomeação Estruturada**: Ao renomear a saída para scaled_metais, garantimos que, se você rodar vários aglomerados no mesmo notebook, os dados de "Metais" não sobrescrevam os dados de "Petróleo" ou outros setores.

**Por que isso é necessário?**

Redes neurais são sensíveis à escala. Se um preço é **$60.00** e o RSI é **70.0**, a rede pode achar que o RSI é mais importante apenas por ser um número maior. A normalização coloca todos na "mesma importância", facilitando a convergência e o aprendizado do modelo.

# --- NORMALIZAÇÃO DOS DADOS (AGLOMERADO DE METAIS) ---

# Instancia o escalonador para colocar todos os dados na mesma escala (0 a 1)
scaler_metais = MinMaxScaler()

# Ajusta o scaler aos dados reais e transforma em valores normalizados
# Renomeamos para 'scaled_metais' para evitar conflitos com outros aglomerados
scaled_metais = scaler_metais.fit_transform(data)

**Lógica de Janelas Deslizantes (Sliding Windows)**

Este bloco define o "cérebro" da preparação dos dados. Ele transforma uma tabela estática em uma sequência temporal que a Inteligência Artificial consegue entender como um histórico que leva a uma previsão.

**O que está acontecendo no código**:

1. **Criação de Sequências Multivariadas**: Diferente de modelos simples, esta função lida com múltiplas variáveis ao mesmo tempo (Preços + Indicadores de RIO e FCX). Ela organiza os dados para que o modelo aprenda a relação entre todos esses fatores.

2. **A Janela Histórica (`X`)**: * O código seleciona um bloco de dados (ex: os últimos 60 dias).

- Este bloco contém **todas as informações** (as 8 colunas: Close, SMA, EMA, RSI de ambos os ativos).

- É o que o modelo usará para "olhar para trás" antes de tomar uma decisão.

3. **O Alvo da Previsão (`y`)**:

- Enquanto `X` olha para o passado, `y` captura o valor real do **dia seguinte**.

- Utilizando os `target_indices` mapeados no Bloco 1, a função extrai apenas os preços de fechamento. Ou seja, o modelo estuda 8 colunas para tentar prever apenas 2 (os preços de RIO e FCX).

4. **Estrutura de Saída (NumPy Arrays)**:

- Ao final, os dados são convertidos em arrays NumPy. Isso é essencial para que o PyTorch consiga transformar essas informações em "Tensores" (o formato matemático usado no treinamento) nos blocos seguintes.

# --- DEFINIÇÃO DA FUNÇÃO DE SEQUENCIAMENTO TEMPORAL ---

def create_multivariate_sequences(data, seq_len, target_indices):
    """
    Transforma dados tabulares em janelas deslizantes (Sliding Windows)
    para o treinamento de modelos de séries temporais (LSTM/GRU).
    """
    X, y = [], []

    # Garantimos que os dados sejam tratados como um array NumPy para fatiamento
    data_array = np.array(data)

    # O loop percorre os dados a partir do tamanho da janela (ex: 60 dias)
    for i in range(seq_len, len(data_array)):
        # X: Janela histórica com todas as colunas (Preços e Indicadores Técnicos)
        # Captura as linhas de [i-seq_len] até [i-1]
        X.append(data_array[i-seq_len:i, :])

        # y: Os valores de fechamento (Target) de AMBOS os ativos no dia exato 'i'
        # A sintaxe [i, target_indices] extrai apenas as colunas de 'Close' desejadas
        y.append(data_array[i, target_indices])

    return np.array(X), np.array(y)

**Preparação das Matrizes e Divisão Cronológica**

Este bloco executa a separação final dos dados que serão usados para "ensinar" a rede neural e os dados que serão usados para "testar" se ela realmente aprendeu.

**O que está acontecendo no código**:
1. **Aplicação da Janela Móvel**: O código utiliza a função criada no bloco anterior para transformar os dados normalizados (`scaled_metais`) em grandes blocos 3D. Cada bloco contém **60 dias** de histórico.

2. **Divisão Estratégica (80/20)**:

- **Treino (80%)**: O modelo usa essa fatia para ajustar seus pesos internos e entender os padrões de preços da RIO e FCX.

- **Teste (20%)**: São os dados mais recentes. O modelo nunca viu esses dados durante o treino, servindo como uma "prova final" para validar sua precisão.

3. **Respeito à Linha do Tempo**: Diferente de outros modelos de IA onde os dados podem ser embaralhados, aqui a divisão é **estritamente cronológica**. Não podemos treinar com dados de 2025 para prever 2024; isso causaria um erro grave de lógica conhecido como "olhar o futuro" (*Data Leakage*).

4. **Análise das Dimensões (O que os números significam)**:

- **X_train (N, 60, 8)**: Significa que temos `N` sequências, cada uma com **60 dias** de duração, contendo **8 informações** simultâneas (Preço, SMA, EMA e RSI de cada um dos 2 ativos).

- **y_train (N, 2)**: Significa que para cada sequência de 60 dias, o modelo tentará prever **2 resultados**: o preço de fechamento da Rio Tinto e o da Freeport-McMoRan.

# --- GERAÇÃO DE SEQUÊNCIAS E DIVISÃO DE DADOS (TREINO/TESTE) ---

# 1. Configuração da janela temporal (60 dias de histórico para prever o próximo)
seq_len = 60
X, y = create_multivariate_sequences(scaled_metais, seq_len, target_indices)

# 2. Divisão treino/teste (Cronológica: 80% treino, 20% teste)
# Em séries temporais, mantemos a ordem dos dados para evitar o "vazamento de dados" (Data Leakage).
split = int(0.8 * len(X))
X_train, X_test = X[:split], X[split:]
y_train, y_test = y[:split], y[split:]

# 3. Verificação de dimensões para o Aglomerado de Metais:
print("=== Verificação de Dimensões (Aglomerado de Metais) ===")
print(f"X_train shape: {X_train.shape}") # Esperado: (Amostras, 60, 8)
print(f"y_train shape: {y_train.shape}") # Esperado: (Amostras, 2) -> Alvos: RIO e FCX

**Estruturação do Dataset para PyTorch**

Este bloco cria a "ponte" entre os dados que preparamos no NumPy e o motor de processamento do PyTorch. Sem essa estrutura, a rede neural não conseguiria ler as janelas de tempo de forma eficiente.

**O que está acontecendo no código**:
1. **Conversão para Tensores**:

- O PyTorch não trabalha diretamente com arrays comuns; ele exige **Tensores**. O código converte os preços e indicadores para `torch.float32`, garantindo alta precisão matemática e compatibilidade total com aceleração por hardware (GPU/CUDA).

2. **Método Especial** `__len__`:
Informa ao sistema exatamente quantas sequências de 60 dias existem para o aglomerado de metais. Isso ajuda o algoritmo de treinamento a saber quando uma "época" (uma volta completa nos dados) terminou.

3. **Método Especial** `__getitem__`:
Funciona como um sistema de indexação. Quando o modelo pede "me dê a amostra 50", este método entrega a 50ª janela de 60 dias (`X`) e o respectivo preço de fechamento do dia seguinte (`y`).

# --- CRIAÇÃO DA ESTRUTURA DE DATASET (PYTORCH) ---

class TimeSeriesDataset(Dataset):
    """
    Classe customizada que herda de 'Dataset' do PyTorch.
    Sua função é converter os arrays NumPy em Tensores e organizar
    o acesso aos dados durante o treinamento.
    """
    def __init__(self, X, y):
        # Converte as matrizes X e y para tensores de ponto flutuante (float32)
        # O float32 é o padrão ouro para processamento em GPUs e redes neurais.
        self.X = torch.tensor(X, dtype=torch.float32)
        self.y = torch.tensor(y, dtype=torch.float32)

    def __len__(self):
        # Retorna o número total de amostras (janelas de 60 dias) no dataset
        return len(self.X)

    def __getitem__(self, idx):
        # Permite que o DataLoader busque uma amostra específica (X) e seu alvo (y)
        # através de um índice, facilitando o sorteio de lotes (batches).
        return self.X[idx], self.y[idx]

**Orquestração de Lotes (DataLoaders)**

Este bloco é o estágio final da preparação de dados. Ele define como as janelas de tempo serão "servidas" para a rede neural durante o processo de aprendizagem.

**O que está acontecendo no código**:

1. **Criação dos Objetos Dataset**: O código aplica a estrutura `TimeSeriesDataset` (definida no Bloco 5) tanto para os dados de **Treino** (80%) quanto para os de **Test**e (20%), transformando-os em objetos prontos para o PyTorch.

2. **Definição do Batch Size (32)**: O modelo não tenta aprender com todos os dados de uma vez (o que travaria a memória) nem um por um (o que seria muito lento). Ele processa 32 sequências simultaneamente. Esse é um equilíbrio padrão para estabilidade e velocidade.

3. **Shuffle (Embaralhamento no Treino)**: `shuffle=True`: No treino, embaralhamos as janelas. Isso força o modelo a aprender o **padrão técnico** (Ex: "Se o RSI subir e a média cruzar, o preço sobe") em vez de simplesmente "decorar" que a segunda-feira vem depois do domingo.

4. **Estabilidade no Teste**:
No `test_loader`, o embaralhamento é desligado. Isso é importante para que, ao final, possamos plotar um gráfico de previsão que siga a linha do tempo real, permitindo comparar a previsão da IA com o preço real de mercado de forma sequencial.

# --- INSTANCIAÇÃO DOS DATALOADERS (LOTES DE TREINO E TESTE) ---

# 1. Instanciamos a classe Dataset criada no bloco anterior
train_ds = TimeSeriesDataset(X_train, y_train)
test_ds = TimeSeriesDataset(X_test, y_test)

# 2. Criamos os DataLoaders para gerenciar a entrega dos dados ao modelo
# 'batch_size=32' significa que o modelo verá 32 janelas de 60 dias por vez.
# 'shuffle=True' embaralha os dados de treino para evitar que a rede decore a ordem.
train_loader = DataLoader(train_ds, batch_size=32, shuffle=True)

# No conjunto de teste, não embaralhamos (shuffle=False por padrão)
# para manter a ordem cronológica da avaliação final.
test_loader = DataLoader(test_ds, batch_size=32)

print(f"=== Configuração de Lotes (Batches) ===")
print(f"Número de lotes no Treino: {len(train_loader)}")
print(f"Número de lotes no Teste: {len(test_loader)}")

**Inspeção Visual e Auditoria Estatística**

Este bloco atua como um "controle de qualidade". Antes de iniciar o treinamento pesado, verificamos se os dados foram processados corretamente e se a normalização preservou o comportamento do mercado.

**O que está acontecendo no código**:

1. **Identidade Visual**: O código atribui cores temáticas (Azul Marinho para o gigante do minério Rio Tinto e Bronze para a mineradora de cobre Freeport) para facilitar a distinção visual nos gráficos de desempenho.

2. **Análise de Séries Temporais (Subplots)**:

Ele gera dois gráficos independentes para comparar o comportamento dos alvos (`y_train`).

Ao observar as primeiras **100 amostras**, conseguimos identificar visualmente se existem ruídos anormais ou se as curvas de preço mantêm sua natureza fluida mesmo após a normalização.

3. **Auditoria de Escala (0 a 1)**:

- O código imprime o valor **Mínimo**, **Máximo** e a **Média** de cada ativo no conjunto de treino.

- **O objetivo técnico**: Garantir que os dados estejam bem distribuídos entre 0 e 1. Se o máximo for `1.0000` e o mínimo `0.0000`, o scaler funcionou perfeitamente. Se os valores estivessem muito próximos (ex: tudo 0.5), o modelo teria dificuldade em aprender.

# --- VISUALIZAÇÃO E VALIDAÇÃO DOS ALVOS (Y_TRAIN) ---

# 1. Ajuste dos Tickers e Identidade Visual (Metais)
# Definimos nomes amigáveis e cores representativas: Azul (RIO) e Bronze/Cobre (FCX)
tickers_label = ['Rio Tinto (RIO)', 'Freeport-McMoRan (FCX)']
colors = ['#003366', '#B87333']

# 2. Criação da Visualização (2 Subplots para análise individual)
fig, axs = plt.subplots(1, 2, figsize=(15, 6))
fig.suptitle('Distribuição dos Alvos de Metais - Primeiras 100 Amostras (y_train Normalizado)', fontsize=16)

# Loop pelos 2 alvos do aglomerado (RIO e FCX)
for i in range(len(tickers_label)):
    ax = axs[i]
    # Plota as primeiras 100 amostras do conjunto de treino
    # O eixo Y representa o valor de fechamento (Close) na escala normalizada (0 a 1)
    ax.plot(y_train[:100, i], color=colors[i], label='Target Normalizado', linewidth=2.5)

    ax.set_title(f'Série Temporal: {tickers_label[i]}')
    ax.set_xlabel('Sequência de Amostras (Tempo)')
    ax.set_ylabel('Valor (Escala 0 a 1)')
    ax.grid(True, linestyle='--', alpha=0.5)
    ax.legend(loc='upper right')

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# 3. Conferência Estatística do Aglomerado de Metais
# Validação fundamental para garantir que o Scaler não saturou os dados
print("=== Conferência Técnica: Aglomerado de Metais (RIO & FCX) ===")
for i, ticker in enumerate(tickers_label):
    print(f"{ticker}:")
    print(f"   > Mínimo: {y_train[:, i].min():.4f}")
    print(f"   > Máximo: {y_train[:, i].max():.4f}")
    print(f"   > Média:  {y_train[:, i].mean():.4f}")
    print("-" * 45)

**O Coração da IA - Arquitetura Híbrida**

Este bloco define a estrutura do modelo. Ele utiliza uma técnica avançada que combina duas das arquiteturas mais poderosas para séries temporais: **LSTM** e **GRU**.

**O que está acontecendo no código**:

1. **Camada LSTM (Long Short-Term Memory)**:

- É a primeira a processar os dados. Ela possui "portões de esquecimento" que permitem memorizar tendências que duram meses, ignorando variações irrelevantes do dia a dia.

- Ela recebe as **8 características** (preços e indicadores) e as transforma em uma representação complexa de **64 neurônios**.

2. **Camada GRU (Gated Recurrent Unit)**:

- Recebe a saída da LSTM. A GRU é conhecida por ser mais eficiente e rápida para captar mudanças bruscas de curto prazo (volatilidade).

- Ela "peneira" os 64 sinais da LSTM e entrega apenas **32 sinais** altamente relevantes.

3. **Lógica "Many-to-One"**:

- Embora o modelo receba uma sequência de 60 dias, o código seleciona apenas o estado final (`out_gru[:, -1, :]`).

- Isso significa: "Use todo o contexto dos últimos 60 dias para tomar uma única decisão sobre o preço de amanhã".

4. **Camada de Saída (Linear)**:

- É a camada final que traduz o pensamento da rede neural em valores numéricos. Ela mapeia os 32 sinais internos para as **2 saídas** desejadas: o preço da Rio Tinto e o da Freeport-McMoRan.

# --- ARQUITETURA HÍBRIDA DA REDE NEURAL (LSTM + GRU) ---

class LSTM_GRU_Model(nn.Module):
    def __init__(self, input_size, hidden_lstm=64, hidden_gru=32, output_size=2):
        super().__init__()

        # 1. Camada LSTM: Identifica ciclos longos (tendências de meses)
        # Recebe 8 entradas (4 de RIO + 4 de FCX) e expande para 64 sinais internos
        self.lstm = nn.LSTM(input_size=input_size,
                            hidden_size=hidden_lstm,
                            batch_first=True)

        # 2. Camada GRU: Refina o aprendizado focando na volatilidade de curto prazo
        # Recebe os 64 sinais da LSTM e condensa em 32, filtrando ruídos rápidos
        self.gru = nn.GRU(input_size=hidden_lstm,
                          hidden_size=hidden_gru,
                          batch_first=True)

        # 3. Camada de Saída (Totalmente Conectada / Linear)
        # Transforma os 32 neurônios da GRU nas 2 previsões finais de preço
        self.fc = nn.Linear(hidden_gru, output_size)

    def forward(self, x):
        # Fluxo de dados (Forward Pass)

        # Passagem pela LSTM: Extração de padrões de longo prazo
        out_lstm, _ = self.lstm(x)

        # Passagem pela GRU: Refinamento com foco em movimentos recentes
        out_gru, _ = self.gru(out_lstm)

        # Seleção do estado final (Lógica Many-to-One)
        # Capturamos apenas a saída do último dia da janela de 60 dias (índice -1)
        # Isso resume todo o histórico em um único vetor de decisão
        last_time_step = out_gru[:, -1, :]

        # Projeção final para os 2 alvos: [RIO_Close, FCX_Close]
        final_output = self.fc(last_time_step)

        return final_output

**Setup de Otimização e Controle de Hardware**

Este bloco prepara o "terreno" onde o modelo será treinado. Ele define as regras matemáticas de aprendizado e garante que o código utilize o máximo de poder de processamento disponível.

# --- CONFIGURAÇÃO DO AMBIENTE DE TREINAMENTO E HARDWARE ---

# 1. Detecção Automática de Features (Aglomerado de Metais)
# O input_size captura as 8 colunas (4 da Rio Tinto + 4 da Freeport-McMoRan)
# Colunas: [Close, SMA, EMA, RSI] x 2 ativos
input_size = X_train.shape[2]

# 2. Definição do Hardware (Aceleração por GPU/CUDA se disponível)
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")

# 3. Inicialização do Modelo Híbrido (LSTM + GRU)
# O output_size=2 garante a previsão simultânea da Rio Tinto (RIO) e da Freeport (FCX)
model = LSTM_GRU_Model(input_size=input_size, output_size=2).to(device)

# 4. Função de Perda: MSE (Mean Squared Error)
# Ideal para commodities metálicas: penaliza severamente erros grandes,
# forçando a rede a capturar movimentos bruscos de volatilidade no setor mineral.
criterion = nn.MSELoss()

# 5. Otimizador: Adam (Adaptive Moment Estimation)
# Taxa de aprendizado (LR) de 0.001. O Adam ajusta o gradiente para cada
# peso individualmente, sendo o padrão ouro para lidar com ruído em séries temporais.
optimizer = torch.optim.Adam(model.parameters(), lr=0.001)

# Verificação de Segurança
print(f"=== Setup de Treinamento (Metais) ===")
print(f"Dispositivo: {device}")
print(f"Features de Entrada: {input_size}")
print(f"Targets de Saída: 2 (RIO e FCX)")

**Execução do Treinamento e Curvas de Convergência**

Este bloco é o motor principal. Ele executa o aprendizado iterativo da rede neural e implementa uma técnica de segurança para garantir que fiquemos com a melhor versão possível do modelo.

**O que está acontecendo no código**:

1. **O Ciclo de 50 Épocas**:
O modelo passa 50 vezes por todos os dados de treino. A cada passagem, ele tenta prever os preços, calcula o erro e ajusta seus pesos internos através do `loss.backward()` (Backpropagation).

2. **Separação Treino vs. Validação**:

- **Fase de Treino (`model.train()`)**: A rede está "ativa" e aprendendo.

- **Fase de Validação (`model.eval()`)**: A rede é testada com dados que ela não usou para ajustar pesos. O `torch.no_grad()` desativa os cálculos de gradiente, economizando memória e garantindo que o teste seja justo.

3. **Estratégia de Checkpoint (`deepcopy`)**:
É comum que, após muitas épocas, o modelo comece a "decorar" o passado (Overfitting) e piore sua performance no futuro. O código monitora o erro de validação e salva uma "foto" (`best_model_state`) sempre que o erro atinge a mínima histórica. Ao final, ele restaura essa melhor versão.

4. **Visualização da Convergência**:
O gráfico gerado ao final é vital.

- Se ambas as curvas descem juntas, o modelo está aprendendo bem.

- Se a curva de treino desce e a de validação sobe, houve overfitting.

# --- CICLO DE TREINAMENTO COM CHECKPOINT (EARLY SAVING) ---

from copy import deepcopy

# 1. Configuração Inicial e Reset de Métricas
best_val_loss = float('inf')
best_model_state = None
train_losses, val_losses = [], []

print("Iniciando Treinamento do Aglomerado de Metais...")
print(f"Hardware: {device} | Ativos: Rio Tinto (RIO) e Freeport-McMoRan (FCX)")
print("-" * 70)

# Loop de 50 Épocas (Iterações completas sobre o dataset)
for epoch in range(1, 51):
    # --- FASE DE TREINO ---
    model.train()
    batch_losses = []

    for xb, yb in train_loader:
        xb, yb = xb.to(device), yb.to(device)

        optimizer.zero_grad()
        preds = model(xb)

        # O MSE calcula o erro simultâneo para RIO e FCX
        loss = criterion(preds, yb)

        loss.backward()
        optimizer.step()

        batch_losses.append(loss.item())

    train_loss = np.mean(batch_losses)

    # --- FASE DE VALIDAÇÃO (TESTE) ---
    model.eval()
    val_batch_losses = []

    with torch.no_grad():
        for xb, yb in test_loader:
            xb, yb = xb.to(device), yb.to(device)
            preds = model(xb)
            v_loss = criterion(preds, yb)
            val_batch_losses.append(v_loss.item())

    val_loss = np.mean(val_batch_losses)
    train_losses.append(train_loss)
    val_losses.append(val_loss)

    # LOG DE PROGRESSO
    print(f"Epoch {epoch:02d}/50 | Erro Treino: {train_loss:.6f} | Erro Validação: {val_loss:.6f}")

    # 2. Checkpoint do melhor modelo
    if val_loss < best_val_loss:
        best_val_loss = val_loss
        best_model_state = deepcopy(model.state_dict())

# 3. Restauração do melhor estado (Evita Overfitting)
if best_model_state:
    model.load_state_dict(best_model_state)
    print("-" * 70)
    print(f"Treinamento Concluído! Melhor Erro de Validação: {best_val_loss:.6f}")

# 4. Gráfico das Curvas de Aprendizado
plt.figure(figsize=(12, 5))
plt.plot(train_losses, label='Erro de Treino (RIO/FCX)', color='#003366', linewidth=2)
plt.plot(val_losses, label='Erro de Validação (RIO/FCX)', linestyle='--', color='#B87333', linewidth=2)
plt.title('Curvas de Convergência - Setor de Metais (LSTM+GRU)', fontsize=14)
plt.xlabel('Época')
plt.ylabel('MSE Loss (Normalizado)')
plt.legend()
plt.grid(True, alpha=0.3)
plt.show()

**Tradução de Resultados e Confronto Real vs. Modelo**

Este bloco é o momento da verdade. Ele converte os números decimais abstratos (0 a 1) de volta para valores monetários em dólares (**USD**) e coloca as previsões da IA lado a lado com os preços reais.

**O que está acontecendo no código**:

1. **Inferência Final**: O modelo entra em modo de avaliação (`eval()`) e processa todo o conjunto de teste. Ele gera previsões simultâneas para a **Rio Tinto** e para a **Freeport-McMoRan**.

2. **O Desafio da Desnormalização (`get_inverse_prices`)**:
Como o modelo foi treinado com dados escalonados, ele prevê valores como `0.456`. Para saber se isso significa **$60.00** ou **$65.00**, o código cria uma matriz "fantasma" (dummy) que imita a estrutura original de 8 colunas, insere os resultados nos lugares certos e usa o `scaler.inverse_transform`.

3. **Visualização Comparativa**:

- **Linha Sólida Azul**: Representa o que realmente aconteceu no mercado durante o período de teste.

- **Linha Pontilhada Bronze**: Representa a "aposta" feita pela arquitetura híbrida LSTM+GRU.

4. **Análise Setorial**: Ao plotar os dois ativos lado a lado, você consegue visualizar se o modelo capturou a **correlação** entre eles (ex: se ambos subiram juntos devido a uma alta no preço do minério de ferro ou cobre).

# --- DESNORMALIZAÇÃO E AVALIAÇÃO VISUAL (REAL VS. PREVISTO) ---

# 1. Avaliação Multivariada: Real vs Previsto para as 2 ações de Metais
model.eval()
all_preds = []
all_actuals = []

with torch.no_grad():
    for xb, yb in test_loader:
        xb = xb.to(device)
        out = model(xb) # Gera as 2 predições simultâneas (RIO e FCX)
        all_preds.append(out.cpu().numpy())
        all_actuals.append(yb.numpy())

# Transformar listas de batches em arrays numpy únicos
preds_scaled = np.concatenate(all_preds, axis=0)
actuals_scaled = np.concatenate(all_actuals, axis=0)

# --- Função de Desnormalização para Aglomerado de Metais ---
def get_inverse_prices(scaled_data, scaler, target_indices):
    # Criamos uma matriz "fantasma" com o shape original (8 colunas)
    n_features = scaler.n_features_in_
    dummy = np.zeros((len(scaled_data), n_features))

    # Preenchemos apenas as colunas de fechamento (Close) nos índices corretos
    # target_indices mapeia onde estão 'RIO_Close' e 'FCX_Close' no scaler
    for i, col_idx in enumerate(target_indices):
        dummy[:, col_idx] = scaled_data[:, i]

    # Inverte a escala para voltar aos valores monetários reais (Dólares)
    inverse = scaler.inverse_transform(dummy)

    # Extraímos apenas os preços desnormalizados das colunas alvo
    return inverse[:, target_indices]

# Obter preços finais (Desnormalizados para USD)
# IMPORTANTE: Use o scaler_metais definido no Bloco 2
preds_final = get_inverse_prices(preds_scaled, scaler_metais, target_indices)
actuals_final = get_inverse_prices(actuals_scaled, scaler_metais, target_indices)

# --- Plotagem dos 2 Gráficos de Metais ---
tickers_label = ['Rio Tinto (RIO)', 'Freeport-McMoRan (FCX)']
units = ['USD', 'USD']
colors_real = ['#003366', '#003366'] # Azul Marinho para o histórico (Real)
colors_pred = ['#B87333', '#B87333'] # Bronze para a previsão (LSTM+GRU)

fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Avaliação do Modelo: Preço Real vs. Previsto - Setor de Metais (RIO & FCX)', fontsize=18)

for i in range(len(tickers_label)):
    ax = axs[i]
    # Plotagem dos dados reais
    ax.plot(actuals_final[:, i], label='Preço Real (Histórico)', color=colors_real[i], alpha=0.7, linewidth=2)

    # Plotagem das previsões do modelo
    ax.plot(preds_final[:, i], label='Previsão LSTM+GRU', color=colors_pred[i], linestyle='--', linewidth=1.5)

    ax.set_title(f'Ativo: {tickers_label[i]}', fontsize=14)
    ax.set_ylabel(f'Preço de Fechamento ({units[i]})')
    ax.set_xlabel('Tempo (Dias no Conjunto de Teste)')
    ax.legend()
    ax.grid(True, alpha=0.3)

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# Resumo Final de Erro (Opcional para conferência rápida)
print(f"=== Resumo de Avaliação: {', '.join(tickers_label)} ===")
for i, ticker in enumerate(tickers_label):
    last_real = actuals_final[-1, i]
    last_pred = preds_final[-1, i]
    print(f"{ticker}: Último Real: ${last_real:.2f} | Último Previsto: ${last_pred:.2f}")

**Diagnóstico de "Assinatura" e Saúde da Rede**

Este bloco realiza uma autópsia técnica nos resultados antes deles serem convertidos para dólares. O objetivo é entender como a rede neural está "pensando" e se ela não caiu em armadilhas comuns de modelos matemáticos.

**O que está acontecendo no código**:
1. **Análise da "Assinatura" de Saída**:
Ao plotar os valores normalizados (`preds_scaled`), observamos a fluidez da previsão. Se a linha fosse reta ou apresentasse degraus artificiais, teríamos um sinal de que o modelo "travou". Como estamos lidando com metais (RIO e FCX), esperamos ver uma oscilação que reflita a natureza volátil dessas ações.

2. **Monitoramento de Saturação**:
O relatório no console verifica a **Amplitude** (mínimo e máximo).

- **Se os valores estiverem presos em 0 ou 1**: Indica que os neurônios "saturaram" (morreram), e o modelo parou de aprender.

- **Se a amplitude for saudável (ex: entre 0.2 e 0.8)**: Significa que a rede está operando em uma zona de alta sensibilidade, captando nuances do mercado.

3. **Desvio Padrão e Estabilidade**:

- O código calcula o desvio padrão das predições. Isso nos diz se a rede está sendo muito conservadora (prevendo sempre a média) ou se está conseguindo "ousar" para captar os picos e vales dos preços da Rio Tinto e Freeport-McMoRan.

# --- DIAGNÓSTICO TÉCNICO DA ASSINATURA DE SAÍDA ---

# 1. Configuração de Identidade Visual (Aglomerado de Metais)
tickers_label = ['Rio Tinto (RIO)', 'Freeport-McMoRan (FCX)']
colors = ['#003366', '#B87333'] # Azul RIO e Bronze FCX

# 2. Criação da Visualização de Diagnóstico (2 Subplots)
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle('Diagnóstico Técnico: Assinatura de Saída da Rede (Metais - Escala 0-1)', fontsize=16)

print("=== Relatório de Diagnóstico de Saída (Escala 0-1) - Metais (RIO & FCX) ===")

for i in range(len(tickers_label)):
    ax = axs[i]

    # Plotamos as primeiras 100 predições para observar a "assinatura" e volatilidade da rede
    # 'preds_scaled' contém os valores brutos que saíram da camada Linear final do modelo
    ax.plot(preds_scaled[:100, i], color=colors[i], label=f'Predição {tickers_label[i]}', linewidth=2)

    # 3. Cálculo de métricas estatísticas da saída normalizada
    p_min, p_max = preds_scaled[:, i].min(), preds_scaled[:, i].max()
    p_mean = preds_scaled[:, i].mean()
    p_std = preds_scaled[:, i].std()

    ax.set_title(f'Distribuição: {tickers_label[i]}')
    ax.set_ylabel('Valor Normalizado (Saída da Camada Linear)')
    ax.set_xlabel('Amostra (Dias no Conjunto de Teste)')
    ax.grid(True, linestyle='--', alpha=0.5)
    ax.legend(loc='upper right')

    # Relatório técnico no console para verificar saúde dos gradientes
    print(f"{tickers_label[i]}:")
    print(f"   > Amplitude: {p_min:.4f} até {p_max:.4f}")
    print(f"   > Média: {p_mean:.4f} | Desvio Padrão: {p_std:.4f}")
    print("-" * 60)

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

**Projeção Futura e Mecanismo de Recursão**

Este é o estágio final, onde o modelo deixa de olhar para o passado e passa a gerar conhecimento novo, estimando os preços para os próximos 5 dias úteis.

**O que está acontecendo no código**:
1. **Lógica Auto-regressiva (Recursão)**:
Como não temos os dados reais do "amanhã", o modelo usa sua própria previsão como entrada para o dia seguinte. Ele "chuta" o preço de T+1, anexa esse valor à janela de 60 dias e descarta o dia mais antigo, criando um ciclo de previsão contínuo.

2. **Manutenção de Indicadores**:
Durante os 5 dias de projeção, o código mantém os indicadores técnicos (RSI, Médias) estáveis. Isso é uma estratégia de **estabilidad**e: recalcular indicadores sobre previsões pode causar um efeito "bola de neve" de erros. Focar apenas na variação do preço protege a integridade da tendência.

3. **Visualização "T+n"**:
O gráfico apresenta pontos marcados e valores anotados, permitindo uma leitura rápida da tendência (Alta, Baixa ou Lateralização) para a Rio Tinto e a Freeport-McMoRan de forma independente, mas baseada no mesmo contexto de mercado.

4. **Resumo Executivo**:
A tabela final consolida os valores em dólares, oferecendo uma visão clara e organizada para tomada de decisão ou relatórios de análise técnica.

# --- PREVISÃO MULTIVARIADA DE 5 DIAS ÚTEIS (PROJEÇÃO T+5) ---

model.eval()
n_future = 5  # Projeção para a próxima semana útil
tickers_label = ['Rio Tinto (RIO)', 'Freeport-McMoRan (FCX)']
moedas = ['USD', 'USD']
colors_plot = ['#003366', '#B87333'] # Azul RIO e Bronze FCX

# 1. Preparação da última janela real disponível (Lookback de 60 dias)
# Usamos o scaler_metais para garantir a escala correta do aglomerado
last_sequence_raw = data.tail(seq_len).values
last_scaled = scaler_metais.transform(last_sequence_raw)

# Tensor inicial: Shape [1, 60, 8] enviado para o dispositivo (CPU/GPU)
current_input = torch.tensor(last_scaled, dtype=torch.float32).unsqueeze(0).to(device)

future_preds_scaled = []

for _ in range(n_future):
    with torch.no_grad():
        # O modelo prevê os 2 fechamentos simultaneamente (Multivariado)
        next_pred = model(current_input)
        pred_vals = next_pred.cpu().numpy()[0] # [Pred_RIO, Pred_FCX]
        future_preds_scaled.append(pred_vals)

    # 2. Mecanismo de Recursão (Sliding Window Auto-regressiva)
    # Criamos a entrada para o "amanhã" baseada na previsão de "hoje"
    new_entry = current_input[0, -1, :].cpu().numpy().copy()

    # Atualizamos apenas as colunas de FECHAMENTO (target_indices) com as novas predições
    for i, idx in enumerate(target_indices):
        new_entry[idx] = pred_vals[i]

    # 3. Deslocamento da Janela: Removemos o dia T-60 e adicionamos o T+1 previsto
    new_entry_tensor = torch.tensor(new_entry, dtype=torch.float32).view(1, 1, -1).to(device)
    current_input = torch.cat([current_input[:, 1:, :], new_entry_tensor], dim=1)

# --- DESNORMALIZAÇÃO PARA VALORES MONETÁRIOS REAIS ---
future_preds_scaled = np.array(future_preds_scaled)

def denormalize_future(scaled_data, scaler, target_indices):
    n_features = scaler.n_features_in_
    dummy = np.zeros((len(scaled_data), n_features))
    for i, idx in enumerate(target_indices):
        dummy[:, idx] = scaled_data[:, i]
    inv = scaler.inverse_transform(dummy)
    return inv[:, target_indices]

future_prices = denormalize_future(future_preds_scaled, scaler_metais, target_indices)

# --- PLOTAGEM DAS PROJEÇÕES LADO A LADO ---
fig, axs = plt.subplots(1, 2, figsize=(16, 6))
fig.suptitle(f'Projeção do Setor de Metais para os Próximos {n_future} Dias Úteis (T+5)', fontsize=18)

dias_futuros = range(1, n_future + 1)

for i in range(len(tickers_label)):
    ax = axs[i]
    ax.plot(dias_futuros, future_prices[:, i], marker='o', color=colors_plot[i],
            linestyle='--', linewidth=2.5, markersize=10)

    ax.set_title(f'Estimativa: {tickers_label[i]}', fontsize=14, fontweight='bold')
    ax.set_ylabel(f'Preço de Fechamento ({moedas[i]})')
    ax.set_xlabel('Dias à frente (T+n)')
    ax.set_xticks(dias_futuros)
    ax.grid(True, linestyle=':', alpha=0.6)

    # Adicionar anotações de valor exato
    for x, y in zip(dias_futuros, future_prices[:, i]):
        ax.annotate(f'${y:.2f}', (x, y), textcoords="offset points",
                    xytext=(0,15), ha='center', fontsize=10, fontweight='bold', color=colors_plot[i])

plt.tight_layout(rect=[0, 0.03, 1, 0.95])
plt.show()

# --- TABELA DE RESUMO EXECUTIVO ---
print(f"\n--- Tabela de Projeções: Aglomerado de Metais (RIO & FCX) ---")
df_future = pd.DataFrame(future_prices, columns=tickers_label,
                         index=[f"Dia +{i+1}" for i in range(n_future)])
print(df_future.round(2))

**Persistência de Resultados (Setor de Metais)**

Nesta etapa, salvamos os resultados desnormalizados do modelo de Metais. Como este modelo previu os preços da Rio Tinto (RIO) e da Freeport (FCX), criamos cópias em memória para que o próximo passo do seu script não apague esses valores.

**Segurança de Dados**:
O uso do `.copy()` aqui é o que permite que você mantenha o histórico de Metais vivo enquanto a variável `preds_final` é liberada para outros usos.

# --- SALVAMENTO ESPECÍFICO DO SETOR (METAIS) ---

# Salva os resultados desnormalizados para uso futuro em comparações
# Usamos .copy() para garantir que os dados de RIO e FCX sejam preservados
preds_final_metais = preds_final.copy()
actuals_final_metais = actuals_final.copy()

print("✓ Backup de memória concluído: Resultados brutos de Metais preservados.")

**Blindagem de Variáveis para Correlação Final (Metais)**

Agora, "congelamos" os dados sob nomes fixos. Com `preds_metais_fixed`, você terá a certeza de que esses dados representam exatamente o que foi validado no Bloco 13 de Metais.

**Por que isso é vital para a Correlação?**
Para fazer uma correlação, você precisará comparar `preds_petro_fixed` com `preds_metais_fixed`. Sem essa blindagem, você estaria tentando comparar variáveis que mudam o tempo todo.

# --- FINALIZAÇÃO E SALVAMENTO DE VARIÁVEIS DE CONTROLE ---

# Criamos cópias explícitas para blindagem contra sobrescrita acidental
preds_metais_fixed = preds_final.copy()
actuals_metais_fixed = actuals_final.copy()

print("-" * 60)
print("✅ SETOR DE METAIS CONCLUÍDO E BLINDADO")
print("Resultados disponíveis em: 'preds_metais_fixed'")
print("Sistema pronto para análise de correlação Cross-Asset (Petróleo vs. Metais).")
print("-" * 60)

### Matriz de Correlação e Alinhamento de Dados - Mercados iguais

Este bloco consolida os resultados dos dois fluxos (Petróleo e Metais). O ponto crítico aqui é o alinhamento temporal: como as bolsas podem ter calendários diferentes, usamos o min_len para garantir que estamos comparando "maçãs com maçãs" no mesmo intervalo de dias do conjunto de teste.

**Por que separar Preços de Retornos?**
- **Correlação de Preços**: Mostra se a direção geral (tendência) é a mesma.
- **Correlação de Retornos (%)**: É o padrão ouro das finanças. Ela revela se a **volatilidade** e a intensidade das subidas/descidas diárias estão sincronizadas, eliminando distorções de escala (ex: uma ação custar $10$ e outra $100$).

# --- CONSOLIDAÇÃO E MATRIZ DE CORRELAÇÃO ---

import seaborn as sns

# 1. Alinhamento de Dimensões (Segurança contra calendários diferentes)
min_len = min(len(preds_petro_fixed), len(preds_metais_fixed))

# 2. Criação do DataFrame Consolidado (Preços Previstos)
df_corr = pd.DataFrame({
    'Petroleo_Aramco': preds_petro_fixed[-min_len:, 0],
    'Petroleo_Total':  preds_petro_fixed[-min_len:, 1],
    'Metais_RioTinto': preds_metais_fixed[-min_len:, 0],
    'Metais_Freeport': preds_metais_fixed[-min_len:, 1]
})

# 3. Cálculo de Retornos Diários Previstos (Variação %)
# Essencial para capturar a dinâmica real do mercado
df_retornos = df_corr.pct_change().dropna()

# 4. Visualização: Heatmap de Correlação (Retornos %)
plt.figure(figsize=(10, 8))
sns.heatmap(df_retornos.corr(), annot=True, cmap='RdYlGn', center=0, fmt=".2f", linewidths=0.5)

plt.title('Correlação de Retornos: Petróleo vs Metais (Intersetorial)', fontsize=14)
plt.show()

**Dispersão e Diagnóstico Estratégico Intersetorial**

Enquanto a Matriz de Correlação nos dá um número frio, este bloco utiliza **Gráficos de Dispersão (Scatter Plots)** com **Linhas de Regressão** para visualizar a "personalidade" do movimento entre os setores de Petróleo e Metais.

1. **O Papel** do `sns.regplot`
O gráfico de dispersão mapeia cada dia de retorno previsto como um ponto no espaço.

- **Eixo X**: Retorno do Petróleo.

- **Eixo Y**: Retorno dos Metais.

- **Linha de Regressão (Vermelha)**: É a linha de melhor ajuste. Se ela for muito inclinada para cima, a conexão entre os ativos é forte. Se for quase horizontal, a relação é fraca.

**2. Comparação de Líderes vs. Seguidores**

O código divide a visualização em dois painéis para um diagnóstico de "Aglomerados":

- **Painel 1 (Líderes)**: Compara a Saudi Aramco com a Rio Tinto. Como são os maiores players de seus setores, essa correlação geralmente reflete o sentimento macroeconômico global (Ex: Se o PIB da China cresce, ambos tendem a subir).

- **Painel 2 (Seguidores/Alternativos)**: Compara a TotalEnergies com a Freeport (FCX). Isso ajuda a verificar se a correlação é consistente em todo o setor ou se apenas os líderes estão sincronizados.

# --- DISPERSÃO E DIAGNÓSTICO ESTRATÉGICO ---

plt.figure(figsize=(14, 5))

# Comparação Intersetorial 1: Líderes (Aramco vs Rio Tinto)
plt.subplot(1, 2, 1)
sns.regplot(data=df_retornos, x='Petroleo_Aramco', y='Metais_RioTinto',
            scatter_kws={'alpha':0.4, 'color':'forestgreen'}, line_kws={'color':'red'})
plt.title('Dispersão: Petróleo (Aramco) vs Metais (Rio Tinto)')
plt.grid(True, alpha=0.3)

# Comparação Intersetorial 2: Seguidores (Total vs Freeport)
plt.subplot(1, 2, 2)
sns.regplot(data=df_retornos, x='Petroleo_Total', y='Metais_Freeport',
            scatter_kws={'alpha':0.4, 'color':'royalblue'}, line_kws={'color':'red'})
plt.title('Dispersão: Petróleo (Total) vs Metais (Freeport)')
plt.grid(True, alpha=0.3)

plt.tight_layout()
plt.show()

# --- RELATÓRIO DE INTERPRETAÇÃO AUTOMÁTICA ---
print("\n=== Diagnóstico de Correlação de Retornos ===")
avg_corr_inter = df_retornos[['Petroleo_Aramco', 'Metais_RioTinto']].corr().iloc[0,1]

if avg_corr_inter > 0.7:
    print("⚠️ ALTA SINCRONIA: Os setores respondem ao mesmo estímulo macro (Dólar/Inflação).")
elif avg_corr_inter < 0.3:
    print("✅ ALTA DIVERSIFICAÇÃO: Movimentos independentes. Ótimo para hedge (proteção).")
else:
    print("ℹ️ CORRELAÇÃO MODERADA: Existe influência mútua parcial.")


