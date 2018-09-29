# git 명령어, MarkDown 문법 정리
### 2015261034 백재인
***
## git 명령어 정리
1. **전역 설정 정보 조회**
> git config - -global - -list
2. **전역 설정 정보 삭제시키기**
> git config --global --unset-all user.email

> git config --global --unset-all user.name
3. **새로운 저장소 초기화하기**
> git init
4. **저장소 복제하기**
> git clone <저장소 url>
5. **새로운 원격 저장소 추가하기**
> git remote add <원격 저장소> <저장소 url>
6. **새로운 파일 git에 등록시키기(staging)**
> git add <파일>
7. **현재까지 작업한 내용 저장하기**
> git commit -m “<메시지>”
8. **원격 저장소에서 합치지 않고 지역 브랜치로 변경 사항 가져오기**
> git fetch <원격 저장소>
9. **원격 저장소에서 변경 사항을 가져와 현재 브랜치에 합치기**
> git pull <원격 저장소>
10. **새로운 로컬 브랜치를 원격 저장소에 푸싱하기**
> git push <원격 저장소> <지역 브랜치>
***
## markdown 문법 정리
### 1. **제목(Headers)**
가장 많이 쓰게 되는 서식 중 하나입니다. 제목은 # 문자로 표현합니다.

`# 가장 큰 제목 (H1)`
# 가장 큰 제목 (H1)
`## 두 번째 수준 제목 (H2)`
## 두 번째 수준 제목 (H2)
`### 세 번째 수준 제목 (H3)`
### 세 번째 수준 제목 (H3)
***
### 2. **인용(Blockquotes)**

본문 중 인용된 글을 표시하고자 할 때, > 기호를 모든 줄 앞에 써줍니다.

예)

`> 인용되는 글입니다.`

`> 인용되는 글의 두 번째 줄.`

`> 인용되는 글의 세 번째 줄.`

위와 같이 쓰면 아래와 같이 표시됩니다.

> 인용되는 글입니다.

> 인용되는 글의 두 번째 줄.

> 인용되는 글의 세 번째 줄.

줄 하나하나마다 엔터치지 않고 그냥 한 문단이 길게 이어져 있는 경우에 문단의 맨 앞에 한 번만 > 기호를 넣어줄 수도 있습니다.

예)

`> 두 문단으로 구성된 글을 인용합니다. 두 문단으로 구성된 글을 인용합니다. 두 문단으로 구성된 글을 인용합니다. 두 문단으로 구성된 글을 인용합니다.`

`> 두 문단으로 구성된 글의 두 번째 문단입니다. 두 문단으로 구성된 글의 두 번째 문단입니다. 두 문단으로 구성된 글이 두 번째 문단입니다.`

위와 같이 쓰면 아래와 같이 보이게 됩니다.

> 두 문단으로 구성된 글을 인용합니다. 두 문단으로 구성된 글을 인용합니다. 두 문단으로 구성된 글을 인용합니다. 두 문단으로 구성된 글을 인용합니다.

> 두 문단으로 구성된 글의 두 번째 문단입니다. 두 문단으로 구성된 글의 두 번째 문단입니다. 두 문단으로 구성된 글이 두 번째 문단입니다.

그리고 >> 처럼 꺽쇠 기호를 더하면 들여쓰기 수준이 늘어나게 됩니다. 그리고 인용문 안에서 다른 MarkDown 문법을 중복 적용하는 것도 가능합니다.

예)

`> 인용되는 첫 번째 줄입니다.`

`>> 인용되는 내용 안에서 다시 인용되는 부분입니다.`

`> (인용 수준을 변경할 때 이렇게 빈 줄 하나 넣어줍니다.)`

`> 꺽쇠 한 번만 쓰면 다시 상위 수준으로 표시됩니다.`

`> ## 큰 제목도 인용 안에서 표시 가능합니다.`

위와 같이 쓰면 아래처럼 표시됩니다.

> 인용되는 첫 번째 줄입니다.

>> 인용되는 내용 안에서 다시 인용되는 부분입니다.

> 꺽쇠 한 번만 쓰면 다시 상위 수준으로 표시됩니다.

> ## 큰 제목도 인용 안에서 표시 가능합니다.
***
### 3. **리스트(Lists)**

MarkDown으로 숫자 리스트, 블릿 리스트를 표현할 수 있습니다.

일단 그냥 블릿 리스트를 표현할 때는 *별표시, +플러스기호, -빼기 기호 중 아무거나 쓰시면 됩니다.

예)

`* 고구마`

`* 감자`

`* 옥수수`

이렇게 쓰면 아래처럼 나옵니다.

* 고구마

* 감자

* 옥수수

