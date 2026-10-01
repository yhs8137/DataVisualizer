# AUIGrid 기본 예제

AUIGrid 3.0.18 문서의 Quick Start를 바탕으로 만든 Vanilla JS 예제입니다.

## 포함 기능
- 칼럼 레이아웃 정의 (숫자 `#,##0`, 날짜 포맷)
- 셀 편집, 상태 칼럼(`showStateColumn`)
- `cellClick`, `cellEditEnd` 이벤트
- 행 추가(`addRow`) / 삭제(`removeRow`)
- 변경 내역 조회(`getAddedRowItems`, `getEditedRowItems`, `getRemovedItems`)

## 실행 방법
AUIGrid 엔진은 비상업용 CDN(jsDelivr, `aui-community/auigrid-noncommercial`)에서 불러오므로
별도 파일 설치가 필요 없습니다.

> 비상업용 배포본입니다. 상업적 용도로 쓰려면 정식 라이선스 엔진으로 교체하세요.

## 실행 방법 (중요)
비상업용 라이선스(`AUIGridLicense.js`)의 허용 도메인은 `localhost`, `127.0.0.1` 뿐입니다.
반드시 로컬 웹 서버로 띄워 접속하세요.

```bash
# DataVisualizer/ 루트에서
npx serve -l 8080 .
```

브라우저에서 `http://localhost:8080/examples/basic/` 로 접속합니다.

### `AUIGrid is not defined` 에러가 날 때
CDN 의 `AUIGrid.js` 가 로드되지 않은 것입니다.
- 개발자 도구 Network 탭에서 `cdn.jsdelivr.net` 요청이 실패(차단/404)했는지 확인
- 사내망·방화벽에서 jsDelivr 가 막혀 있지 않은지 확인
- 에디터/앱의 미리보기 패널처럼 외부 스크립트나 `eval` 을 막는(CSP) 환경이 아닌 일반 브라우저에서 열기
