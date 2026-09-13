| 순서 | 모델 | 탄생 배경·해결하려던 문제 | 공부할 핵심 |
|---|---|---|---|
| 1 | [AlexNet (2012)](https://papers.nips.cc/paper_files/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html) | 대규모 이미지 분류에 깊은 CNN을 효과적으로 학습시키기 | GPU 학습, ReLU, Dropout, 데이터 증강 |
| 2 | [VGG (2014)](https://arxiv.org/abs/1409.1556) | **네트워크를 더 깊게 만들면 성능이 좋아지는가?** | 작은 `3×3` 필터 반복, 깊이, receptive field |
| 3 | [Network in Network (2013)](https://arxiv.org/abs/1312.4400) | 각 지역에서 특징을 더 풍부하게 추출하고, 큰 FC 분류기를 대체하기 | `1×1 Conv`, Global Average Pooling. **개념만 짧게** |
| 4 | [GoogLeNet / Inception v1 (2014)](https://arxiv.org/abs/1409.4842) | 연산량을 과도하게 늘리지 않으면서 깊고 넓게 만들기 | 여러 크기의 필터를 병렬 사용, `1×1 Conv`로 채널 축소 |
| 5 | [ResNet (2015)](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper) | 깊이를 늘렸는데 **훈련 오차까지 나빠지는 현상** 해결 | Residual connection: `y = F(x) + x` |
| 6 | [DenseNet (2016/2017)](https://arxiv.org/abs/1608.06993) | 이전 층의 특징을 재사용하고 정보·gradient 전달을 강화하기 | 이전 특징들을 **이어 붙이기(concat)**, ResNet의 덧셈과 비교 |
| 7 | [MobileNet v1 (2017)](https://arxiv.org/abs/1704.04861) | 모바일 환경에서도 사용할 수 있도록 연산량 줄이기 | Depthwise convolution + Pointwise convolution |
| 8 | [EfficientNet (2019)](https://arxiv.org/abs/1905.11946) | 모델을 키울 때 깊이·너비·입력 해상도를 어떻게 배분할까? | 세 요소를 함께 조절하는 compound scaling |