순서대로 숫자가 매겨지는 리스트는 간단하게 숫자랑 점 찍어서 쓰시면 됩니다.

예)

`1. 고구마`

`2. 감자`

`3. 옥수수`

이렇게 쓰면 아래처럼 나옵니다.

1. 고구마

2. 감자

3. 옥수수

숫자 리스트는 숫자를 순서대로 쓰지 않아도 자동으로 순서대로 바뀌어서 표시됩니다.

예)

`1. 고구마`

`3. 감자`

`5. 옥수수`

이렇게 쓰면 아래처럼 나옵니다.

1. 고구마

3. 감자

5. 옥수수

이렇게 잘 나오게 됩니다.
***
### 4. **코드 블록(Code Blocks)**

키보드 왼쪽 위, 숫자키 1 왼쪽에 있는 역방향 강세기호(`)(=backtick)를 앞 뒤로 써주어서 코드 문자가 코드로 인식되지 않고 문자 그대로 인식하게 해줍니다.

`'<table><tr><td></td></tr></table>'`

위와 같이 쓰면 아래처럼 나옵니다.

`<table><tr><td></td></tr></table>`
***
### 5. **가로선(Horizontal Rules)**

*** 별표 세 개는 수평선으로 삽입됩니다.
***
### 6. **링크 서식**

링크들(Links)

MarkDown 은 링크를 쉽게 생성합니다.

`[링크걸 문구](http://주소)`

예)

`[네이버](http://www.naver.com)`

이렇게 쓰면, 아래처럼 나타납니다.

[네이버](http://www.naver.com)

물론, 상대주소도 가능합니다.

예)

`[소개페이지](/about/about.htm)`
***
### 7. **강조하기(Emphasis)**

가장 많이 사용하게 될 기호가 아닐까 싶습니다.

`*이탤릭*` : 이렇게 별표 하나 사이에 두면 이탤릭체로 표현됩니다.

*이탤릭*

`**볼드**` : 이렇게 별표 두 개 사이에 두면 굵은 볼드체로 표현됩니다.

**볼드**

\* 별표는 _ (언더바)로 대체 가능합니다. 즉, 언더바 두 개 사이에 두면 별표 두 개와 마찬가지로 굵은 글자로 표현됩니다.

`__굵은 글자로__` 표현.

__굵은 글자로__ 표현.

별표나 언더바는 \ 역슬래시 기호 뒤에 쓰면 있는 모습 그대로 표현됩니다. 또한, 앞뒤로 스페이스(공간)가 있을 때에도 본래 모습으로 표현됩니다.
***
### 8. **이미지 삽입(Images)**

사진 하나 넣으려고 할 때 html 태그가 상당히 번거롭습니다. MarkDown 문법에서는 그림이나 사진 삽입 태그를 아래와 같이 사용합니다.

`![사진이름](사진경로)`

![사진이름](사진경로)

사진경로는 http:// 로 시작하는 사진파일 경로 전체를 쓰셔도 되고, title 지정되어 있으면 같은 서버 경로에서 호출해도 됩니다.
***
### 9. **링크 걸기**

먼저, 링크 주소 자체를 클릭할 수 있도록 하려면, 간단하게 <기호와 > 기호 사이에 넣어주기만 하면 됩니다.

`<http://www.naver.com>`

이렇게만 쓰면 아래처럼 표시되는 것이죠.

<http://www.naver.com>

이메일 주소도 꺽쇠 안에 넣어만 주세요.

`<jiback96@naver.com>`

아래처럼 클릭할 수 있게 됩니다. (기본 메일 클라이언트로 연결)

<jiback96@naver.com>
***
### 10. **MarkDown 에 사용되는 기호 표시**

MarkDown 문법에 사용되는 기호를 있는 그대로 출력하고 싶을 때가 있습니다. 예를 들어 # 마크를 그냥 쓰면 실제로는 H1 제목으로 출력되기 때문에 이 기호를 그대로 출력하고 싶다면 기호 앞에 \ 문자를 써주면 됩니다.

앞에 \ 문자를 쓰는 순간 문법 기능으로 쓰이는 대신 기호 모습 그대로 출력되는, 다시 말해서 MarkDown 문법에서 주요하게 사용되는 기호는 다음과 같습니다.

\ (역방향 슬래시) ... 따라서 역방향 슬래시를 그대로 표현하려면 역방향 슬래시 기호를 두 번 쓰면 됩니다. \\\ 이렇게요.

` (backtick = 제2강세 악센트 기호)

\* 별표

_ 언더바

{ } 중괄호

[ ] 대괄호

( ) 소괄호

\# 우물정자

\+ 플러스기호

\- 마이너스 기호

. 마침표

! 느낌표
