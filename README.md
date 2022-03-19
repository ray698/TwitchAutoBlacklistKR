## TwitchAutoBlacklistKR
트위치에서 차단 용어를 자동으로 등록해주는 매크로입니다.<br>
매니저 관리 창 -> 차단 용어 등록에서 사용하는걸 기반으로 제작되었습니다.

## 사용하기 전에 필수적으로 해야하는 내용
1. 시작과 종료 키를 제대로 설정했는지 확인한다.
2. 하단의 윈도우 스파이를 사용하여 마우스 커서 좌표를 확인한다.
3. 메모장으로 ahk 파일을 열어서 Click 1575, 814, 0 를 Click x, y, 0 (윈도우 스파이에서 얻은 좌표)로 바꿔준다.
4. 인터넷, 컴퓨터 상황에 맞게 기다리는 시간을 설정 후. 실행한다.

## 코드 사용법 설명<br>

F2:: ;시작 부분입니다.<br>
;F1~F12까지 원하는 단축키로 변경 가능합니다. 예시 : F3 키로 시작하고 싶으면 F3::<br><br>

Clipboard = 10물<br>
;클립보드에 이 내용을 복사합니다.<br><br>
Clipwait<br>
;기다립니다.<br><br>
Send, ^v<br>
;컨트롤 + V<br><br>
Send, {Enter}<br>
;엔터 버튼을 사용합니다.<br><br>
Click 1575, 814, 0<br>
;0의 속도로 마우스 커서를 이동합니다. (Window Spy에서 얻은 좌표값으로 바꿔주세요.)<br><br>
Click<br>
;클릭합니다.<br><br>
sleep, 1200<br>
; 1.2초 동안 기다립니다. 본인의 인터넷, 컴퓨터 상황에 맞게 바꾸어 사용해주세요. (여기서 더 빠르게 하는 것은 권장하지 않음)<br><br>
<br>
F4:: ;종료 부분입니다.<br>
;F1~F12까지 원하는 단축키로 변경 가능합니다. 단, 시작 키와 겹치지 않게 해주세요. 예시 : F3 키로 시작하고 싶으면 F3:: <br><br>

## Windows Spy 사용법

![Window Spy 켜기](https://github.com/ray698/TwitchAutoBlacklistKR/blob/main/WindowsSpy1.png)
<br>
ahk 파일을 실행 후 좌측 하단에서 아이콘을 우클릭.<br>
이후 Window Spy를 선택한다.<br>
<br>
![Window Spy 사용](https://github.com/ray698/TwitchAutoBlacklistKR/blob/main/WindowsSpy2.png)<br>
매니저 창, 차단 용어 탭에서, 초록색 부분으로 마우스를 이동 한다.<br>
Window Spy의 Mouse Position -> Window 의 x, y 좌표 값을 확인한다.<br>
