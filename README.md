# SAS Hackathon 2023: South Korea's Fertility Decline Feature Analysis

## 개요
이 프로젝트는 SAS 해커톤 2023에 제출된 작품으로, 한국의 출산율 감소에 대한 사회적, 경제적, 인구학적 요인을 분석하여 그 원인과 영향을 파악하는 것을 목표로 합니다.

## 팀 소개
**K-Analysts**  
팀원:
- Victor Ahn
- Federico Chung
- Sebin Lee
- Yongjung Lee
- Jangwon Yun

## 프로젝트 정의

### 문제 정의
한국은 OECD 국가 중 10위의 GDP를 자랑함에도 불구하고, 지속 가능한 출산율 유지에 어려움을 겪고 있습니다. 2013년 이후로 한국의 출산율은 OECD 국가 중 최저를 기록하고 있으며, 2022년에는 0.78로 떨어졌습니다. 본 프로젝트는 이러한 저출산 문제를 해결하기 위해 사회적, 경제적, 문화적 요인을 종합적으로 분석합니다.

### 연구 질문
- 한국의 출산율 감소에 가장 큰 영향을 미친 요인은 무엇인가?

### 프로젝트 목표
1. 한국의 출산율 감소에 가장 큰 영향을 미친 주요 요인을 규명합니다.
2. 출산율 감소를 완화하기 위해 상위 요인들을 무효화할 수 있는 방안을 제시합니다.
## 사용된 데이터

| 데이터 파일 이름 | 설명 | 출처 |
| ---------------- | ---- | ---- |
| `merged_dataset.csv` | 분석에 사용된 병합 후 필터링 된 데이터셋으로 다양한 사회적, 경제적, 인구학적 변수를 포함합니다. | OECD 데이터베이스 |

### 주요 변수 설명

| 변수 이름 | 설명 |
| --------- | ---- |
| `fertility_rate` | 출산율 |
| `suicide_rate` | 자살률 (인구 100,000명 당) |
| `education_rate` | 교육 수준 (고등 교육을 받은 인구 비율) |
| `population_density` | 인구 밀도 (제곱 킬로미터 당 인구) |
| `gender_wage_gap` | 성별 임금 격차 (남성과 여성의 평균 임금 차이) |
| `crude_divorce_rate` | 조이혼율 (인구 1,000명 당) |
| `life_expectancy` | 기대수명 (평균 수명) |
| `median_age` | 중위 연령 |
| `median_age_bearing` | 출산 중위 연령 |
| `housing_prices` | 주택 가격 지수 |
| `internet_access` | 인터넷 접근 비율 |
| `spending_on_education` | 교육 지출 (GDP 대비 비율) |

이 데이터는 한국의 출산율 감소에 영향을 미칠 수 있는 다양한 요인을 포함하고 있으며, 이를 분석하여 주요 영향을 규명하고자 했습니다.

## 데이터 분석

### 분석 방법
- 사용 기술: SAS Viya, Google Colab(Python), Excel
- 데이터 출처: OECD 데이터베이스
- 분석 방법: 머신러닝 알고리즘 (랜덤 포레스트, 라쏘 회귀, 선형 혼합 효과) 및 통계적 분석

### 주요 결과
1. **자살률**: 출산율에 가장 큰 상관관계를 가지고 있는 변수로 확인됨. 자살률이 높을수록 출산율은 낮아지는 경향을 보임.
4. **성별 임금 격차**: 큰 상관관계를 가지고 있는 변수로 확인됨. 성별 임금 격차가 클수록 출산율이 낮아지는 경향을 보임.

## 연구 결과
- 한국의 출산율은 1950년대 이후 지속적으로 감소하여 현재 OECD 국가 중 최저 수준입니다.
- 자살률과 출산율 간의 명확한 상관관계를 발견했습니다. 자살률이 높은 한국은 출산율이 매우 낮습니다.
- 이러한 결과는 한국이 생활하기에 특히 도전적이고 스트레스가 많은 국가임을 시사하며, 이는 출산율 감소에 기여할 수 있습니다.

## 제안
1. 공공 교육의 질을 향상시켜 사교육의 필요성을 줄입니다.
2. 주택 우선 분양 및 자녀 지원 정책을 강화합니다.
3. 블라인드 채용을 통해 교육 수준과 관계없이 공정한 채용 기회를 제공합니다.

## 한계
- 역사적 사건, 결혼 및 출산에 대한 문화적 태도, 성 역할 변화, 사회적 압력 및 개인적 선호도와 같은 정량화하기 어려운 요인들이 존재합니다.
- 본 연구는 출산율 감소와 관련된 요인 간의 인과 관계를 확립하지 못했습니다.

## 추가 연구
- 질적 연구를 통해 정량화하기 어려운 추가 변수를 포함하고 데이터 분석을 수행합니다.
- 지연 변수를 사용하여 출산율에 미치는 영향을 분석합니다.
- 대체 방법을 확립한 후 연구하여 정확한 출산율 하락과의 인과 관계를 확립합니다.

## 데이터 파일
- `merged_dataset.csv`: 분석에 사용된 병합된 데이터셋
- `SAS Hackathon 2023.ipynb`: 데이터 분석에 사용된 Jupyter 노트북

## 참고 문헌
- Jeong, K., Yoon, J., Cho, H. J., Kim, S., & Jang, J. (2022). The Relationship Between Changes In The Korean Fertility Rate And Policies To Encourage Fertility. BMC Public Health, 22(1), 2298.
- Kim, A. M. (2020). Factors Associated With The Suicide Rates In Korea. Psychiatry Research, 284, 112745.
- OECD (2023). "Family Indicators" OECD Social and Welfare Statistics.
- Yun, J., Kim, C. Y., Son, S. H., Bae, C. W., Choi, Y. S., & Chung, S. H. (2022). Birth Rate Transition in the Republic of Korea: Trends and Prospects. Journal of Korean medical science, 37(42), e304.