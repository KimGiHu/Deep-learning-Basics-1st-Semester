# 심화학습 기초 1학기 프로젝트

기존의 baseline 코드의 output을 향상시키도록, 수업시간에 배운 기초 딥러닝 지식을 활용하여 시도해보자.
- - - - -
- 기존의 baseline 코드의 Accuracy : 97.16%
- - - - -
- test해보고 있는 현 상황을 표로 정리하였습니다.
1. change the learning rate and epoch for increasing the accuracy

- No ensemble

|learning_rate\epoch| 50 |   100   |   150   |   200   |
|:------:|:---:|:---:|:---:|:---:|
0.01    |  96.3 |  96.34  | 96.34  | 96.37  | 
0.001      |  96.05 |  95.40  | 95.52  | 95.39  |

- Ensemble

|learning_rate\epoch| 50 |   100   |   150   |   200   |
|:------:|:---:|:---:|:---:|:---:|
0.01    |  97.16 |  97.15  | 97.15  | 97.14  | 
0.001      |  97.15 |  96.44  | 96.38  | 96.36  |

- - - - - 
2. change the step size for increasing the accuracy (step size : 30 -> 20 / 30 -> 15)


|step_size| 30 |   15   |   20   |   45   |  60   |
|:------:|:---:|:---:|:---:|:---:|
no ensemble    |  96.3 |  96.37  | 96.32  | 96.19  |  96.19   |
ensemble      |  97.16 |  96.86  | 96.87  | 96.87  |  96.87   |

  (1) step size : 30 -> 20

  - No ensemble : 96.32%

  - Ensemble : 96.86%

  (2) step size : 30 -> 15

  - No ensemble : 96.37%

  - Ensemble : 96.87%

  (3) step size : 30 -> 45

  - No ensemble : 96.19%

  - Ensemble : 96.87%

  (4) step size : 30 -> 60

  - No ensemble : 96.19%

  - Ensemble : 96.87%
