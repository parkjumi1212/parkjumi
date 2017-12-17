#ict융합학부2017012897박주미


##오픈소스 소프트웨어 기초

###PBL CASE#1 PROBLEM

당신은 대형 음악서비스 포털인 ㈜KT 뮤직의 전략기획실 신기술개발팀장이다. 최근 대법원 판결(2013 다 219616)에 따라 디지털 음원을 매장에서 재생할 때, 공연보상금을 징수하는 기준이 3,000m2 이상에서 모든 면적으로 확대되었다. 이에 따라 본사는 기존 매장음원서비스인 “샵엔 지니” 서비스를 확장하여 보다 다양한 시장을 확보하고자 2017 년 9 월 6 일 전략기획회의를진행하였다. 회의 결과 별도의 음악 재생용 PC 마련이 곤란한 소형 점포를 위해 저렴한 독립형 뮤직 셋톱박스(standalone music set-top box)를 제공하는 “플러그엔 지니” 서비스를 새롭게 기획하기로 하였다. 이에 신규 서비스의 가능성 타진을 위해 신기술개발팀에서는 ++오픈소스 SW 와 Raspberry Pi 나 비글본 같은 간단한 오픈소스개발보드를 활용하여 최소기능제품(MVP, Minimum Viable Product)을 개발하기로 하였다. ++당신의 팀은 9 월 27 일까지 독립형 뮤직 셋톱박스에 대한 MVP 를 개발하여 시연해야 한다.MVP 는 오픈소스에 기반한 간단한 네트워크 스토리지 서버와 뮤직 플레이어 클라이언트로 구성된다. ==클라이언트는 마지막 재생채널을 기억하고 있다가 전원 연결(플러그인) 시 자동으로 유/무선의 네트워크상에서 서버의 해당채널 음원을 스트리밍하여 3.5mm 오디오 단자로 출력하는 기본 기능을 지원해야 한다. 또한, 현재 재생 중인 채널 및 곡에 대한 간단한 정보를 LED 혹은 LCD 디스플레이 상에 표시하여야 하며, 채널전환 버튼을 통해 손쉽게 음악채널들을 전환할 수 있어야 한다.==

###PBL CASE#1 SOLUTION

![오픈소스 중간결과물.mp4](/Users/parkjumi/Movies/오픈소스 중간결과물.mp4)


###PBL CASE#2 PROBLEM
당신은 대형 음악서비스 포털인 ㈜KT 뮤직의 전략기획실 신기술개발팀장이다. 최근 대법원 판결(2013 다 219616)에 따라 디지털 음원을 매장에서 재생할 때, 공연보상금을 징수하는 기준이 3,000m2 이상에서 모든 면적으로 확대되었다. 이에 따라 본사는 기존 매장음원서비스인 “샵엔 지니” 서비스를 확장하여 보다 다양한 시장을 확보하고자 2017 년 9 월 6 일 전략기획회의를 진행하였다. 회의 결과 별도의 음악 재생용 PC 마련이 곤란한 소형 점포를 위해 저렴한 독립형 뮤직 셋톱박스(standalone music set-top box)를 제공하는 “플러그엔 지니” 서비스를 새롭게 기획하기로 하였다. 이에 신규 서비스의 가능성 타진을 위해 신기술개발팀에서는 오픈소스 SW 와 Raspberry Pi 나 비글본 같은 간단한 오픈소스개발보드를 활용하여 최소기능제품(MVP, Minimum
Viable Product)을 개발하기로 하였다. 당신의 팀은 9 월 27 일까지 독립형 뮤직 셋톱박스에 대한 MVP 를 개발하여 시연해야 한다. MVP 는 오픈소스에 기반한 간단한 네트워크 스토리지 서버와 뮤직 플레이어 클라이언트로
구성된다. 클라이언트는 마지막 재생채널을 기억하고 있다가 전원 연결(플러그인) 시 자동으로 유/무선의 네트워크상에서 서버의 해당채널 음원을 스트리밍하여 3.5mm 오디오 단자로 출력하는 기본 기능을 지원해야 한다. 또한, 현재 재생 중인 채널 및 곡에 대한 간단한 정보를 LED 혹은 LCD 디스플레이 상에 표시하여야 하며, 채널전환 버튼을 통해 손쉽게 음악채널들을 전환할 수
있어야 한다.
__[UPDATED on 9/27]
성공적인 시연 결과, 당신의 팀이 만든 솔루션을 활용하여 본격적인 신규 매장음원서비스를 기획하기로 결정되었으며, 당신을 본부장급 권한을 가진 “플러그엔 지니” 태스크 포스 리더로 임명하여, 신규 사업 승인을 위한 최종 데모를 11 월 15 일 임원회의에서 진행하기로 하였다. ==이에 기획팀, 설계팀 및 디자인팀을 이끌고, 나선형 모델(spiral model)에 입각하여 요구사항 명세서,설계 명세서 등의 적절한 산출물과 함께 구체적인 서비스 기획 및 설계를 진행한 후, 이 시스템에 사용될 케이스와 주변기기에 대한 적절한 디자인을 개발, 3D 프린터로 rapid prototype 를 제작하여 성공적인 신제품 데모를 수행하라.==__

###PBL CASE#2 SOLUTION 
####소프트웨어
1. 기존의 기능 : 이전 곡 재생 , 다음 곡 재생 , 이전 채널 재생 , 다음               채널 재생 
2. 추가된 기능 : 셔플 재생 기능 : 셔플 기능의 ON/OFF 가 가능하며 재생 채널이 바뀌어도 셔플 기능이 사라지지 않는다. 또한 셔플 재생시 이전 곡과 같은 곡은 재생되지 않는다.


####3D 모델링

![그림2.png](/Users/parkjumi/그림2.png)

###결과 동영상


**https://youtu.be/U_atE4m7sHU**


