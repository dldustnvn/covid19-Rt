# covid19-Rt

## 데이터 불러오기
### 확진자 데이터(covid_data.xlsx)
- 전체 코로나 확진자 데이터
### Wallinga data(Data_infector_infectee_0810.xlsx)
- Wallinga를 계산 할 때에는 infector와 infectee 데이터가 필요하므로 그에 관한 데이터
### 변이 데이터(df_combine_0908.xlsx)
- 각 변이 비율 데이터 * 전체 코로나 확진자 데이터
- 음수 값이 존재하여 내삽을 이용해 보간함
### 부트스트랩 데이터(Rt 전체.xlsx)
- 부트스트랩을 사용하여 생성한 데이터
### 해외 변이 데이터(world_varient.xlsx)
- 일본, 캐나다, 이탈리아, 미국, 영국, 독일, 프랑스


## Rt 방법 세가지
### 내장 함수
- covid19라는 library를 가져와 계산
### cori
- cori method를 사용하여 계산
### Bettencourt
- bettencourt method를 사용하여 계산
### Wallinga
- Wallinga method를 사용하여 계산
- 값이 잘 나오지 않음

## 포스터 그래프
- 포스터를 만들 때 썼던 양식이므로 무시하여도 무관하다.
### result 1 : 국내 변이 시각화
- python으로 계산한 데이터
- R로 만든 데이터 -> python으로 Rt 계산
  - R로  계산한 Rt 값(case_korea_varient.xlsx)이 좀 더 자연스러워 이를 이용하여 다시 시각화한 결과
### result 2 : 해외 변이 시각화
- 일본, 캐나다, 이탈리아, 미국, 영국, 독일, 프랑스
### result 3 : 분포, scattor plot
- Rt mean, std
- Rt mean, covid-19 case mean
- Rt mean, sum of covid-19 case
- frequency plot
- 히트맵 (Rt 시각화)
