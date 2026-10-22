# 나의 공부 계약 — 개인 안드로이드 앱

기존 공부 계약 HTML을 WebView에 포함한 오프라인 개인 앱 프로젝트입니다.

## APK 만들기
1. PC에 Android Studio를 설치합니다.
2. `study_contract_android` 폴더를 Android Studio에서 Open으로 엽니다.
3. Gradle 동기화가 끝나면 Build > Build Bundle(s) / APK(s) > Build APK(s)를 선택합니다.
4. 결과 APK는 `app/build/outputs/apk/debug/app-debug.apk`에 만들어집니다.
5. APK를 본인 휴대폰으로 옮겨 설치합니다. 기기에서 출처별 설치 허용이 필요할 수 있습니다.

## 알아둘 점
- 오프라인 동작, 회원가입 불필요, 서버 전송 없음.
- 앱의 저장소는 기존 Chrome/HTML 파일의 저장소와 다릅니다. 기존 기록은 자동 이전되지 않습니다.
- Android WebView에서는 브라우저용 JSON 다운로드 기능이 기기/버전에 따라 동작하지 않을 수 있습니다. 앱 내부 자동 저장은 WebView 저장소에 남습니다.
- 앱 삭제 또는 앱 데이터 삭제 시 기록이 사라집니다.
- 화면이 꺼져도 경과시간을 시각 기반으로 계산하지만 백그라운드 알림을 보장하지 않습니다.
- 이 폴더는 APK 자체가 아니라 APK를 만들 수 있는 소스 프로젝트입니다.
