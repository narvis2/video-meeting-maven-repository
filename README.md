## 🍎 Jitsi-Meet 기반 화상회의 SDK 화 작업 테스트
- ✔️ Jitsi-Meet Repository 👉 [Jitsi-Meet](https://github.com/jitsi/jitsi-meet) 
### 🍀 Jitsi-Meet Android SDK 화 작업 순서
- 1. [jitsi-Meet git](https://github.com/jitsi/jitsi-meet) 👉 Repository Clone
- 2. cd android
- 3. cd scripts
- 4. sh release-sdk.sh
- ⚠️ 오류 ⚠️
  - 1️⃣ /jitsi-maven-repository/releases: No such file or directory 👉 clone 받은 폴더 내부에 필요한 폴더 생성
    > ✅ **_참고_** ✅
    > - release-sdk.sh 스크립트 성공시 sdk 가 /jitsi-maven-repository/releases 에 생성됨
    > - jitsi-maven-repository 폴더 생성
    > - jitsi-maven-repository 내부에 release 폴더 생성
  - 2️⃣ mvn: command not found 👉 maven 다운로드 및 환경 변수 설정
    > ✅ **_참고_** ✅ [참고 사이트](https://www.digitalocean.com/community/tutorials/install-maven-mac-os)
    >> 나는 development 에 압축 파일 풀고 환경변수 설정함
- 🍬 SDK Version 변경 🍬
  - android > `gradle.properties`
    > - appVersion
    >> - 99.0.0 👉 1.0.0
    > - sdkVersion
    >> - 99.0.0 👉 1.0.0
