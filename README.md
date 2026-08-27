# AI-Subject

## 1차시: 데이터 전처리

---
* 파일 입력 및 출력 처리 복습
* 데이터 전처리(Data Preprocessing) 환경 설정 및 기초 문법
  * Pandas, Excel 라이브러리 설치:
    ```jupyterpython
    %pip install pandas openpyxl
    ```
    * `import pandas as pd`를 통해 라이브러리 호출
    * `pd.tail()`, `pd.head()`를 통해 하위/상위 5개의 행을 출력


## 2차시: 데이터 전처리

---
* **Pandas 문법 기초**:

  * `./assets/my_grade.xlsx` 파일에서 유비, 관우, 장비의 지필평가, 수행평가 점수 및 등급 데이터를 불러와 출력합니다.
  * `./assets/club.xlsx` 파일에서 동아리 데이터를 불러온 뒤, 신규 부원(1학년 김하늘)의 정보를 기존 데이터프레임에 추가(`pd.concat`)합니다.
  * 수정된 동아리 회원 데이터를 `./assets/new_club.xlsx` 파일로 새로 저장하고 불러와 최종 목록을 확인합니다.


## 3차시: 데이터 전처리

---
### 데이터 정렬
1. **정렬**
  * 데이터를 일정한 기준에 따라 순서대로 나열
  * `sort_values()` 사용
    ```jupyterpython
    DataFrame.sort_values(by=[], ascending=True, inplace=False)
```