# [React / VanillaJS] UI 요소 직접 만들기 Part 1
인프런 [정재남님 강의](https://www.inflearn.com/course/react-vanillajs-ui%EC%9A%94%EC%86%8C%EB%A7%8C%EB%93%A4%EA%B8%B0-part1)를 듣고 기록합니다.

### 커밋유형

| 커밋유형     | 의미                       |
|----------|--------------------------|
| feat     | 새로운 기능 추가                |
| fix      | 버그 수정                    |
| chore    | 그 외 자잘한 수정               
| style     | CSS 수정 및 업데이트                    |
| docs     | 문서 생성                    |
| refactor | 리팩토링                     |
| rename   | 파일 또는 폴더 명을 수정하거나 옮기는 작업 |
| remove   | 파일을 삭제                   |


## [ UI요소 만들기 강의 코드 ]

### 디렉토리 구조

- `app`: app 전반에 대한 기본 view 제공
    - `[...item]/page.tsx`: `/[...item]` route의 page view. `routes`의 `key`에 매칭된 컴포넌트를 렌더링.
    - `layout.tsx`: 기본적인 html 구성
    - `page.tsx`: `/` route의 page view. `/README.md`를 보여줍니다.
    - `global.scss`: app 전반의 style
    - `gnb.tsx`: 좌측 메뉴 컴포넌트
- `components`
    - `vanillaWrapper.ts`: 독립적인 VanillaJS 환경의 wrapper 컴포넌트
- `routes.ts`: route 구성

### Getting Started

- 다운로드 받은 파일의 압축을 해제하고, 터미널에서 해당 폴더로 이동합니다.

```bash
cd ui-study
```

- npm module 설치를 진행합니다.

```bash
npm install
# or
pnpm install
# or
yarn
```

- 개발 서버를 실행합니다.

```bash
npm run dev
# or
pnpm run dev
# or
yarn dev
```

- 브라우저에서 [http://localhost:3000](http://localhost:3000)에 접속
