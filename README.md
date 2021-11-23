# K-Means (K-평균) tutorial

## 개요
k-means 클러스터링 방법은 n개의 데이터를 입력 받았을 때, n보다 작거나 같은 k개의 그룹으로 나누는 것을 의미한다. k-means 알고리즘은 각 그룹의 중심(centroid)과 그룹 내의 데이터들과의 유클리드 거리를 최소화 하는 방향으로 동작한다.

## 실행 과정
### 1. 초기 중심점 선택
![k개의 초기 중심점](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/K_Means_Example_Step_1.svg/187px-K_Means_Example_Step_1.svg.png)

데이터 중 랜덤한 k개의 중심점을 선택(위 그림의 경우 k=3)

### 2. 그룹화(클러스터링)
![유클리드 거리에 따른 그룹화](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/K_Means_Example_Step_2.svg/209px-K_Means_Example_Step_2.svg.png)

모든 점들은 각 중심점과의 유클리드 거리에 따라 해당 그룹으로 묶임

### 3. 중심점 재설정 및 클러스터링
![중심점 재설정](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3e/K_Means_Example_Step_3.svg/209px-K_Means_Example_Step_3.svg.png)

그룹에 포함된 점들의 평균으로 중심점을 재설정

![재클러스터링](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d2/K_Means_Example_Step_4.svg/209px-K_Means_Example_Step_4.svg.png)

수렴할 때까지 2,3 과정을 반복

---
출처
- https://ko.wikipedia.org/wiki/K-%ED%8F%89%EA%B7%A0_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98
- https://velog.io/@gayeon/%EB%8D%B0%EC%9D%B4%ED%84%B0-%EB%B6%84%EC%84%9D-%EC%B4%88%EB%B3%B4%EC%9E%90%EB%A5%BC-%EC%9C%84%ED%95%9C-k-means-clustering-with-sklearn
