# Weather_Fairy


## 🧑‍🤝‍🧑 Team Members (구성원)
<table>
  <tbody>
    <tr>
     <td align="center" valign="top" width="14.28%">
       <a href="https://github.com/Luna828">
       <img src="https://avatars.githubusercontent.com/u/93186591?v=4" width="100px;" alt="김은경"/>
       <br />
         <sub>
           <b>김은경</b>
         </sub>
       </a>
       <br />
       <sub>
           <b>iOS Developer</b>
       </sub>
       <br />
     </td>
    <td align="center" valign="top" width="14.28%">
       <a href="https://github.com/angwoo0503">
       <img src="https://avatars.githubusercontent.com/u/136118540?v=4" width="100px;" alt="박상우"/>
       <br />
         <sub>
           <b>박상우</b>
         </sub>
       </a>
       <br />
       <sub>
           <b>iOS Developer</b>
       </sub>
       <br />
     </td>
      <td align="center" valign="top" width="14.28%">
       <a href="https://github.com/chumubird">
       <img src="https://avatars.githubusercontent.com/u/138557882?v=4" width="100px;" alt="박철우"/>
       <br />
         <sub>
           <b>박철우</b>
         </sub>
       </a>
       <br />
       <sub>
           <b>iOS Developer</b>
       </sub>
       <br />
     </td>
      <td align="center" valign="top" width="14.28%">
       <a href="https://github.com/dnjs012452">
       <img src="https://avatars.githubusercontent.com/u/139090550?v=4" width="100px;" alt="원성준"/>
       <br />
         <sub>
           <b>원성준</b>
         </sub>
       </a>
       <br />
       <sub>
           <b>iOS Developer</b>
       </sub>
       <br />
     </td>
  </tbody>
</table>

## 🖥️ TEAM APP Project - Weather_Fairy
스파르타코딩 iOS_7기 iOS심화 팀프로젝트 `떡잎마을 방범대` 입니다

저희 팀은 이번 3가지 주제중 4명에게 부족한 API 공부를 위하여 `날씨 App`을 진행하기로 하였습니다.

**앱 구성 : 보라색 하이라이트 → 기능 핵심**
 
- UI를 구성하는 Item들을 `모듈화`시켜 하나의 MainWeatherView에 옮김
     
     → VC에서 `loadView`에 `view = mainWeatherView` 로 view를 씌워주기
     
 - 검색 기록을 저장하기 위한 수단 = `UserDefault` 사용
 - 가져와야할 api 정보
     - 현재기온
     - 최고/최저 기온
     - 지역 이름
     - 대기질
     - 바람
     - 습도
     - 강수확률
 - 강수확률에 따른 준비물 `알림`기능 추가
 - `MapKit` 라이브러리 사용하여 현재 위치 보이기
 
 개발기간: 2023/09/25 월요일 ~ 2023/10/05 목요일

발표: 2023/10/06 금요일


