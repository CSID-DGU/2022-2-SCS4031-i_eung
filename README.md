# 2022-2-SCS4031-i_eung
2022-2 융합캡스톤디자인 이응팀입니다.

<br>

## Team Members
|                김세영                 |                 박세연                |                 유연아                 |               윤서정                |
| :-----------------------------------: | :-----------------------------------: | :------------------------------------: | :----------------------------------: |
|                 팀장                  |                 팀원                  |                  팀원                  |                  팀원                |
| [Seyoung1220](https://github.com/Seyoung1220) | [irina0627](https://github.com/irina0627) | [yeonah98](https://github.com/yeonah98) | [harriet221](https://github.com/harriet221) |

<br>

## Project - 지능형 CCTV 영유아 위험행동 및 상황 감지 시스템

### 아이아이(AI - EYE); 아이들의 안전을 책임지는 인공지능 눈
<br>
<img src="https://user-images.githubusercontent.com/101785754/206646562-9b2f69be-7a4f-4ed4-91d6-b1e0b1809414.png"  width="80%"/>
<br>

### 
### 시스템 구조도
<img src="https://user-images.githubusercontent.com/101785754/206645456-4276a62f-3b4c-4c15-96e2-3eb889232f70.png"  width="70%"/><br>
<br>

### 모델 성능 - best.pt
: <b>[YOLOv5](https://github.com/ultralytics/yolov5)</b> s 기반 모델<br/></br>
<img src="https://user-images.githubusercontent.com/101785754/206645887-b52df3c0-4a09-4ae8-b187-1c19b4849858.png"  width="40%"/><br>
<br>

<br>

## 알림 서비스
- **카톡 알림 서비스**는 아래와 같이 테스트를 완료했지만, 정식 서비스는 추후 사업자 등록이 진행된다면 지속할 계획입니다.<br>
<img width="180" alt="스크린샷 2022-12-06 오전 3 39 25" src="https://user-images.githubusercontent.com/81620424/206842124-8fd43aaa-e827-4321-8fa1-b8e8e3e65fdb.png"> <br><br>
- **프론트 알림 서비스**는 이용이 가능합니다.<br>

<br>

## HOW TO RUN
### 설치 및 준비
https://nodejs.org/en/ 에서 본인 컴퓨터 버전에 맞는 node를 설치합니다.<br>
```powershell
git clone https://github.com/CSID-DGU/2022-2-SCS4031-i_eung.git
cd 2022-2-SCS4031-i_eung
pip install -r requirements.txt   # yolo 모듈 설치 (시간이 소요될 수 있습니다)

npm install express               # node.js 모듈 설치
npm install dotenv
npm install request
npm i socket.io
npm i ejs
```
### 실행
```powershell
python custom_detect.py --weights best.pt --conf 0.3 --source 0    # 기본 웹캠은 0, 외부 웹캠 연결시 1
node app.js   # 위 detect 명령어 실행중에 다른 터미널에 서버 명령어 실행
```

<br>

## License
GPL 3.0
