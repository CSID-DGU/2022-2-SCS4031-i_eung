# 2022-2-SCS4031-i_eung
융합캡스톤디자인 이응팀입니다. 

<br>

## Team 이응
|                김세영                 |                 박세연                |                 유연아                 |               윤서정                |
| :-----------------------------------: | :-----------------------------------: | :------------------------------------: | :----------------------------------: |
|                 팀장                  |                 팀원                  |                  팀원                  |                  팀원                |
| [Seyoung1220](https://github.com/Seyoung1220) | [irina0627](https://github.com/irina0627) | [yeonah98](https://github.com/yeonah98) | [harriet221](https://github.com/harriet221) |

<br>

## HOW TO RUN
### 설치 및 준비
https://nodejs.org/en/ 에서 본인 컴퓨터 버전에 맞는 node를 설치합니다.<br>
```powershell
git clone https://github.com/CSID-DGU/2022-2-SCS4031-i_eung.git
cd 2022-2-SCS4031-i_eung
pip install -r requirements.txt   # 모듈 설치 (시간이 소요될 수 있습니다)
```
### 실행
```powershell
python custom_detect.py --weights best.pt --conf 0.3 --source 0    # 기본 웹캠은 0, 외부 웹캠 연결시 1
node app.js   # 위 detect 명령어 실행중에 다른 터미널에 서버 명령어 실행
```
