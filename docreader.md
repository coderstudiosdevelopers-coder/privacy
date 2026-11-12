---
layout: privacy
app_name: 문서 리더(DocReader)
app_desc: 문서 열람 앱
effective_date: 2026년 11월 12일

summary: |
  문서 리더는 회원가입이나 로그인 없이 이용할 수 있습니다. 이용자가 연 문서 파일은 **기기 안에서만 열람**되며, 개발자 서버나 제3자에게 전송되지 않습니다. 다만 앱 개선과 오류 수정, 알림 발송을 위해 Firebase를 통해 앱 이용 통계, 오류 정보, 푸시 알림 토큰이 자동으로 수집됩니다.

items:
  - type: 문서 파일
    data: 이용자가 선택해 연 문서 파일(PDF 등)과 그 내용
    how: 이용자가 직접 선택 (기기 안에서만 열람)
  - type: 앱 이용 정보
    data: 앱 실행·화면 이용 기록, 기기 모델, OS 버전, 앱 버전, 앱 인스턴스 ID
    how: Firebase Analytics를 통한 자동 수집
  - type: 오류 정보
    data: 앱 충돌(크래시) 로그, 오류 발생 당시의 기기·OS 정보
    how: Firebase Crashlytics를 통한 자동 수집
  - type: 알림 정보
    data: 푸시 알림 토큰(FCM 토큰)
    how: 앱 설치·실행 시 자동 생성
items_note: |
  앱은 회원가입·로그인 기능이 없으며, 이름·전화번호·이메일 등 이용자를 직접 식별할 수 있는 정보는 수집하지 않습니다.

storage: |
  이용자가 연 문서 파일은 **이용자의 기기 안에서만** 열람·처리됩니다. 개발자는 문서 파일을 서버로 전송받거나 별도로 저장하지 않으므로 그 내용을 열람할 수 없습니다.

  앱 이용 정보, 오류 정보, 푸시 알림 토큰은 Google이 운영하는 Firebase에서 처리됩니다(아래 '개인정보 처리의 위탁 및 국외 이전' 참고).

purposes: |
  - 기기에 저장된 문서 파일 열람 기능 제공
  - 앱 알림 발송
  - 앱 이용 통계 분석을 통한 서비스 품질 개선(Firebase Analytics)
  - 오류 원인 파악 및 앱 안정성 개선(Firebase Crashlytics)

retention: |
  - **문서 파일:** 이용자의 기기에 저장되며 개발자 서버에는 보관되지 않습니다. 앱을 삭제하면 앱이 기기에 저장한 정보도 함께 삭제됩니다.
  - **Firebase를 통해 수집된 정보:** Google Firebase의 데이터 보관 정책에 따라 일정 기간 보관된 후 삭제됩니다.

processors_intro: |
  앱은 서비스 개선과 알림 발송을 위해 아래 외부 서비스를 이용합니다. **문서 파일과 그 내용은 이 서비스들로 전송되지 않습니다.**
processors:
  - name: Google LLC
    service: Firebase Analytics
    task: 앱 이용 통계 분석
    data: 앱 이용 기록, 기기 정보, 앱 인스턴스 ID
  - name: Google LLC
    service: Firebase Crashlytics
    task: 오류 로그 수집·분석
    data: 크래시 로그, 기기·OS 정보
  - name: Google LLC
    service: Firebase Cloud Messaging
    task: 푸시 알림 발송
    data: 푸시 알림 토큰
overseas: |
  - **이전 국가:** 미국 등 Google 데이터센터 소재 국가
  - **이전 일시 및 방법:** 앱 이용 시 네트워크를 통해 수시로 전송
  - **보유 기간:** Google Firebase의 데이터 보관 정책에 따름
  - **관련 안내:** [Firebase 개인정보 보호 안내](https://firebase.google.com/support/privacy)

  국외 이전을 원하지 않는 경우 앱 이용을 중단(삭제)하여 정보 전송을 멈출 수 있습니다.

third_party: |
  개발자는 이용자의 개인정보를 제3자에게 판매하거나 제공하지 않습니다. 문서 파일은 기기 외부로 전송되지 않으므로 판매·공유가 발생하지 않습니다.

permissions:
  - name: 파일·저장공간
    why: 기기에 저장된 문서 파일 열기
  - name: 인터넷(네트워크)
    why: 이용 통계·오류 정보 전송 및 푸시 알림 수신
permissions_note: |
  권한은 기기 설정에서 언제든지 변경할 수 있습니다.

rights: |
  - 기기 설정의 앱 정보 화면에서 앱 데이터를 삭제하거나 앱을 삭제하면 앱이 기기에 저장한 정보가 삭제됩니다.
  - 알림 수신은 기기 설정에서 해제할 수 있습니다.
  - 그 밖의 개인정보 관련 문의·요청은 아래 문의처로 연락해 주세요.

safety: |
  - 문서 파일은 기기 안에서만 처리하여 외부 전송에 따른 유출 위험을 최소화합니다.
  - Firebase와의 통신은 암호화(HTTPS)된 구간을 통해 이루어집니다.
  - 접근 권한은 서비스 제공에 필요한 최소한의 범위로만 요청합니다.
---
