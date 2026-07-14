# 표 뷰어 (xlsx / xls / xlsm / csv / tsv)

브라우저 안에서만 동작하는 스프레드시트 뷰어.
**파일은 서버로 전송되지 않습니다.** 모든 파싱이 로컬에서 이뤄지며, 앱 자체를 내려받은 뒤에는 네트워크 요청이 발생하지 않습니다. (개발자도구 → Network 탭에서 확인 가능)

## 배포 방법 (택 1)

### GitHub Pages
1. 새 저장소 생성 → 이 폴더의 `index.html`, `manifest.webmanifest`, `sw.js` 업로드
2. Settings → Pages → Source: `main` / `(root)` → Save
3. 1~2분 뒤 `https://<계정>.github.io/<저장소>/` 접속
4. 그 URL을 즐겨찾기 (PC가 초기화돼도 URL만 있으면 복구 완료)

### Netlify Drop (계정 없이 즉시)
https://app.netlify.com/drop 에 이 폴더를 드래그 → 즉시 URL 발급

### 사내 웹서버 / 공유 폴더
파일 3개를 그대로 복사. `https://`가 아니면 오프라인 캐시(PWA)만 비활성화되고 나머지 기능은 동일하게 동작.

## 사용
- 페이지 열고 파일을 창에 끌어다 놓기 (또는 "파일 열기")
- 브라우저 메뉴 → "앱으로 설치" 하면 아이콘 생성 + 오프라인에서도 실행

## 기능
xlsx / xls(BIFF8) / xlsm / csv / tsv · 셀 서식 · 조건부 서식 · 병합 · 틀 고정 ·
숫자·날짜 서식 · 정렬 · 검색 · 범위 선택 합계/평균 · CSV 저장 · 다크/라이트
