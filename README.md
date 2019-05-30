# Black_and_White_BoardGame
### 한양대학교 CSE1017 프로그래밍기초 1학년 1학기 팀프로젝트
#### TEAM_NAME: 절대태보해@==(^0 ^)@
#### TEAM_MEMBERS: Jung_Ji_Yong, Han_Seung_Woo, Ko_Dong_Woo
## 게임규칙

1. `player`는 컴퓨터와 게임을 진행합니다.
2. 각자에게 0 ~ 9까지 적힌 타일이 주어집니다. (홀수 타일은 검은색, 짝수 타일은 흰색)
3. 컴퓨터의 타일은 랜덤으로 섞고 타일의 뒷면(색상)을 보여줍니다. 
4. `player`는 타일 뒷면의 색깔을 보고 왼쪽부터 순서대로 숫자를 유추해야합니다. 
5. `round`는 총 10`round`로 진행되며 승점의 합이 더 높은 쪽이 승리하게 됩니다.
6. `round`당 하나의 숫자를 입력하고 프로그램이 입력한 수와 `COM`의 해당 타일을 비교합니다.
7. 타일의 색이 같은 경우 숫자가 높은 쪽이 `score`1점을 획득합니다.
8. 타일의 색이 다른 경우 숫자가 높은 쪽이 `score`2점을 획득합니다.
9. 숫자 0은 숫자9를 이길 수 있습니다.
10. 게임이 끝난 후 `COM`와 `player`의 `score` 차 만큼 `Burrito`를 획득하게 됩니다.
*10 vs 8로 `player`가 이겼다면 10 - 8 = 2 즉, `Burrito`2개를 획득합니다.*
***
## 개발 계획
>`split`
>   >게임 로딩 화면입니다.
>`load_members()`
>   >`members.txt`에서 `player`들의 정보를 `members`에 불러옵니다.
>`login(members)`
>   >`members`에서 아이디와 비밀번호를 비교합니다.
>   >비밀번호가 틀리면 다시 입력할 수 있습니다.
>   >존재하지 않는 아이디를 입력하면 `register()`를 호출합니다.
>`register()`
>   >아이디와 비밀번호를 입력받아 `members`에 추가시킵니다.
>   >비밀번호는 두번 입력받아 사용자가 잘못 입력하는 것을 방지합니다.
>`make_COM_list()`
>   >컴퓨터의 타일을 랜덤으로 섞어줍니다.
>`show_tile`
>   >튜플로 만들어져있는 `COM_list`를 시각화하여 보여줍니다.
>   >ex) □■□□□■■■□■
`store_members(members)`
`show_top5(members)`
`more(message)`
## 기타 개발 주의 사항
모든 입력값 비교는 문자(str)로 비교한다.