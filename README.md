# NER_biomed_domain

## Эксперименты
  
Экспериментs с активным обучением на основе модели `RuBioBERT` [ссылка](https://github.com/ekaterinatao/NER_biomed_domain/tree/main/active_learning)  
  
Обучение трансформеров с базовыми параметрами [ссылка](https://github.com/ekaterinatao/NER_biomed_domain/tree/main/transformers_base)  

## Отчеты об обучении
  
Сравнение базовых трансформеров из семейства BERT [ссылка](https://api.wandb.ai/links/taoea/fg3xt01o)  
Лучшее качество демонстрирует `RuBioBERT`  
  
Модель `RuBioBERT`при обучении на 100%, 70% b 50% датасета [ссылка](https://api.wandb.ai/links/taoea/d0zdikvq)  
  
Подбор гиперпараметров для базовых моделей [ссылка](https://github.com/ekaterinatao/NER_biomed_domain/blob/main/transformers_base/%D0%92%D0%9A%D0%A0_nerel_bio_ruBERT_base.ipynb)  
  
Сравнение стратегий активного обучения (MNLP и BALD) с рандомным сэмплированием и базовой моделью [ссылка](https://api.wandb.ai/links/taoea/18vvray4)  
|                            | Random sampling | MNLP            | BALD            | Non AL          |
| -------------------------- | --------------- | --------------- | --------------- | --------------- |
|F1-score test (100% of data)| 82.28           | 81.89           | 82.75           | 82.65           |
|F1-score test (70% of data) | 80.87           | 80.6            | 78.87           | 81.35           |
|F1-score test (50% of data) | 80.78           | 79.33           | 78.35           | 81.02           |  
