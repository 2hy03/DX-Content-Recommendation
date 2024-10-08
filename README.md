# DX-Content-Recommendation

디지털 트랜스포메이션(DX)에 대한 관심이 높아짐에 따라, 관련된 다양한 콘텐츠가 생성되고 있습니다. 이 시스템은 개인의 역량에 맞춰 이러한 콘텐츠를 추천하는 것을 목표로 하고 있습니다.

## 기능

### 콘텐츠 데이터 수집
- **YouTube 크롤링**:
  - BIZ 영역의 DX 이해, DX 태도, Tech 영역의 필요 기술 역량, 최신 기술 활용 역량, 협업 역량 등 주요 카테고리에 맞춰 YouTube 영상 링크를 수집합니다.
  - 수집한 URL을 통해 제목, 날짜, 제작자, 조회수 등의 정보를 추출합니다.
  - 현재, 약 700~800개의 데이터를 수집완료했습니다.
  - 카테고리별 데이터가 충분히 쌓일 경우, 자동 분류 모델 생성을 고려하고 있습니다.

- **GPT-3.5를 활용한 키워드 추출**:
  - 영상의 제목과 설명을 기반으로 DX 관련 키워드를 추출합니다. 이 키워드를 통해 콘텐츠 추천을 목표로 하고 있습니다.

- **클러스터링 및 주제 모델링**:
  - 초기 분류 기준에 따라 클러스터링 기법을 사용하여 데이터를 3~4개의 그룹으로 나눕니다.
  - 토픽 모델링(LDA)을 통해 각 그룹 내 핵심 주제를 파악하고 카테고리를 세분화합니다.
  - 최신 콘텐츠가 지속적으로 수집되면 트렌드 반영에 따라 세부 카테고리도 조정가능합니다.
    ![image](https://github.com/user-attachments/assets/8743b3a3-a226-4985-b7be-ae407c5d59fe)



### TF-IDF 추천
- TF-IDF 방법을 사용하여 키워드 중요도를 바탕으로 콘텐츠를 추천합니다.
- 향후, 데모개발 및 테스터를 통해 Hybrid Recommender System을 목표로 하고 있습니다.
  - ![image](https://github.com/user-attachments/assets/3942f23a-c258-472f-823d-c6c657606cbf)

