# Introdução
Este repositório tem como intuito o desenvolvimento de um modelo para classificação de imagens de Raio-X de pacientes saudáveis e doentes. Tal tarefa foi inspirada e utiliza os dados de https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset. A fim de entregar ao modelo de classificação dados mais confiáveis, um outro modelo de visão computacional foi empregado para segmentação dos pulmões e, após treino e validação, utilizado nas imagens contidas no dataset do Kaggle, para gerar imagens que contem apenas os pulmões dos pacientes.

## Metodologia
Para ser possível realizar uma boa classificação da imagens de raio-X, inicialmente, utilizou-se um modelo de Segmentação de imagem a fim de criar máscaras da localização dos pulmões e filtrar cada imagem com tais máscaras. Um exemplo da segmentação é mostrados a seguir:
![ex_lung](https://user-images.githubusercontent.com/24653032/217374837-5c63e061-79dd-49dd-926f-0e986cbfe0a7.png)

A descrição de todos os dados utilizados pode ser encontrada em: https://kaggle.com/datasets/fb4823d1ab6f96333377a7c94f90f9fe6f589c78643ed8a463d17d0bd67a193f

## Referências

•	Montgomery Dataset: Contém imagens de máscaras feitas a mão, foi utilizado como input do modelo de segmentação

Jaeger S, Candemir S, Antani S, Wáng YX, Lu PX, Thoma G. Two public chest X-ray datasets for computer-aided screening of pulmonary diseases. Quant Imaging Med Surg. 2014 Dec;4(6):475-7. doi: 10.3978/j.issn.2223-4292.2014.11.20. PMID: 25525580; PMCID: PMC4256233.
  
• National Library of Medicine, National Institutes of Health, Bethesda, MD, USA and Shenzhen No.3 People’s Hospital, Guangdong Medical College, Shenzhen, China

    1)	Jaeger S, Karargyris A, Candemir S, Folio L, Siegelman J, Callaghan F, Xue Z, Palaniappan K, Singh RK, Antani S, Thoma G, Wang YX, Lu PX, McDonald CJ.  Automatic tuberculosis screening using chest radiographs. IEEE Trans Med Imaging. 2014 Feb;33(2):233-45. doi: 10.1109/TMI.2013.2284099. PMID: 24108713
    2)	Candemir S, Jaeger S, Palaniappan K, Musco JP, Singh RK, Xue Z, Karargyris A, Antani S, Thoma G, McDonald CJ. Lung segmentation in chest radiographs using anatomical atlases with nonrigid registration. IEEE Trans Med Imaging. 2014 Feb;33(2):577-90. doi: 10.1109/TMI.2013.2290491. PMID: 24239990

  -Contém imagens de máscaras feitas a mão, foi utilizado como input do modelo de segmentação
 
• Modelos de segmentação -- segmentation_models.pytorch 

https://github.com/qubvel/segmentation_models.pytorch
