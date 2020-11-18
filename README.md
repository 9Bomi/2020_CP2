# 2020_CP2
## 빅데이터를 활용한 입지분석 모델링
### 쉐어하우스 데이터를 활용한 입지분석 모델 생성, 활용
------------
### 🎈Project 개요
> 최근 원룸, 빌라, 쉐어하우스 등 주거 사업의 수요와 공급이 증가함에 따라 경제적 이득의 최대화를 위한 입지 선정이 굉장히 중요한 이슈로 떠올랐다. 이에 따라 빅데이터 자료를 딥러닝을 이용해 입지를 분석하고 원하는 위치의 적합도를 예측하였다. 또한 시각적 편의를 위해 그 결과값을 웹을 통하여 시각화하여 표현하였다. 

### 🌹데이터 전처리
> 우리는 다양한 빅데이터 중 쉐어하우스에 대한 데이터를 이용하여 입지를 분석하였다. 데이터는 각 쉐어하우스의 방 크기, 방의 거주인원 수 등을 포함하고 있다. 이런 내부 데이터들과 주거지 선택과 밀접한 관계를 가지는 외부 데이터들, 즉 대학, 버스 정류장, 지하철 역, 의료 시설 등 편의 시설들과의 거리를 합하여 데이터로 사용하였다. 이 데이터들을 MinMax Scaler등을 활용하여 정규화를 진행하는 등 다양한 전처리 기법들을 시험해보며 더 정밀한 결과값을 얻고자하였다.

### 🧩최적의 Deep Learning model 선정
> 가장 좋은 결과값을 얻어내기 위해 우리는 여러가지 Deep Learning model들을 시도해 보았다.
##### Logistic Regression
> 우선 Supervised Learning 중 하나인 Logistic Regression을 사용해보았다. Logistic Regression은 수치형 설명변수 X와 연속형 숫자로 이뤄진 종속변수 Y 간의 관계를 선형으로 가정하고 이를 가장 잘 표현할 수 있는 회귀계수를 데이터로부터 추정하는 모델이며, 이 회귀계수들은 모델의 예측값과 실제값의 차이, 즉 오차제곱합(error sum of squares)을 최소로 하는 값들이다. 즉, 데이터들이 Class에 속할 확률을 알려주는 Algorithm이라고 할 수 있다. 그리고 이를 통해 해당 위치에 대한 적합도를 계산해 낼 수 있다.
##### Clustering
> Clustering은 Unsupervised Learning 중 하나로써, 데이터들이 주어졌을 때, 개체들을 몇 개의 Cluster(부분 그룹)으로 나누는 과정을 의미한다. 즉 학습에 사용한 빅데이터들을 각종 데이터들을 이용하여 Cluster로 나누고, 이를 토대로 새로운 데이터를 입력했을 때 무슨 Cluster에 속하는 지를 예측하는 방법이라고 볼 수 있다. 우리는 다양한 Cluster model들을 실험해 보았다. 가장 유명한 방법인 K-means를 비롯해, hierarchical clustering, DBSCAN 등을 모두 실험해 보았다. 

### 👀시각화를 위한 Web 구축
> 결과값을 더 효율적으로 확인하기 위해 Web을 통해 정리하고 시각화하였다.

### 🎁기대효과
> 우리는 이 프로젝트를 통해 주거 사업에 큰 도움을 줄 수 있을 것이라고 생각한다. 원룸, 쉐어하우스 등 모든 주거 사업들에 입지 선정이 가장 큰 성공 요인으로 뽑히고 있고, 우리 프로젝트는 이를 효과적으로 도울 수 있을 것이라고 생각한다. 현재는 단지 쉐어하우스의 데이터를 이용해서 학습을 하고 구현을 하였지만, 데이터 입력만 바꿔주면 다른 주거 사업들에도 쉽게 적용이 가능하고, 더 나아가 식당, 다양한 창업을 위한 입지 분석에도 쉽게 사용할 수 있다. 이러한 점을 통해 입지 분석에 애를 먹고 있는 수많은 사람들에게 큰 도움이 될 수 있을 것이다.
------------
### 🙋‍♂️팀원소개
##### 이정진 (심화컴퓨터전공 4학년) - 팀장
##### 구보미 (심화컴퓨터전공 4학년)
##### 이다연 (심화컴퓨터전공 4학년)
##### 이준하 (심화컴퓨터전공 3학년)
