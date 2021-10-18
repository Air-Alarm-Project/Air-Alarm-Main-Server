# Air-Alarm-Main-Server

## 개발환경

- Pycharm, Python 3.9
- Raspberry Pi
- Flask
- SQLITE3

## 파일/폴더 안내
- main : 플라스크를 이용해 REST API를 구현하는 핵심 소스코드
### API 폴더
- dust : 공공데이터포털 미세먼지 API 연동 소스코드
- weather : 공공데이터포털 기상청 기상정보 API 연동 소스코드
### DB 폴더
- STM32 : STM32 모듈과의 시리얼 통신을 통해 센서값을 읽어오는 소스코드
- insertToDB : 읽어온 센서값과 API를 통해 받은 기상 정보 등을 DB에 저장하는 소스코드
- getFromDB : DB에 저장된 값을 읽어들여 반환하는 소스코드
### IP 폴더
- iptemp : 내부, 외부 아이피를 반환하는 소스코드
- insertToDB : 메인 서버와의 통신을 통해 아이피를 전송하는 소스코드