## 👨‍💻 역할분담 및 프로젝트 주요기능 
* [TEAM S.A](https://www.notion.so/S-A-1f9f48c90f2b49b6a6a4a3e2cda18086)

### 김은경
- currentWeatherViewItem  -> UIViewItem 분리 중 한개
- myLocationViewItem -> UIViewItem 분리 중 한개
- MapKit 내부 라이브러리 사용 -> 현재 위치 서비스 및 위치 정보 Authorization 허용
- Error Handling -> Enum Type 생성
- Google Font 다운로드
- GitHub PR 지도 및 Conflict/Merge 정리
- README 초안 작성
  
### 박상우
- 도시 검색 페이지 제작
- 사용자의 입력을 받아 검색 기능 구현
- OpenWeather API를 호출해 검색 도시들의 날씨 출력 기능 구현
- UserDefaults를 활용한 검색 기록 저장 구현
  
### 박철우
- push notification 기능 ( api에서 필요한 데이터 가져와서 해당 데이터를 이용한 알림 생성 호출)
- SceneDelegate에서 background에서 알림을 받을수있게 설정
- appDelegate에서 알림 허용 설정기능 // 어플이 실행된 직후에  단 한번 보여줄 알림 처리할수있는 기능
  
### 원성준
- 메인 현재 위치 기온 섭씨, 화씨 단위 변환
- 메인 현재 위치, 기온, 기상상태 openweathermap api 설정
- 메인 현재 위치에 대한 일출시간, 바람, 습도, 일몰시간 api 설정
- 메인 현재 위치에 대한 5일간, 3시간 간격 기상예보 api 설정

## ⚡️ 팀 규칙
```text
1. 아래의 Git Convention 지켜서 commit과 PR 요청하기! 
git commit -m "[FEAT] : ⚙️ commit init"

2. 스크럼: 오전 9시 30분
3. Pull Request: 오후 8시

4. 자리비울 때 말하기 (개인사정)
5. 이슈 트랙킹/트러블슈팅시 질문하기
```
## ⚙️ Requirements

- 최소 iOS 14.0 +

- Xcode 14.3.1

- 필수 구현 기능(필수)
    - [x]  사용자 위치 지정
    - [x]  날씨 데이터
    - [x]  사용자 입력 (SearchPage 검색창)
    - [x]  날씨 표시
    - [x]  단위 변환
    - [x]  사용자 친화적인 인터페이스
    - [x]  데이터 새로 고침
    - [x]  배경 이미지
    
- 추가 구현 기능(선택)
    - [x]  알림
    - [x]  예보 (3시간별, 5일간)
    - [x]  위치 서비스
    - [x]  지도 통합
    - [x]  검색 기록
    - [ ]  애니메이션
    - [x]  디자인 패턴 (MVVM)
    
- **GIT**
    - [x]  git add / commit / push 활용
    - [x]  git 브랜치/ PR / merge 활용
    - [x]  github pull request에서 Code review 활용

## ✏️ 와이어프레임
  <table>
    <tr>
      <td>
        <img src="https://github.com/iOS-Oppenheimer/Weather_Fairy/assets/93186591/d61440c8-6d28-4f95-8ff8-d12b6406dd37"/>
      </td>
      <td>
        <img src="https://github.com/iOS-Oppenheimer/Weather_Fairy/assets/93186591/b90a5003-4326-4904-9c44-e3efda574e67"/>
      </td>
      <td>
        <img src="https://github.com/iOS-Oppenheimer/Weather_Fairy/assets/93186591/5af549eb-ff7a-4afd-9eb6-5fc073411814"/>
      </td>
    </tr>
  </table>

  <table>
    <tr>
      <td>
        <img src="https://github.com/iOS-Oppenheimer/Weather_Fairy/assets/93186591/b112fa1e-10ca-4612-a115-2933f56bcaae"/>
      </td>
    </tr>
  </table>

  <table>
    <tr>
      <td>
        <img src="https://github.com/iOS-Oppenheimer/Weather_Fairy/assets/136118540/5e1baa94-e60d-43c6-af39-b6d24fa96ef1"/>
      </td>
    </tr>
  </table>


## ⭐️ YOUTUBE 시연영상 ⭐️
[![Video Label](http://img.youtube.com/vi/CG0sDbMho24/0.jpg)](https://youtu.be/CG0sDbMho24)

## 📚 Library
```text
//외부 라이브러리
https://github.com/SnapKit/SnapKit

//내부 라이브러리
import UserNotifications
import MapKit
```

## 🔥 Project Issue 🔥

[🚨MapKit - 현재 내 위치 버튼 버그 수정하기🚨](https://github.com/iOS-Oppenheimer/Weather_Fairy/issues/45)

[🚨SearchPage에서 키보드가 내려간 후 셀 터치 미작동 문제 #46🚨](https://github.com/iOS-Oppenheimer/Weather_Fairy/issues/46)

[🚨Push Notification 관련 문제 ( 불필요하게 여러번 실행) #50🚨](https://github.com/iOS-Oppenheimer/Weather_Fairy/issues/50#issue-1927566970)



## 🍰 추후 보완하거나 시도해보고 싶은 Point🪡
- 현재 위치 누를 때 -> Mapkit만 바뀌는게 아니라 전체 값이 변경됐으면 함
- Searchpage에서 Cell 클릭시 background image 나오는 중간에 검은색 화면이 노출됨
- 검색 했을 때 Cell 개별로 UI 업데이트를 하는 것이 아니라 전체 Cell이 업데이트 됐을 때 TableView에 출력이 됐으면 함
- Constant 사용하기

## 🍎 회고 & 느낀점
### 김은경
```text
이번 iOS 7기 심화 프로젝트에서 날씨 앱을 만들어보기로 결정했다.
프로젝트가 시작하기 전주에 개인공부 한주가 있었는데, 팀 프로젝트가 다가오기 전에 Slack으로 소통하여 미리 github organization과 repo를 미리 만들어두는 작업을 하여
팀 프로젝트 시작하고 나서 시간적인 부담을 좀 줄이도록 노력하였습니다. 

긴 추석 연휴가 있음에도 불구하고 자신의 시간들을 쪼개서 자신의 할 일에 대해 미루지 않고 열심히 해온 것이 제 의욕을 더 북돋아주었고,
열정적으로 프로젝트에 임해준 것에 대해서 다들 존경스럽고 너무 감사했습니다! 
다들 2주 동안 팀 스크럼에 한번도 빠지지않고 참여해주셔서 의욕 넘치게 이번 프로젝트 잘 마무리할 수 있어 매우 만족스럽고 또 감사했습니다 여러붕!!
(글 실력이.. 여기까지인가봐요.. 더 잘 쓰고 싶었는데 ㅠㅠ)

또한, 제가 한 것 중에서 느낀점과 보완해야할 점에 대해서 쓰겠습니다!
첫 번째로, 이번 팀프로젝트에서는 4명이서 2페이지를 공동 작업했기 때문에 Git 충돌에 유의하면서 작업을 진행하였고,

자신이 쓴 코드를 잘 숙지해서 충돌시 해결에 있어 큰 어려움 없이 넘어갔던 점이 매우 좋았던 것 같습니다. → 소통에 문제가 없었던 점이 우리 조의 큰 자랑입니다!

두 번째로는 Xcode에 내장되어져있는 Mapkit 사용 방법 및 위도 경도에 따라서 지도를 표시할 수 있는 법과 MapAnnotation을 사용해서 custom할 수 있는 법에 대해서 알 수 있는 좋은 경험이었다

세 번째로는 UIViewItem별로 나눠서 하나의 View에 모아서 코드를 작성하였다.

UIKit을 코드로만 작성하여 뷰를 만들다 보니 코드가 매우 방대해져서 가독성이 좋지 않다고 생각하여 팀원들과 함께 코드를 나눠서 합치는 작업을 해보았습니다 → 다른 방법은 뭐가있을 지 추후에 더 생각해보면 좋을 것같습니다! 

마지막으로, 처음에 MapKit 사용할 때 두개의 생성자를 만들어놓고 사용해서 하루를 날렸던 점.. 중복사용 주의..해야할 것같습니다!! (다음부터 실.수 안하기..)
```
  
### 박상우

```text
이번 날씨 프로젝트를 진행하며 좋은 팀원들을 만나 즐거운 프로젝트를 진행할 수 있었다.

내가 맡은 역할은 검색 페이지 제작과 검색에 관련된 여러 기능들의 구현이었다.

프로젝트를 진행하며 내가 느낀 다섯 가지에 대해 말해보자 한다.

첫 번째, Git의 Rebase에 대해 알게됐다. 우리 팀원 중 은경 님이 Git 전문가였다. Git 전략 중 Rebase를 활용하는 법을 알려주어 Git 그래프를 굉장히 깔끔하게 관리할 수 있었다.

또한 형상 관리 도구인 Fork의 사용법도 알려주어 더 편리하게 Git을 이용할 수 있게 됐다.

두 번째, API 사용에 익숙해졌다. 지금까지 프로젝트를 진행해오며 내가 나서기보다 남은 것들을 해왔기에 메인 아이템을 손대기가 어려웠다.

이번 2주간 운 좋게 API를 호출하고 받은 데이터를 가공하며 어느정도 API를 사용할 수 있게 됐다.

세 번째, MVVM 패턴은 아직 어렵다. 아직 모델-뷰-뷰 모델을 나누는 개념 확립이 덜 된 것 같다.

뷰에서는 UI 관련 코드만 들어가야하는데 자꾸 뷰 모델의 역할이 들어가는 것 같아 MVVM과 데이터 흐름에 대한 추가적인 학습이 필요하다.

네 번째, 터치 이벤트에 대해 생각해보게 됐다. 이번 트러블 슈팅에서도 작성했던 내용이지만 iOS에서는 조금 복잡한 원리로 사용자의 제스쳐를 처리한다.

사용자 경험이 더 편리하고 완성도 있는 앱을 만드려면 제스쳐에 대한 공부도 불가피하다.

마지막 다섯 번째, 좋은 팀원들이 있으면 무서울게 없다. 은경, 철우, 성준이라는 멋진 팀원들과 같이 2주간 열심히 달려오며 많은 문제들에 부딪혔지만 서로 머리를 맞대고 해결하면 안 풀릴 문제가 없다는 걸 깨달았다.

못난 팀장 때문에 고생한 우리 떡잎방범대에게 미안한 마음을 전한다.

추석 연휴 동안에도 열심히 달려와준 은경 님, 철우 님, 성준 님 고생 많으셨습니다. 네 명이 이렇게 열심히 톱니바퀴처럼 굴러가는 팀은 또 처음이었네요.

파이널 프로젝트 때 지금같은 열정과 더 나아진 실력으로 훨훨 날아다니시길 바랍니다. 파이팅!
```

### 박철우
```text
이번 13조에 배정되고 나서 총기간 개인과제 2주 + 팀과제 2주를

존경하는 저희 팀 구성원 , 팀장 상우님 , 팀원 성준님 그리고 은경님 세분과 함께

공부+팀 미니 프로젝트를 하게되어서 너무 즐거웠습니다 !

개인 과제 2주간에도 매일 각자 공부한것과 풀어나가야할 개인과제들을 서로 어떠한 방식으로 해쳐나갔는지

공유하며, 뭔가 시도해보고싶었지만 기회가없었거나 아직 그 부분들에대한 공부가 부족해서 못해본것들을 

팀원분들의 과제 + 리뷰 등을 통해서 간접적으로 알게되고 시도해보고 하는대에 큰 도움이 되었습니다.

또한, 개인주차때도 틈틈히 팀과제 주차때를 대비해서 서로 미리 합을 맞추기위해서 소통하고 사전 준비를 매일 조금씩

부담안되는 선에서 잘 조율이 되어서 너무 만족스러웠습니다.

팀과제 주차때는 추석 연휴가 있었음에도 불구하고 모두 짧거라 길게라도 팀원분들을 서로 먼저 배려하며 시간을 내서

작은 부분이라도 같이 함께 진행하고 크고 작은 문제들이 생길때도 서로 고민하고 이끌어주는 팀 협업 방식에 큰 동기부여가 되었습니다.

이번 날씨어플관련 팀과제에서 푸쉬알림 기능을 맡아서 하게되었는대, 개인적인 호기심으로 스스로 자처해서 하겠다고 했을때, 

팀원분들이 믿고 맡겨주셨고, 맡은 기능 구현을 진행하면서 appDelegate, sceneDelegate 파일들도 좀더 관심있게 살펴보게되고

또 직접적인 api기능을 다루진 못했지만 , 알림 기능을 생성할때 api 데이터를 받아서 처리해볼수있는 작은 부분들도 시도해볼수있어서

의미있는 시간이었습니다.

또 깃 관련부분에서도 모르는게 여전히 많지만 이번 팀원분들과 과제를 진행하면서 좀더 알아가게되었고 깃을 조금씩 알아갈수록

팀플래이에 재미가 더 상승하는거같단 느낌이 들었습니다.
```

### 원성준
```text
발제가 주어지고 이번 팀프로젝트때 개인마다 하고 싶은 목표나 사용해보고 싶은 기능들을 정하고 의견을 취합해서 프로젝트를 기획하여 진행하였고

이전 프로젝트 기간보다 기간이 긴 프로젝트이므로 어떻게 진행할지 다같이 계획하는 부분에 있어서 모두 굉장히 집중도 있게 진행하여

너무 만족스러웠습니다.
첫번째로는 이전 프로젝트 진행하면서 API를 사용하지 못하여 이번 기회에 API를 사용해보았습니다. 처음 API를 호출하고 데이터를 가공해보았는데

처음에는 호출하는 부분에 있어서 어려움을 겪었지만 팀원분들께서 API 사용하는 부분을 참고도 하고 여러번 사용해보니 어느정도 사용법을 알게되어

만족했습니다.

두번째로는 현재 MVVM패턴에 대해 이해도가 부족한 상황에 은경님께서 MVVM 틀을 마련해주셨고 분리하는 과정에서 상우님께서 도움을 주셔서 조금

패턴에 가까워진거 같아서 감사했습니다.

이번 프로젝트 진행에 있어서 팀원 한분 한분 모두 서로에게 신경쓰며 배려해주어 서로 부족한 부분을 채워주고 문제가 생겼을때 다같이 확인하고

체크하면서 진행했던 부분들이 프로젝트를 잘 마무리하는데에 큰 부분을 차지했던거 같고 팀프로젝트에 있어서 굉장히 좋은점이라고 생각합니다.

정말 쉼없이 2주간 열심히 열정적으로 달려오신 우리 상우님, 은경님, 철우님께 대단하고 존경한다는 말씀드리고 싶습니다.

이번에 수월하게 API를 사용하는 부분과 완벽하게 구현하지 못한 부분이 있어 아쉬웠고 다시한번 아직 부족하는걸 느껴 더욱 열심히 파고

들어야겠다는 생각이 들었습니다. 그리고 프로젝트 진행하면서 프로젝트를 완성하는데에 많이 부족했을텐데 미안하고 모두 감사하다고 전하고 싶습니다.

매일매일 새로운 경험이었고 문제가 발생했을때 풀어나가는 부분과 새로운 기능을 사용하는 부분에 있어서 정말 많이 배웠습니다.

다시 한번 이번에 함께해주신 철우님, 은경님, 상우님께 감사합니다.
```
