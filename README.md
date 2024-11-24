# GDGoC Hongik 프로젝트 트랙 3기 미션 코스

안녕하세요, GDGoC Hongik Organizer 이혁입니다.

지난 1주차 미션은 다들 잘 마무리하셨나요? 아무래도 처음 시작하는 미션이다보니 코드보다는 개념적인 내용을 위주로 진행하려 했었어요.

이번에도 물론 아직 배워야 할 개념이 많기에 내용 정리도 하지만, 코드를 짜보는 시간을 가지려 해요. 이번 주차에 배우는 내용이 특히 중요하니 확실하게 진행해주세요!

물론 이번 주차 내용은 저번 주차보다 내용이 많고, 코드를 구현하는 과정에서 마주하는 어려움이 많을 거예요. 하지만 매우 중요한 내용이 많기에 기한을 넘길지언정 끝까지 마무리하시는 걸 권장 드릴게요! 기한까지 열심히 했다는 흔적만 남겨주셔도 다이너마이트 없이 넘어가도록 하겠습니다. (따라서 주기적으로 커밋과 푸시를 남겨주셔야 확인 가능해요.)

또한 지난 주차 과제들을 둘러보고 공통 피드백을 작성해봤어요. 공통 피드백은 디스코드 공지에 추후에 따로 첨부해드릴테니 읽어보시고 이번에 한번 적용해보아요!

참고: 프론트엔드 트랙은 다른 트랙과 다르게 매 주차마다 새로운 레포지토리가 개설돼요. 매번 Fork하고 Clone해야하니 이 점 유의해서 진행해주세요.

