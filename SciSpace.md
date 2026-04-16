# Monitoramento Não Invasivo de Frequência Cardíaca e Pressão Arterial via Fotopletismografia Remota (rPPG) e Visão Computacional.

## Questões de pesquisa geradas  

  | Nº | Pergunta em Inglês | Pergunta em Português |
  |----|-------------------|----------------------|
  | 1 | What are the latest machine learning methods for non-invasive heart rate and blood pressure monitoring via rPPG? | Quais são os métodos mais recentes de aprendizado de máquina para monitoramento não invasivo da frequência cardíaca e pressão arterial por meio de rPPG? |
  | 2 | How is computer vision used in remote photoplethysmography for cardiovascular parameter estimation? | Como a visão computacional é utilizada na fotopletismografia remota para estimar parâmetros cardiovasculares? |
  | 3 | What are the main challenges in using rPPG and machine learning for blood pressure and heart rate monitoring? | Quais são os principais desafios no uso de rPPG e aprendizado de máquina para o monitoramento da pressão arterial e da frequência cardíaca? |
  | 4 | What are the latest machine learning methods for non-invasive heart rate and blood pressure monitoring via rPPG? | Quais são os métodos mais recentes de aprendizado de máquina para monitoramento não invasivo da frequência cardíaca e pressão arterial por meio de rPPG? |
  | 5 | How is computer vision used in remote photoplethysmography for cardiovascular parameter estimation? | Como a visão computacional é utilizada na fotopletismografia remota para estimar parâmetros cardiovasculares? |
  | 6 | What are the main challenges in using rPPG and machine learning for blood pressure and heart rate monitoring? | Quais são os principais desafios no uso de rPPG e aprendizado de máquina para o monitoramento da pressão arterial e da frequência cardíaca? |

## Strings de busca utilizadas pela ferramenta  
  | Nº | String de Busca (Original) | Tradução / Interpretação (Português) |
  |----|---------------------------|--------------------------------------|
  | 1 | "remote photoplethysmography" OR rPPG "machine learning" "heart rate" "blood pressure" | "fotopletismografia remota" OU rPPG "aprendizado de máquina" "frequência cardíaca" "pressão arterial" |
  | 2 | "computer vision" rPPG "non-invasive monitoring" (regression OR classification) | "visão computacional" rPPG "monitoramento não invasivo" (regressão OU classificação) |
  | 3 | "remote PPG" "blood pressure estimation" machine learning challenges | "PPG remota" "estimativa de pressão arterial" desafios de aprendizado de máquina |
  | 4 | all:rPPG+AND+all:machine+learning+AND+all:heart+rate | todos os campos: rPPG E todos os campos: aprendizado de máquina E todos os campos: frequência cardíaca |
  | 5 | all:remote+photoplethysmography+AND+all:blood+pressure+AND+all:computer+vision | todos os campos: fotopletismografia remota E todos os campos: pressão arterial E todos os campos: visão computacional |

## Lista dos 8 artigos escolhidos 


## Revisão da literatura 

### 1. Descrição do Problema
A Fotopletismografia Remota (rPPG) é uma técnica de monitoramento sem contato que utiliza câmeras convencionais (RGB) para detectar variações sutis na reflectância da pele causadas pelo ciclo cardíaco. Quando o coração bate, o volume de sangue nos capilares faciais muda, alterando a absorção de luz.

Estimativa de Frequência Cardíaca (HR): O sinal de rPPG é extraído de regiões de interesse (ROI) na face e processado para identificar o pico de frequência dominante, que corresponde aos batimentos por minuto.
Estimativa de Pressão Arterial (BP): Ao contrário da HR, a pressão arterial não é observada diretamente. A literatura utiliza modelos que correlacionam a morfologia da onda de pulso (shape features) ou o Tempo de Trânsito do Pulso (PTT) — o tempo que a onda leva para percorrer dois pontos — com valores sistólicos e diastólicos.


### 2. Áreas de Aplicação
Saúde e Telemedicina: Triagem remota de pacientes, monitoramento de idosos em casa e consultas virtuais.
Bem-estar e Fitness: Aplicativos de saúde para smartphones que monitoram sinais vitais durante exercícios ou repouso sem necessidade de sensores vestíveis.
Segurança e Detecção de Liveness: Verificação de que um rosto em frente à câmera é de uma pessoa viva (baseado no pulso sanguíneo) para evitar fraudes em sistemas biométricos e detecção de deepfakes.
Computação Afetiva: Análise de estresse, fadiga e estados emocionais em motoristas ou trabalhadores sob alta carga cognitiva.


### 3. Tipos de Tarefas de Aprendizado de Máquina
O problema é resolvido predominantemente através de:

Regressão (Tarefa Principal):
Modelos de Deep Learning (CNNs 3D, Transformers) são usados para prever a série temporal do sinal de volume sanguíneo (BVP) ou diretamente os valores contínuos de HR e BP.
Exemplo: Uso de redes como DeepPhys ou PhysNet para extrair sinais fisiológicos de vídeos.
Classificação:
Usada de forma secundária para categorizar estados de saúde (ex: Hipertensão vs. Normotensão) ou níveis de estresse.
Agrupamento (Clustering):
Menos comum, mas utilizado na fase de pré-processamento para segmentar regiões da face com melhor relação sinal-ruído (SNR).



Contactless Blood Pressure Measurement Via Remote Photoplethysmography With Synthetic Data Generation Using Generative Adversarial Networks


### 4. Principais Desafios na Literatura
Variações de Iluminação: Mudanças súbitas ou luz ambiente fraca podem obscurecer as variações de cor da pele, dificultando a extração do sinal.
Movimentos da Cabeça: Movimentos voluntários ou involuntários do usuário introduzem ruídos que superam a amplitude do sinal rPPG.
Diversidade de Tom de Pele: Peles com maior concentração de melanina absorvem mais luz, resultando em uma relação sinal-ruído mais baixa, o que pode levar a vieses algorítmicos.
Compessão de Vídeo: Formatos de compressão (como H.264) podem eliminar as variações sutis de cor necessárias para o rPPG.
Generalização de Domínio: Modelos treinados em laboratório frequentemente perdem precisão em cenários reais ("in-the-wild").



### Referências Principais:
## Referências Principais

1. RAO, G. N.; BHARGAV, D. (2025).  
   **Remote Heart Rate Estimation Using Deep Learning-Based RPPG Models.**  
   *Indian Scientific Journal of Research in Engineering and Management.*

2. SHAO, H. et al. (2024).  
   **TranPulse: Remote Photoplethysmography Estimation with Time-Varying Supervision.**  
   *IEEE Transactions on Instrumentation and Measurement.*

3. CHU, S. et al. (2025).  
   **CodePhys: Robust Video-based Remote Physiological Measurement through Latent Codebook Querying.**  
   *arXiv.*

4. MA, X. (2020).  
   **Towards a Contactless Vital Sign System.**  
   *University of Ottawa.*


Contactless Blood Pressure Measurement Via Remote Photoplethysmography With Synthetic Data Generation Using Generative Adversarial Networks
