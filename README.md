# NetflixUI
Clone Netflix UI

<img width="469" alt="스크린샷 2022-07-04 오후 11 07 14" src="https://user-images.githubusercontent.com/87454813/177171172-f819c5e3-12bb-4784-9af7-f679a8ae823d.png">

1. 넷플릭스 UI 버튼 안에 이미지 크기 맞춰서 넣는 방법: 

버튼 속성 = type은 커스텀, style은 default 로.

이렇게 하면 일단 네모난 버튼 안에 이미지 크기가 대충 맞춰 넣어짐.
-> 이것도 아닌가보다.. 두번째 이미지부턴 이게 안먹힘 ..

2. UI버튼 둥글게 만들기
방법은.. ?

<img width="398" alt="스크린샷 2022-07-04 오후 11 11 42" src="https://user-images.githubusercontent.com/87454813/177172082-af07f706-4b25-4021-a9bf-e176dd16bc34.png">

왜 안될까..?

A. cornerRadius를 설정하더라도 속성이 적용되지 않는 뷰가 있다.

view 에서 drawing의 clipsToBounds 기본값이, 뷰 객체 종류마다 다르게 설정되어있기 때문

이거 체크표시해야 적용이 됨! 또는 코드에서 clipsToBounds  = true 로 해주어야됨.
