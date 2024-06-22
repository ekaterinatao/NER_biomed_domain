# NER_biomed_domain

## Активное обучение
  
Эксперименты с активным обучением на основе модели `RuBioBERT` [ссылка](https://github.com/ekaterinatao/NER_biomed_domain/tree/main/active_learning)  
  
Сравнение стратегий активного обучения (MNLP и BALD) с рандомным сэмплированием и отбором на основании точности   
  
**Лучшая стратегия MNLP**:
* повышено качество обучения модели на 2% на равных объемах размеченного тренировочного  
* уменьшен объем размеченного тренировочного корпуса на 12%  

[](https://github.com/ekaterinatao/NER_biomed_domain/blob/main/data/MIPT_master_thesis/NER_biomed_domain/data/AL_sampling_30iter_mnlp_rand_bald.png)  
  
|                            | Random sampling | MNLP            | BALD            | 'accuracy'      |
| -------------------------- | --------------- | --------------- | --------------- | --------------- |
|F1-score test (10% of data) | 70.15 ± 1.50    | 72.51 ± 0.94    | 67.32 ± 0.95    | 73.58 ± 0.43    |
|F1-score test (15% of data) | 73.98 ± 1.28    | 75.28 ± 0.71    | 71.30 ± 1.41    | 75.99 ± 0.21    |
|F1-score test (20% of data) | 75.60 ± 1.01    | 77.16 ± 1.09    | 73.54 ± 1.38    | 76.89 ± 0.54    |  

## Базовые модели без активного обучения
Обучение трансформеров с базовыми параметрами [ссылка](https://github.com/ekaterinatao/NER_biomed_domain/tree/main/transformers_base)  

Сравнение базовых трансформеров из семейства BERT [ссылка](https://api.wandb.ai/links/taoea/fg3xt01o)  
|                            | BERT base       | ruBERT          | RuBioBERT       | RuBioRoBERTa    |
| -------------------------- | --------------- | --------------- | --------------- | --------------- |
|F1-score test (100% of data)| 63.82           | 79.04           | 82.65           | 84.99           |  

Модель `RuBioBERT`при обучении на 100%, 70% и 50% датасета [ссылка](https://api.wandb.ai/links/taoea/d0zdikvq)  
  
Подбор гиперпараметров для базовых моделей [ссылка](https://github.com/ekaterinatao/NER_biomed_domain/blob/main/transformers_base/%D0%92%D0%9A%D0%A0_nerel_bio_ruBERT_base.ipynb)  
