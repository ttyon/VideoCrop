# VideoCrop
- 비디오 crop 및 merge
- video event annotation 생성 기능
- video frame 추출 후 저장 기능
- frame별 object tagging 기능
- frame에 object detection 기능

## Requirements
- python 3.6
- pyqt 5
- ffmpeg
- k-lite codec pack ( http://www.codecguide.com/download_kl.htm )
- requirements.txt 참조 

## How to use
### video crop and merge
<img width="926" alt="KakaoTalk_20200923_174424241" src="https://user-images.githubusercontent.com/46225226/93990911-a746ac00-fdc6-11ea-8432-c693abd204e7.png">

1. 영상에 자를 비디오 선택
2. 비디오 목록에서 삭제
3. 리스트에서 더블클릭하면 영상 재생 준비
4. 이벤트 추가 및 삭제, 삭제하려면 삭제하려는 이벤트 선택해야함
5. 자르기 전에 json에 입력할 이벤트 선택, 선택된 이벤트는 빨간색으로 변함
6. 영상 준비가 되고 누르면 영상 재생
7. crop할 시작시점 설정, 옆 input 칸에서 입력 가능
8. crop할 종료시점 설정, 옆 input 칸에서 입력 가능
9. 영상이 선택되고, 이벤트가 선택되면 crop list에 추가
10. crop list에 있는 목록들을 수정 가능. ▲, ▼ 눌러 순서 변경 가능, refresh 눌러 cutList 초기화, 초기화는 영상을 다 만들고 나서 초기화버튼을 누른다.
11. cut list에 있는 목록들을 random 배치, video 생성, json 생성
-> video, json을 생성할 때 반드시 파일 이름에 .mp4, .json이 들어가야함
12. 옆 칸을 통해 원하는 프레임을 추출하거나, 그냥 tagging 툴로 이동


* * *

### object tagging
<img width="960" alt="KakaoTalk_20200923_174424241_01" src="https://user-images.githubusercontent.com/46225226/93990988-be859980-fdc6-11ea-8fae-91155b88edf8.png">

##### 단축키
- w : label 크기 설정, w 누르고 마우스 클랙 앤 드래그 하면 label 생성
- a : 이전 이미지
- d : 다음 이미지
- space : json 저장, label이 지정되어 있지 않은 공간을 한 번 누르고 space를 눌러주세요.

1. object annotation을 저장할 폴더를 우선 선택한다. 파일 기반으로 이루어진 툴이기 때문에 먼저 선택해야한다. -> 선택되면 빨간색으로 표시
2. 다음 이미지 표시 (단축키: d)
3. 이전 이미지 표시 (단축키: a)
4. object detection 기능, 자동으로 설정한 폴더에 json파일이 저장된다.
5. label을 수정한 후에 누르면 지정된 폴더에 자동 저장
6. 추출된 frame들을 볼 수 있다.
7. label을 수정하는 곳. label 이동, label 수정, 삭제 가능
8. description을 볼 수 있는 곳, label을 누르고 더블클릭하면 수정된다.
9. description 수정
10. 해당 image에 있는 label을 관리 하는 곳, 더블클릭하면 해당 label을 선택하고, 옆 체크박스로 visible을 관리할 수 있다.
11. 해당 image에 있는 모든 label을 visible, unvisible 할 수 있는 버튼
 

