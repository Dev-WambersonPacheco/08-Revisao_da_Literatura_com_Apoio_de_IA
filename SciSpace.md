# Monitoramento Não Invasivo de Frequência Cardíaca e Pressão Arterial via Fotopletismografia Remota (rPPG) e Visão Computacional.

## SciSpace
## Questões de pesquisa geradas  

  | Nº | Pergunta em Inglês | Pergunta em Português |
  |----|-------------------|----------------------|
  | 1 | What are the latest machine learning methods for non-invasive heart rate and blood pressure monitoring via rPPG? | Quais são os métodos mais recentes de aprendizado de máquina para monitoramento não invasivo da frequência cardíaca e pressão arterial por meio de rPPG? |
  | 2 | How is computer vision used in remote photoplethysmography for cardiovascular parameter estimation? | Como a visão computacional é utilizada na fotopletismografia remota para estimar parâmetros cardiovasculares? |
  | 3 | What are the main challenges in using rPPG and machine learning for blood pressure and heart rate monitoring? | Quais são os principais desafios no uso de rPPG e aprendizado de máquina para o monitoramento da pressão arterial e da frequência cardíaca? |
  | 4 | What are the latest machine learning methods for non-invasive heart rate and blood pressure monitoring via rPPG? | Quais são os métodos mais recentes de aprendizado de máquina para monitoramento não invasivo da frequência cardíaca e pressão arterial por meio de rPPG? |
  | 5 | How is computer vision used in remote photoplethysmography for cardiovascular parameter estimation? | Como a visão computacional é utilizada na fotopletismografia remota para estimar parâmetros cardiovasculares? |
  | 6 | What are the main challenges in using rPPG and machine learning for blood pressure and heart rate monitoring? | Quais são os principais desafios no uso de rPPG e aprendizado de máquina para o monitoramento da pressão arterial e da frequência cardíaca? |

### Strings de busca utilizadas pela ferramenta  
  | Nº | String de Busca (Original) | Tradução / Interpretação (Português) |
  |----|---------------------------|--------------------------------------|
  | 1 | "remote photoplethysmography" OR rPPG "machine learning" "heart rate" "blood pressure" | "fotopletismografia remota" OU rPPG "aprendizado de máquina" "frequência cardíaca" "pressão arterial" |
  | 2 | "computer vision" rPPG "non-invasive monitoring" (regression OR classification) | "visão computacional" rPPG "monitoramento não invasivo" (regressão OU classificação) |
  | 3 | "remote PPG" "blood pressure estimation" machine learning challenges | "PPG remota" "estimativa de pressão arterial" desafios de aprendizado de máquina |
  | 4 | all:rPPG+AND+all:machine+learning+AND+all:heart+rate | todos os campos: rPPG E todos os campos: aprendizado de máquina E todos os campos: frequência cardíaca |
  | 5 | all:remote+photoplethysmography+AND+all:blood+pressure+AND+all:computer+vision | todos os campos: fotopletismografia remota E todos os campos: pressão arterial E todos os campos: visão computacional |

### artigos escolhidos 
| Título                                                                                                                                     | Fonte         | Ano  | Relevance Score | Relevance Tag   |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------- | ---- | --------------- | --------------- |
| Contactless Blood Pressure Measurement via Remote Photoplethysmography with Synthetic Data Generation Using Generative Adversarial Network | IEEE          | 2022 | 100/100         | Highly Relevant |
| VidFormer: A novel end-to-end framework fused by 3DCNN and Transformer for Video-based Remote Physiological Measurement                    | SciSpace      | 2020 | 100/100         | Highly Relevant |
| Neurodata Lab’s approach to the Challenge on Computer Vision for Physiological Measurement                                                 | SciSpace      | 2020 | 100/100         | Highly Relevant |
| HeartTrack: Convolutional neural network for remote video-based heart rate monitoring                                                      | IEEE          | 2020 | 100/100         | Highly Relevant |
| Non-contact PPG signal and heart rate estimation with multi-hierarchical convolutional network                                             | ScienceDirect | 2023 | 100/100         | Highly Relevant |
| DEVICE AGNOSTIC MEASUREMENT OF BLOOD PRESSURE FROM RPPG SIGNALS                                                                            | SciSpace      | 2023 | 100/100         | Highly Relevant |
| AI-enabled remote monitoring of vital signs for COVID-19: methods, prospects and challenges                                                | Springer      | 2023 | 100/100         | Highly Relevant |
| FREQ2TIME: WEAKLY SUPERVISED LEARNING OF CAMERA-BASED RPPG FROM HEART RATE                                                                 | IEEE          | 2024 | 100/100         | Highly Relevant |


### Revisão da literatura 

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
   
---

## NotebookLM
### 1. Resumo Estruturado

### Técnicas de Aprendizado de Máquina
As **Redes Neurais Convolucionais 3D (3D CNNs)** são amplamente utilizadas devido à sua capacidade de capturar simultaneamente informações espaciais e temporais em vídeos faciais. Redes recorrentes, como **LSTM**, são empregadas para modelar dependências sequenciais em sinais fisiológicos, especialmente em aplicações de pressão arterial. Mais recentemente, **Transformers** vêm sendo integrados para capturar relações globais de longo alcance, superando limitações das CNNs. Além disso, **Redes Adversariais Generativas (GANs)** são utilizadas para gerar dados sintéticos e mitigar a escassez de dados biométricos.

