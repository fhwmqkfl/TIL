# 그리디(당장 좋은것만 고르는 케이스)

선택의 순간마다 당장 눈앞에 보이는 최적의 상황만을 쫓아 최종적인 해답에 도달하는 방법<br>
여러 경우 중 하나를 결정해야 할 때마다 그 수간에 최적이라고 생각되는 것을 선택해 나가는 방식으로 진행해 최종적인 해답에 도달<br>
순간마다 하는 선택은 그 순간에 지역적으로 최적이나, 최종적인 결과가 최적이라고는 보장되지 않음.<br>
> 나무위키에서 인용된 구문에서 마시멜로 실험에 비유된게 인상적이었는데, <br>
> 그리디 알고리즘을 이용하는것은 지금 당장 눈 앞에 있는 마시멜로를 먹는 것으로,<br>
> 이 방법을 이용하는건 "기다렸다 2개를 먹는다"는 최적의 상황을 보장해 주지 못한다는 내용임

## 그리디 알고리즘의 정당성 증명
* 탐욕 선택 속성(greedy choice property)
  * 탐욕적인 선택은 항상 안전하다는 것이 보장되어야 함
  * 항상 모든 단계에서 탐욕적으로 선택한 답이 최적해에 포함되어있다는 뜻
* 최적 부분 구조(optional substructure)
  * 문제에 대한 최종 해결 방법이 부분 문제에 대해서도 또한 최적의 해결 방법이다라는 조건

-> 한번의 선택이 다음 선택에는 전혀 무관한 값이어야 하며, 매순간 최적해가 문제에 대한 최적해여야 한다는 의미<br>
탐욕법을 사용해도 항상 최적해를 구할 수 있는 문제를 만난 경우, 탐욕법은 동적 계획법보다 수행 시간이 훨씬 빠르기 때문에 유용하다<br>

다만, 시간이나 공간적 제약으로 인해 다른 방법으로 최적해를 찾기 너무 어렵다면<br>
최적해 대신 **적당히 괜찮은 답(근사값)** 을 찾는 것으로 타협할 수 있다(최적은 아니지만 임의의 답보다는 좋은 답을 구하는 용도로 잘 쓰인다)

> ### 최적 부문 구조
> 
> <img src="https://w.namu.la/s/f6f9d5e08e9beb596a8d52cdded15bbf5cf921aad3cd579360d23c8a578cd638099c8ce0ae12a11b63b85e68acc8fca2700172d5a45a9d87da2e006996865fe9e937baa7a920a262efe62436c18a8fdb7ebdc7bb65f35284f0d60e1901932740baf489383a36dce8224b01ecc4614622" width="40%">
>
>서울에서 대구, 부산으로 가는 최단경로를 보면 200km + 80km, 280km이다. 서울-대구, 대구-부산의 각 최단경로의 합으로, <br>
문제의 최적 해결 방법은 부분 문제에 대한 최적 해결 방법으로 구성된다. 이러한 구조를 최적 부문 구조라 함

## 그리디 알고리즘을 통한 해결 방법
1. 문제의 답을 만드는 과정을 여러 부분 문제로 나눈다.
2. 각 부분 문제마다 어떠한 우선순위(조건)으로 탐욕적으로 선택할지 결정
3. ‘탐욕적 선택 속성', ‘최적 부분 구조'를 만족하는지 체크 <br> → 두 조건을 모두 만족한다면 **최적해**를 구할 수 있다. 그렇지 않으면 **근삿값**이 도출된다

> ### 근사 알고리즘
그리디 알고리즘은 100% 최적해를 보장해 주지 않는다. 다만, 어느 정도 적합한 수준의 해답을 알려주는데,<br>
탐욕 알고리즘은 근사 알고리즘으로 사용할 수 있다.

### 예시
* 거스름돈 문제
* 회의실 배정 문제 
* 다익스트라 알고리즘