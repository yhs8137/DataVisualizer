# AUIGrid 기본 예제

AUIGrid 3.0.18 문서의 Quick Start를 바탕으로 만든 Vanilla JS 예제입니다.

## 포함 기능
- 칼럼 레이아웃 정의 (숫자 `#,##0`, 날짜 포맷)
- 셀 편집, 상태 칼럼(`showStateColumn`)
- `cellClick`, `cellEditEnd` 이벤트
- 행 추가(`addRow`) / 삭제(`removeRow`)
- 변경 내역 조회(`getAddedRowItems`, `getEditedRowItems`, `getRemovedItems`)

## 실행 방법
AUIGrid 엔진은 상용 라이브러리라 저장소에 포함하지 않습니다.
보유한 엔진 파일을 프로젝트 루트의 `AUIGrid/` 폴더에 넣으세요.

```
DataVisualizer/
├─ AUIGrid/
│  ├─ AUIGridLicense.js
│  ├─ AUIGrid.js
│  └─ AUIGrid_style.css
└─ examples/basic/
   ├─ index.html
   └─ data.js
```

`AUIGridLicense.js`는 접속 도메인(브라우저 주소창의 호스트명)을 검사하므로
`file://`로 직접 열지 말고 로컬 웹 서버로 띄워 라이선스에 등록된 도메인으로 접속하세요.

```bash
# 프로젝트 루트(DataVisualizer/)에서 실행
npx serve -l 8080 .
# 또는
python3 -m http.server 8080
```

브라우저에서 `http://localhost:8080/examples/basic/` 로 접속합니다.
라이선스가 `localhost`를 허용하지 않으면 등록된 도메인을 hosts 파일로 127.0.0.1에 매핑해 접속하세요.
