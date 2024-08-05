**이 글은 해당 논문을 읽고 정리한 기록입니다. <a href="https://arxiv.org/pdf/2006.05525">Knowledge Distillation : Survey</a>**

## Abstract 
- 현재 딥러닝은 많은 파라미터들을 이용하고 많은 데이터들을 이용하여 성공하였습니다.
- 그러나 기기에선(on device) 자원이 제한되어 있기 때문에 위와 같은 딥러닝 모델을 배포하기엔 어려움이 존재합니다.
    - 딥러닝 모델은 높은 계산 복잡도를 요구하고, 큰 저장 공간을 요구하기 때문입니다.
- 기기에서도 딥러닝 모델을 사용하기 위해 모델 압축 및 가속 기술이 발전되었고, 이 논문에서 다루는 knowledge distillation은 해당 기술의 대표적인 종류입니다.
    - knowledge distillation : 작은 student model이 큰 teacher model로부터 배우는 것을 말합니다.

## Introduction
- 초록에서 얘기한 딥러닝은 매우 깊은 layer들과 강력한 GPU,TPU로 쉽게 훈련해왔고 좋은 성공을 보였으나 이것은 실제 realtime으로 작동하기 어렵고 device에서 사용하기 어렵다는 이야기를 하며 시작합니다.

- 효율적인 딥러닝 모델을 개발하기 위해
    1. deep model에 대해 efficient building blocks , depthwise separable convolution 포함하기 ( MobileNets, ShuffleNets )
    2. model compression(모델 압축), acceleration (가속) technique 
        - Parameter Pruning, sharing : 성능에 큰 영향을 미치지 않는 파라미터 제거하기
            - 종류
                1. Quantization
                2. Binarization
                3. Structural Matrices
                4. Parameter Sharing
                5. 

