# GNN
GraphNeuralNetwork


### 참고 서적 : 그래프 신경망 입문

![image](https://github.com/junyong1111/GNN/assets/79856225/aa452c1c-5ee6-4bc8-a8be-f95e0c022d52)



아래 정리는 그래프 신경망 입문 (즈위안 리우, 지에 저우 지음,  정지수 옮김)책을 참고하였습니다.

#— 기본적인 그래프 이론과 신경망, 선형대수학은 알고 있다고 가정하고 진행

### 기본 그래프 신경망

GNN의 개념은 고리, 스카셀리가 제안했으며 스카셀리의 모델을 대표로 설명합니다.

그래프에서 노드는 **특징과 관련된 노드**로 정의되며 GNN의 최종 목표는 **각 노드의 상태 임베딩**을 학습하는 것이다. 여기서 말하는 **상태 임베딩이**란 해**당 노드와 주변 노드의 정보를 포함하고** 있고 노드의 출력을을 얻을 때 사용된다. 

### **그래프 어텐션 네트워크**

Attention mechanism은 기계 독해와 같은 **순서에 기반한 문제**들을 성공적으로 해결했다. GCN이 모든 이웃 노드를 골고루 다루는 반면에 어텐션 메커니즘을 사용하면 이웃 노드들에 각기 다른 가중치를 줄 수 있어서 중요한 이웃과 중요하지 않은 이웃 노드을 구분한 수 있다. 이번 장에서는 어텐션 메커니즘과 GNN을 결합한 GAT와 GaAN에 대해서 알아보자.

**GAT**

벨리코비크는 전파 단계에 어텐션 메커니즘을 결합하는 GAT를 제안했다. GAT는 셀프 어텐션 전략을 따르며 각 노드의 은닉 상태는 이웃 노드를로부터 계산한다.
