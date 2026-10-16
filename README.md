# 회날먹 · 회사 일도 날로 먹고 싶다

아무 키나 두드리면 보고서, 엑셀, 메일, PPT, 코드, 영상 편집이 알아서 진행되는 '일하는 척' 화면입니다.
손을 떼고 15초가 지나면 자동 근무가 시작됩니다.

만든 곳: 히피썬 게임즈

## 파일

| 파일 | 내용 |
|---|---|
| `index.html` | 사이트 전체 (파일 하나로 동작) |
| `og.png` | X·카카오톡 등에 링크를 붙였을 때 뜨는 미리보기 이미지 (1200×630) |

## 주소

https://hipythongames.github.io/hoenalmeok/

저장소 이름이나 주소를 바꾸면 `index.html` 머리말의 미리보기(og) 주소 3군데도 함께 바꿔 주세요. 끝의 `/`까지 넣어야 `og.png` 경로가 맞습니다.

## 고칠 곳

**크레딧과 링크** — `index.html`에서 `SITE_CONFIG`를 찾아 채웁니다.

```js
const SITE_CONFIG={
  maker:'',      // 만든 사람
  bio:'',        // 한 줄 소개
  link:'',       // 만든 사람 링크 (https://)
  donateUrl:'',  // 과자 사주기 송금 링크 (https://)
  formUrl:''     // 건의 받을 구글 폼 등 (https://)
};
```

비워 둔 항목은 화면에서 '준비 중'으로 나옵니다. 링크는 `https://`로 시작해야 합니다.

## GitHub Pages 설정 (처음 한 번)

1. GitHub에서 새 저장소 `hoenalmeok`을 Public으로 만듭니다.
2. `index.html`, `og.png`, `README.md`를 저장소에 올립니다 (Add file → Upload files).
3. Settings → Pages → Branch를 `main`, 폴더를 `/ (root)`로 두고 Save.
4. 1~2분 뒤 `https://<GitHub 아이디>.github.io/hoenalmeok/`에서 열립니다.

## 알아 둘 점

- 건의함 저장, 크레딧 편집 기능은 claude.ai 안에서만 동작합니다. 여기서는 `SITE_CONFIG`의 `formUrl`로 건의를 받습니다.
- 이름, 직군 같은 설정은 방문자 각자의 브라우저에만 저장됩니다.
- 화면 속 회사, 사람, 숫자, 메일은 모두 지어낸 것입니다.
