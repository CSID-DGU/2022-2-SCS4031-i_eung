# 2022-2-SCS4031-i_eung
융합캡스톤디자인 이응팀입니다.


```powershell
git clone https://github.com/CSID-DGU/2022-2-SCS4031-i_eung.git
pip install -r requirements.txt  #모듈 설치 (시간이 소요될 수 있습니다)
cd 2022-2-SCS4031-i_eung
python custom_detect.py --weights best.pt --conf 0.3 --source 0   #기본 웹캠은 0, 외부 웹캠 연결시 1
node app.js #위 detect 명령어 실행중에 다른 터미널에 서버 명령어 실행
```
