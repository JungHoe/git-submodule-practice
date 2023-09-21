# git-submodule-practice

서브모듈 기능 연습

## 사용법

### 1. 서브모듈 추가하기

> git submodule add `<remote repository>`

<img src="https://github.com/JungHoe/git-submodule-practice/assets/51188350/c2c36a78-95c4-45c9-b484-9d954b35cc60" width="1200" height="300"/>

### 2. 모듈 clone 하기

> git submodule update -- init

### 3. clone 이후 branch checkout

`detached HEAD` 이슈를 방지하기위해 branch checkout 해준다.

> git submodule foreach git checkout dev

## 소스작업방법

### 1. 서브Repository 에서 Feature branch 생성

> git checkout -b feature/dev-something origin/dev

### 2. 변경사항 커밋 후 push

> git add .
>
> git commit -m "something changed..."
>
> git push

### 3. Feature -> dev PR 작성 및 Merge

### 4. 로컬에서 dev pull 받고 parent 소스에서 diff 파일 커밋 후 push

## 후기

- 생각보다 불편하다. 웹 예시들처럼 credential 파일을 private repo에 처리할때 사용하면 괜찮을것같음
- 프론트에 적용하기는 의문이 드네요...

## 참고 자료

- [Git submodule 사용하기](https://pinedance.github.io/blog/2019/05/28/Git-Submodule)
