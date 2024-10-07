# 가까운 식당 표시 지도 및 알고리즘 개선

## 프로젝트 기간
2021/9/8 ~ 2021/11/23

## 사용 기술
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/> <img src="https://img.shields.io/badge/Jupyter Notebook-F37626?style=flat-square&logo=Jupyter&logoColor=white"/> <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/> <img src="https://img.shields.io/badge/Folium-77B829?style=flat-square&logo=Folium&logoColor=white"/> <img src="https://img.shields.io/badge/geocoder-29A7DF?style=flat-square&logoColor=white"/>

## 내용
알고리즘 강의를 수강하면서 진행했던 프로젝트입니다. 팀원이 크롤링 하여 가져온 식당들의 위치 데이터를 활용하여 현재 위치에서 가장 가까운 식당의 위치를 보여주는 지도 프로그램을 구현하고 총 3회에 걸쳐 속도 개선을 했습니다.
- 1차적으로 속도를 개선한 방법은 무작위로 크롤링 해온 위치 데이터를 정렬하기 전에 가까운 거리, 보통 거리, 먼 거리 3가지로 분류한 뒤 힙 정렬을 진행하여 속도 개선을 이뤄냈습니다.
- 2차적으로 속도를 개선한 방법은 참고한 힙 정렬의 중첩된 for 문의 구조를 변경하여 속도 개선을 이뤄냈습니다.
- 3차적으로 속도를 개선한 방법은 정렬할 데이터 프레임을 생성할 때 이름, 위도, 경도, 거리, 분류등의 컬럼 값을 선언할 때 지정해 주면서 속도 개선을 이뤄냈습니다.

## 파일 요약
- First_Code.ipynb : 맨 처음으로 구현한 프로그램
- Second_Code.ipynb : 1차 개선한 프로그램
- Third_Code.ipynb : 2차 개선한 프로그램
- Final_Code.ipynb : 3차 개선한 프로그램
- restaurant_little.xlsx : 안동시 지역의 식당 엑셀 데이터
- restaurant_average.xlsx : 경상북도 지역의 식당 엑셀 데이터
- restaurant_many.xlsx : 전지역의 식당 데이터 엑셀 데이터
- 가까운 식당 표시 알고리즘 9조.pptx : 프로젝트 발표 ppt

## 프로젝트 결과 

### 최종 개선 결과 및 실행 화면
> ![image](https://user-images.githubusercontent.com/64400731/198871089-ff323b06-0a07-4d8c-ab59-8155b2c6bd0c.png)

### 실행 시간 그래프
> ![image](https://user-images.githubusercontent.com/64400731/198871141-2941e094-aa23-46ab-a9be-f428de6d8557.png)
