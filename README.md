🌍 Análise de Interdependência Geopolítica
Modelagem via LSTM/GRU para o Mercado de Petróleo e Metais
1. Premissa Central do Estudo
O Estreito de Ormuz atua como um "ponto de pressão" único no comércio global. A nossa tese propõe que a instabilidade logística nesta região não afeta apenas o escoamento de energia (Petróleo), mas dita diretamente a viabilidade econômica da produção de commodities industriais (Metais).

2. Objetivos da Modelagem
Através da combinação de redes neurais profundas (LSTM e GRU), este estudo busca:

Quantificar a Defasagem Temporal: Entender quanto tempo leva para um choque no setor energético impactar o preço dos metais.

Medir a Força da Correlação: Identificar o grau de interdependência entre esses dois aglomerados (clusters) aparentemente distintos.

Projeção Multivariada: Gerar estimativas de curto prazo para ativos críticos como Aramco, TotalEnergies, Rio Tinto e Freeport.

3. Estrutura Técnica do Pipeline
A análise está dividida em dois fluxos principais de processamento:

Fluxo 1 (Energia): Foco em Petróleo Brent/WTI e gigantes do setor (Saudi Aramco / TotalEnergies).

Fluxo 2 (Metais): Foco em Minério de Ferro e Metais Não-Ferrosos (Rio Tinto / Freeport-McMoRan).

Coeficiente (r),Classificação,Significado Estratégico
>0.7,Alta Sincronia,Risco de Concentração: O mercado opera em blocos (Risk-On ou Risk-Off). Não há diversificação; setores se movem juntos.
0.3 a 0.7,Moderada,"Influência Mútua: Os setores compartilham pressões macro, mas mantêm independência técnica individual."
<0.3,Alta Diversificação,Hedge (Proteção): Cenário ideal para carteira. Os setores são independentes; um protege a queda do outro.