> **안내 사항**
>
> - 최하단에 기재된 [폴더 구조](#폴더-구조) 형식에 맞춰서 파일을 만들어주세요.
> - 레포지토리를 Fork한 이후, 최대한 빠른 시일 내에 PR을 올려주세요. 이후 Push를 진행해도 되니 운영진이 미션 진행 여부를 확인할 수 있도록 해주세요.
> - 레포지토리는 무조건 Public으로 Fork해주세요. Private으로만 진행하면 운영진이 과제 피드백에 어려움을 겪을 수 있어요.
> - 이번 주에 배우는 내용들도 블로그에 꼭 회고록과 함께 정리해주시고, 해당 링크를 제출해주세요.
> - [GitHub 과제 제출 가이드라인](https://www.gdschongik.com/project-track/3/guide/github)을 준수하여 진행해주세요.

## [기초 미션] GitHub를 비효율적으로 이용하자.

> **학습 목표**
>
> - GitHub에서 Branch를 어느 정도는 다룰 수 있다.
> - Commit Message를 최대한 자세하게 작성해보자.

지난 세션에서 전달해드린 것처럼, 프로젝트 트랙에서는 GitHub를 비효율적으로 이용하는 걸 권장하고 있어요. 이번에는 협업에서 GitHub를 활용하기 위해서 미리 알아둬야 할 것들을 확인해보려 해요.

Branch를 다루는 방법에 대해서는 게임을 통해 배워볼 거예요. 그리 어렵지 않으니 시간 날 때 천천히 클리어 해봅시다. Git의 기본적인 명령어들을 배우는데 도움될 거예요. 해당 게임을 클리어하고 사진을 찍어서 블로그에 함께 업로드 해주세요.

[Branch 게임 사이트](https://learngitbranching.js.org/?locale=ko)

또한 모든 Commit을 작성할 때 Commit Convention을 적용해봐요. 아무렇게나 커밋 메세지를 작성하는 것이 아닌, 조금 더 어떤 코드를 작성했는지에 초점을 맞춰 작성하는 연습을 해봐요. 만약 어떻게 작성해야 할지 감이 잡히지 않는다면 아래 가이드라인과 GDG 선배들의 레포지토리를 참고해봐요.

[커밋 컨벤션 작성 가이드라인](https://velog.io/@shin6403/Git-git-%EC%BB%A4%EB%B0%8B-%EC%BB%A8%EB%B2%A4%EC%85%98-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0)

[와우온보딩 Client 레포지토리](https://github.com/GDSC-Hongik/gdsc-client)
[와우클래스 Client 레포지토리](https://github.com/GDSC-Hongik/wow-class)

추신: Commit Message를 작성할 때 꼭 여려 줄로 작성할 필요는 없어요. 한 줄로 적더라도 어떤 컨벤션이 있는 지 파악해보는 정도면 충분해요. 실수로 컨벤션을 지키지 못해서 생기는 패널티는 없으니 최대한 연습하는 방향으로만 진행하면 돼요.

- [ ] Branch 게임을 끝까지 진행하고 사진을 찍어서 블로그에 업로드해주세요.
- [ ] 모든 Commit Message를 작성할 때 Commit Convention을 지키며 작성해주세요.

## [메인 미션 1] HTTP에 대해 이해해보자.

> **학습 목표**
>
> - 프론트엔드와 백엔드가 어떤 규칙으로 소통하는지 알 수 있다.
> - HTTP 요청과 응답 과정에서 필요한 정보들이 무엇인지 알 수 있다.

홈페이지 주소에 적힌 HTTP는 어떤 의미를 가질까요? 아마 데이터통신을 수강하신 분들은 어느 정도 알고 계시겠지만, 이를 어떻게 코드에 적용할 수 있는지를 배워보려 해요.

우선 HTTP에 대한 이해를 필요로 하기 때문에 기본적인 내용을 공부해야 해요. 기본적으로 웹에서 프론트엔드와 백엔드가 어떻게 통신하는지를 이해해봅시다. 아래 글 외에도 추가적으로 공부해주세요!

[프론트엔드와 백엔드의 소통](https://zero-base.co.kr/event/media_insight_contents_BE_backend_Connection)

간단히 정리하자면 **프론트엔드**는 백엔드에서 받은 정보를 가공하고 보여주는 역할을 하고, **백엔드**는 프론트엔드에서 요청한 내용을 기반으로 데이터베이스를 다루고 정보를 전달해주는 역할을 해요. 그래서 우리는 이 프론트엔드와 백엔드가 소통하는 규약에 대해 알아보려 해요.

- [ ] HTTP Response와 Request에 대한 내용을 공부하고 정리해요.
  - [ ] HTTP Method(GET, POST, DELETE, PATCH 등)들에 대한 내용을 공부하고 정리해요.
  - [ ] HTTP Status(200, 404 등)들에 대한 내용을 공부하고 정리해요.

각각의 내용은 지난 번처럼 본인이 몰랐거나, 중요한 내용 위주로 정리하면 돼요. 기본적인 소통 흐름을 파악해두어야 다음 주 미션을 진행하는데 지장이 없으니 특히 HTTP Method에 대한 내용은 확실하게 공부해두면 좋을 거 같아요.

## [메인 미션 2] 비동기 처리를 이해해보자.

> **학습 목표**
>
> - 동기 처리와 비동기 처리의 차이점이 무엇인지 알 수 있다.
> - 콜백 함수가 무엇인지 알고, Promise가 작동하는 방식을 이해할 수 있다.
> - fetch로 받아오는 JSON이 어떤 형식인지 알고, 데이터를 읽어올 수 있다.
> - `async`/`await`을 이용한 비동기 코드를 작성할 수 있다.

동기 처리와 비동기 처리가 무엇일까요? 간단하게 설명드리자면 **동기 처리**는 동시에 여러 작업을 처리하는 것이고, **비동기 처리**는 한번에 하나씩 순서대로 처리하는 방식이에요. 동기 처리로 한 번에 여러개를 처리하면 당연히 효율적으로 보이지 않나요?

하지만 웹에서 통신하는 것은 통신하는 동안 딜레이가 있기 때문에, 우리가 요청한 값이 도달하기 전에 다른 코드도 함께 실행되어 원치 않은 값에 접근하는 일이 벌어질 수 있어요. 따라서 우리는 강제적으로 통신을 마무리하고, 다음 절차로 넘어가는 코드를 작성해야 할 때가 있어요.

[동기와 비동기, Promise, async/await](https://velog.io/@khy226/%EB%8F%99%EA%B8%B0-%EB%B9%84%EB%8F%99%EA%B8%B0%EB%9E%80-Promise-asyncawait-%EA%B0%9C%EB%85%90)

[자바스크립트의 콜백 함수](https://www.freecodecamp.org/korean/news/https-www-freecodecamp-org-news-javascript-callback-functions-what-are-callbacks-in-js-and-how-to-use-them/)
[콜백 함수 개념 및 응용](https://inpa.tistory.com/entry/JS-%F0%9F%93%9A-%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EC%BD%9C%EB%B0%B1-%ED%95%A8%EC%88%98)

[자바스크립트 Fetch](https://www.daleseo.com/js-window-fetch/)

위 글에서 이번 미션에서 배워야할 내용이 모두 정리가 되어 있어요. 추가적인 공부와 함께 각각의 내용을 공부해보고, 아래 조건에 부합하도록 코드를 작성해주세요.

### 요구 사항

- async/await으로 이루어진 함수에, fetch를 이용하여 `https://jsonplaceholder.typicode.com/posts/`에서 데이터를 가져오는 코드를 작성한다.
- 받아온 데이터 리스트에서 각 객체의 title 프로퍼티를 모두 출력한다.

```bash
# 출력 예시
sunt aut facere repellat provident occaecati excepturi optio reprehenderit
qui est esse
ea molestias quasi exercitationem repellat qui ipsa sit aut
...

```

- [ ] 동기/비동기 처리, Promise, async/await 등 이번 미션에서 새롭게 배우게 된 내용을 정리해요.
- [ ] `asynchronous.js`에 요구 사항에 맞도록 코드를 작성해요.

## [메인 미션 3] React에서 페이지를 구성해보자.

> **학습 목표**
>
> - Yarn을 이용하여 React 프로젝트를 만들 수 있다.
> - react-router-dom 라이브러리를 통해 페이지를 이동할 수 있다.

지난 미션에서는 React를 이용하여 컴포넌트를 만들고, 화면에 띄우는 과정까지를 진행해봤어요. 이번에는 그 페이지들을 실제로 옮기는 과정을 진행해볼 거예요.

먼저, 저번에는 CRA(create-react-app) 방식으로 React 프로젝트를 만들었었죠? 이번에는 Yarn이라는 방식으로 프로젝트를 만들어보려 해요. 방식은 크게 다르지 않아서 그리 어렵지 않게 만들 수는 있겠지만, CRA방식과 다른 명령어들이 존재하니 주의해주세요.

> **왜 다른 방식을 이용하나요?**
>
> React로 프로젝트를 생성하게 되면 node_modules 라는 폴더가 생기게 돼요. 여기에 이용하는 모든 라이브러리가 들어가게 되는데, Yarn의 방식으로 프로젝트를 만들게 된다면 조금 가볍게 프로젝트를 관리할 수 있어요.

프로젝트를 만들고 나서, 각각의 기능을 하는 페이지를 만들어 볼 거예요. 해당 기능을 이용하기 위해서는 `react-router-dom` 라이브러리를 설치하고 이용해야 해요.

1. 다른 페이지들로 이동할 수 있는 Button 컴포넌트들이 있는 페이지 (`/`)
2. 본인 블로그로 이동할 수 있는 `Link`가 있는 페이지 (`/blog`)
   - div 태그 안에 `Link`를 위치해주세요.
3. 본인이 가장 좋아하는 사진이 담긴 img 태그가 있는 페이지 (`/picture`)

위 페이지들을 각각 구현해주시고, 뒤에 있는 경로로 이동할 수 있도록 설정해주세요.

- [ ] Yarn을 이용한 방식으로 React 프로젝트를 세팅해요.
- [ ] react-router-dom 라이브러리를 활용하여 각 페이지를 구현하고, URL로 이동해요.

## [서브 미션] CSS를 더욱 편하게 이용해보자.

CSS로 페이지를 꾸밀 때 항상 `.css` 파일을 만들어서 진행하지 않았었나요? 매번 className 속성을 다르게 지정해줘야 하고, 파일도 항상 새로 만들어야 하는 불편함이 있어요. 또한 CSS를 정적으로 관리해야 한다는 점도 단점이 될 수 있어요.

따라서 이를 해결하기 위한 방법이 있어요.

1. .module.css
2. emotion.js / styled component

둘다 알아보고 편한 방법을 취하시면, 더욱 편하게 CSS를 관리할 수 있어요. 저는 개인적으로는 2번을 추천드리긴 하지만 직접 이용해보시고 어떤 편리함이 있는 각각 체험해보면 좋을 거 같아요.

서브 미션은 메인 미션이 마무리되고, 시간이 남으신 분들이 진행하시면 돼요. 조금더 효율적인 코드를 짜는 경험을 할 수 있을 거예요.

- [ ] [메인 미션 3](#메인-미션-3-react에서-페이지를-구성해보자)에서 작성한 코드에 스타일을 추가해요.

## 폴더 구조

```bash
├── README.md
│
├── mission1
│   └── WIL.md
│
├── mission2
│   ├── WIL.md
│   └── asynchronous.js # 비동기 처리 코드 파일
│
└── mission3
    ├── node_modules
    ├── package-lock.json
    ├── package.json
    ├── public
    └── src
        ├── App.css
        ├── App.js
        ├── # 각 페이지별로 파일을 분리해서 진행해주세요.
        ├── index.css
        └── index.js
# 명세 외의 파일이 추가적으로 있어도 상관없습니다만, 너무 많은 파일이 추가적으로 생기지 않도록 해주세요.
```