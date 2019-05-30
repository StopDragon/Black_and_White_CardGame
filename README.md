# Black_and_White_BoardGame
### 한양대학교 CSE1017 프로그래밍기초 1학년 1학기 팀프로젝트
#### TEAM_NAME: 절대태보해@==(^0 ^)@
#### TEAM_MEMBERS: Jung_Ji_Yong, Han_Seung_Woo, Ko_Dong_Woo
#### 
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
