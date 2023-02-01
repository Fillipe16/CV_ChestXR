# Introdução
Este repositório tem como intuito o desenvolvimento de um modelo para classificação de imagens de Raio-X de pacientes saudáveis e doentes. Tal tarefa foi inspirada e utiliza os dados de https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset. A fim de entregar ao modelo de classificação dados mais confiáveis, um outro modelo de visão computacional foi empregado para segmentação dos pulmões e, após treino e validação, utilizado nas imagens contidas no dataset do Kaggle, para gerar imagens que contem apenas os pulmões dos pacientes.

# Referências

### •	Montgomery Dataset:Jaeger S, Candemir S, Antani S, Wáng YX, Lu PX, Thoma G. Two public chest X-ray datasets for computer-aided screening of pulmonary diseases. Quant Imaging Med Surg. 2014 Dec;4(6):475-7. doi: 10.3978/j.issn.2223-4292.2014.11.20. PMID: 25525580; PMCID: PMC4256233.
  -Contém imagens de máscaras feitas a mão, foi utilizado como input do modelo de segmentação

### • National Library of Medicine, National Institutes of Health, Bethesda, MD, USA and Shenzhen No.3 People’s Hospital, Guangdong Medical College, Shenzhen, China
    1)	Jaeger S, Karargyris A, Candemir S, Folio L, Siegelman J, Callaghan F, Xue Z, Palaniappan K, Singh RK, Antani S, Thoma G, Wang YX, Lu PX, McDonald CJ.  Automatic tuberculosis screening using chest radiographs. IEEE Trans Med Imaging. 2014 Feb;33(2):233-45. doi: 10.1109/TMI.2013.2284099. PMID: 24108713
    2)	Candemir S, Jaeger S, Palaniappan K, Musco JP, Singh RK, Xue Z, Karargyris A, Antani S, Thoma G, McDonald CJ. Lung segmentation in chest radiographs using anatomical atlases with nonrigid registration. IEEE Trans Med Imaging. 2014 Feb;33(2):577-90. doi: 10.1109/TMI.2013.2290491. PMID: 24239990

  -Contém imagens de máscaras feitas a mão, foi utilizado como input do modelo de segmentação
 
 ### • Modelos de segmentação -- segmentation_models.pytorch 
 @misc{Iakubovskii:2019,
  Author = {Pavel Iakubovskii},
  Title = {Segmentation Models Pytorch},
  Year = {2019},
  Publisher = {GitHub},
  Journal = {GitHub repository},
  Howpublished = {\url{https://github.com/qubvel/segmentation_models.pytorch}}
}