### Atributos (Features) Frequentes
O principal atributo utilizado é a **variação de cor da pele (sinal rPPG)** nos canais RGB, relacionada ao fluxo sanguíneo. Também são comuns características **morfológicas da onda**, como picos sistólicos e incisuras (notches), além de suas derivadas (1ª a 4ª ordem). Informações auxiliares como **idade e IMC (BMI)** são frequentemente incorporadas para melhorar a calibração dos modelos.

### Principais Desafios
Os principais desafios incluem:
- **Artefatos de movimento**, como movimentação da cabeça
- **Variações de iluminação** ambiente
- **Escassez de bases de dados** grandes e diversificadas com ground truth confiável
- Variabilidade de **tons de pele**
- Impacto da **compressão de vídeo** na qualidade do sinal

### Técnicas de Pré-processamento
O fluxo típico inclui:
- **Detecção facial e de marcos (landmarks)**
- Definição de **Regiões de Interesse (ROIs)**, como testa e bochechas
- **Filtragem passa-banda** (geralmente entre 0.5 e 8 Hz)
- **Normalização espacial e temporal**

### Métricas de Avaliação
As métricas mais utilizadas são:
- **MAE (Erro Médio Absoluto)**
- **RMSE (Raiz do Erro Quadrático Médio)**
- **Coeficiente de Correlação de Pearson (r)**
- **Desvio padrão (SD)**
- Critérios clínicos como **AAMI**

### 2. Tabela Comparativa

## Tabela Comparativa Completa (8 Artigos)

| Nome / Referência | Técnica(s) Utilizada(s) | Atributos Utilizados | Tipo de Tarefa | Técnicas de Pré-processamento | Métricas de Avaliação | Principais Contribuições |
|------------------|------------------------|----------------------|----------------|-------------------------------|------------------------|---------------------------|
| Bin Li et al. (2023) | 3D CNN (STSC) e Módulo MHFF | Distribuição de cor facial; fluxo óptico esparso para marcos | Regressão (HR e rPPG) | Corte de fundo (ERT); normalização; rastreamento por pirâmide LK | MAE, RMSE, Pearson (r), SD | Rede 3D eficiente com fusão multi-hierárquica; requer apenas 15s de vídeo; novo dataset FaceBio-v1 |
| Bing-Fei Wu et al. | CNN Encoder-Decoder; InfoGAN | Sinais rPPG (face superior/inferior); idade e IMC | Regressão (Pressão Sistólica/Diastólica) | Detecção facial; alinhamento de ROI; extração rPPG (CHROM) | MAE, Desvio Padrão (Std) | Estimador multicanal; uso de GAN para gerar dados sintéticos e mitigar escassez de dados |
| P. Parashiva et al. (2023) | LSTM | Intensidade do canal vermelho; derivadas do sinal (até 4ª ordem) | Regressão (SBP e DBP) | Filtro Butterworth (0.5–8 Hz); segmentação de batimentos; zero-padding | RMSE, MAE, Critérios AAMI/BHI | Método agnóstico de dispositivo para smartphones; robusto a mudanças na taxa de amostragem |
| Jeremy Speth et al. (2024) | 3D CNN (baseada em PhysNet) | Canais expandidos (CHROM, POS, Diff); aumentos de iluminação e ruído | Regressão (HR e HRV) | Marcos faciais (MediaPipe); redimensionamento; expansão de canais (3→9) | MAE, RMSE, Pearson (r), RMSSD, SDNN | Framework Freq2Time para aprendizado fracamente supervisionado |
| M. Artemyev et al. (Neurodata Lab - RePSS) | 3D Attention CNN; 1D CNN | Derivada temporal (diff); frames RGB; máscaras faciais | Regressão (HR médio) | Detecção (RetinaNet); alinhamento afim; filtro FIR passa-banda (45–180 bpm) | MAE, RMSE, Pearson (R) | Mecanismo de atenção para seleção de ROI; rede 1D pré-treinada em dados sintéticos |
| Olga Perepelkina et al. (HeartTrack) | 3D spatio-temporal attention CNN; 1D CNN | Canais RGB (diff); máscaras de pele; marcos faciais | Regressão (Monitoramento de HR) | Filtro passa-banda; alinhamento facial; ROI pooling | MAE, RMSE, Pearson (R) | Arquitetura HeartTrack; integração com síntese de dados; novos datasets MoLi-ppg-1 e 2 |
| Jiachen Li et al. (VidFormer) | Fusão de 3D CNN e Transformers | Patches de cubos de vídeo; atenção espaço-temporal (ST-MHSA) | Regressão (HR, HRV, RF) | Marcos faciais (dlib); recorte de ROI; redimensionamento (128×128) | MAE, RMSE, Pearson (r), STD | Primeiro framework CNN-Transformer (VidFormer); integração de características locais e globais |
| Honnesh Rohmetra et al. (Revisão) | Revisão de CNNs, RNNs, SVR e Sistemas Fuzzy | Vídeo RGB; áudio (tosse); oximetria óptica | Levantamento de métodos (HR, RR, BP, SpO2, tosse) | Segmentação de ROI facial; remoção de artefatos (SVD ou GAN) | MAE, RMSE, Sensibilidade | Revisão abrangente sobre monitoramento remoto na COVID-19; destaque para soluções sem contato |

