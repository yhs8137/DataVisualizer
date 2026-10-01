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

그 다음 `examples/basic/index.html`을 브라우저로 열면 됩니다.
(데이터는 `data.js`에 들어 있어 `file://`로 열어도 동작합니다.)
