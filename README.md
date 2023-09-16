## PMV-PPD Calculator
PMV-PPD를 계산하는 계산기입니다. 

본 계산기는 ASHRAE Standard 55-2020의 PMV-PPD 계산 코드를 참고하여 만들어졌습니다.

(추가로 수정될 수 있습니다.)

## 사용법
현재 서버를 통해 배포하지 않기 때문에, 직접 다운로드 받아서 사용하시면 됩니다.  

1. 먼저 GitHub 우측 상단에 Code 버튼을 눌러 Download ZIP을 통해 파일을 받습니다.  
2. .zip 파일을 받았으면, 압축을 해제하고 하나의 폴더에 모든 폴더를 넣습니다.  
3. 폴더 내에 있는 main.html 파일을 실행하면 계산기가 웹페이지로 실행됩니다.  

## csv 파일 형식
이 계산기는 csv 파일을 넣어 각 행마다 PMV 및 PPD를 계산하여 결과값으로 출력할 수 있습니다.  
csv 파일의 모양은 다음과 같은 모양을 가지고 있으면 됩니다.

|Time(index)|Ta|MRT|Vel|RH|MET|CLO|WME|
|---|---|---|---|---|---|---|---|
|value|value|value|value|value|value|value|value|
|value|value|value|value|value|value|value|value|
|value|value|value|value|value|value|value|value|

## Input Value
PMV-PPD 계산에 필요한 필수 값과 단위는 다음과 같습니다.
- Ta    : 공기온도 (Air Temperature) [°C]
- Tr    : 평균 복사 온도 (MRT, Mean Radiant Temperature) [°C]
- Vel   : 기류 속도 (Relative Air Speed) [m/s]
- RH    : 상대 습도 (Relative humidity) [%]
- MET   : 대사율 (Metabolic Rate) [met]
- CLO   : 의복량 (Clothing) [clo]
- WME   : 추가 활동(?) 기본값 0 (External Work, Default 0) [met]

## Reference
- ASHRAE Standard 55-2020