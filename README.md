### about Alzheimer: what factors have a good or bad influence
#### 목적: 알츠하이머에 영향을 미치는 주요 요인 및 습관 분석
#### 분석 tool: pandas
#### 결론: 긍정적인 요인으로는 보유 질환 관리가 있으며 부정적인 요인으로는 급격한 활동 저하와 같은 것들이 있음. 따라서 평소 건강 관리를 잘하는 것이 중요한 것으로 나타남.

알츠하이머병은 기억력과 사고력을 서서히 파괴하고, 결국 가장 간단한 일을 수행할 수 있는 능력을 파괴하는 뇌 질환임. 이 질환을 앓고 있는 대부분의 사람들, 즉 후기 발병 유형의 증상을 가진 사람들은 60대 중반에 처음 나타난다고 함.

alt(alanine aminotransferase)의 수치가 낮을 수록 알츠하이머 병의 발병과 연관성이 깊으며 인지기능저하가 심하다고 함.

##### 해당 데이터는 알츠하이머 환자들을 대상으로 여러 설문조사를 한 데이터로, 여러 습관 혹은 요인들이 alt 수치에 어떠한 영향을 미쳤는지, 즉 알츠하이머에 어떤 영향을 미쳤는지 판단하고자 함.

![image](https://github.com/alwls5773/side-project/assets/66359601/77f59c33-9164-41c4-bbfa-40b7ae67dfd7)
![image](https://github.com/alwls5773/side-project/assets/66359601/6caa254b-e38c-4d0f-aa05-0a8977bacedc)
위의 사진을 통해 나이와 성별은 큰 영향을 미치지 않을 수도 있음을 확인함.

![image](https://github.com/alwls5773/side-project/assets/66359601/10a3b1bc-5a81-416e-a477-1411eca0e578)
전체 평균을 넘는 그룹은 Overall Health 그룹과 Screenings and Vaccines 그룹임. 
Screenings and Vaccines 그룹이 가장 높으며 Overall Health 그룹이 두번째로 높음. 
그 후 Caregiving과 Nutrition/Physical Acticity/Obesity, cognitive decline 그룹 순으로 높지만, 이 세 그룹은 비슷한 수치를 보임. 
smoking and alcohol use와 mental health 그룹이 가장 낮으며, 높은 그룹들과 비교했을 시 확연한 차이가 존재함.

##### 따라서 흡연/음주가 알츠하이머에 가장 안좋은 영향을 미치는 것을 파악할 수 있었고, 비만과 인지저하보다도 멘탈이 안 좋은 것이 알츠하이머에 더 안좋은 영향을 미치는 것을 알 수 있음.

##### 구체적으로 어떤 습관/행동이 알츠하이머에 부정적인 영향을 미쳤는지 파악할 필요가 있음. 

##### class 1. Smoking and Alcohol Use
![image](https://github.com/alwls5773/side-project/assets/66359601/6e1e8ca0-06a7-4af8-9dad-9e9360766afb)

위의 데이터에서 alt가 Current smoking(흡연) 그룹보다 Binge drinking within past 30 days(30일 내 폭음)그룹에서 더 낮은 것을 알 수 있음.
따라서 흡연보다 과음이 알츠하이머에 부정적일 수도 있음.

![image](https://github.com/alwls5773/side-project/assets/66359601/49a300d4-ae10-4e0b-a2d1-8dcb74cffe6e)
##### class 2. Mental Health
Mental Health class 내에서의 분석

위의 데이터에서 alt가 lifetime diagnosis of depression(만성 우울) 그룹보다 Frequent mental distress(빈번한 정신적 고통)그룹에서 더 낮은 것을 알 수 있음.
따라서 만성 우울보다 잦은 우울이 알츠하이머에 부정적일 수도 있음.

##### class 3. Overall Health
![image](https://github.com/alwls5773/side-project/assets/66359601/269f74d6-3868-4548-8c97-efec01d1096a)

alt가 가장 낮게 나타난 그룹은 physically unhealthy days(육체적으로 힘든 날)이며, 그 다음 recent unhealthy days(최근 활동 저하), fall withh injury within last year(부상으로 쓰러짐) 순으로 낮음. alt가 낮게 나온 세 그룹은 흡연, 잦은 우울 그룹과 비슷한 수치가 확인됨.

따라서 육체적으로 힘든 날이 많을 수록 알츠하이머에 안좋은 영향을 미치는 것을 알 수 있음. 급격한 활동 저하와 부상으로 쓰러짐 또한 알츠하이머에 좋지 않은 것을 알 수 있음. 그 영향은 흡연 혹은 잦은 우울과 비슷한 영향을 미칠 수도 있음.

##### class 4. Screenings and Vaccines
![image](https://github.com/alwls5773/side-project/assets/66359601/a0a2376e-7de7-4274-875b-a881c59dbc73)

alt가 낮게 나타난 그룹은 up-to-data with recommended vaccines and screenings - women과 men 그룹임
alt가 높게 나타난 그룹은 cholesterol checked in past 5 years 그룹, cholestrol cancer screening 그룹임

따라서 권장 백신을 접종하는 것보다 당뇨병, 고혈압을 관리하는 것이 긍정적인 영향을 미치며 그 중에서도 콜레스테롤을 관리하는 것이 가장 긍정적인 영향을 미침.

##### 주의
![image](https://github.com/alwls5773/side-project/assets/66359601/7700e5ad-79ad-4643-a24b-4e0d723c1b39)
현재 각 클래스의 표본의 수가 작음. 따라서 클래스 내에서의 분석 결과는 정확하지 않으며, 신뢰도가 떨어지는 경향이 있음. 또한 클래스 간 크기도 동일하지 않으므로 주의해야 함

### 결론
![image](https://github.com/alwls5773/side-project/assets/66359601/81d63933-20bb-494e-98a3-b64bb0dae339)
알츠하이머 환자들에게 운동을 많이 격려하고, 술을 덜 마시는 게 좋을 것이다.

![image](https://github.com/alwls5773/side-project/assets/66359601/0de98f9e-af3a-417f-92ec-55715be75873)
알츠하이머 환자들에게 지속적으로 Cholestreol 수치를 검사하고, 고혈압이 있을 시 약을 잘 복용하도록 격려하는 것이 추천됨
