---
layout: privacy
app_name: 읽어주는 앱
effective_date: 2026년 6월 24일
updated_date: 2026년 11월 12일

items_intro: |
  앱은 직접적으로 이용자의 개인식별 정보(이름, 이메일, 전화번호 등)를 수집하지 않습니다. 다만, 아래의 서비스 운영 목적으로 자동 수집 정보가 발생할 수 있습니다.
items:
  - type: 기기 정보
    data: 기기 모델, OS 버전, 앱 버전
    how: Firebase를 통한 자동 수집
  - type: 앱 사용 로그
    data: 화면 조회, 기능 사용 빈도
    how: Firebase Analytics를 통한 자동 수집
  - type: 오류 정보
    data: 오류 및 크래시 로그
    how: Firebase Crashlytics를 통한 자동 수집

purposes: |
  - 앱 서비스 제공 및 기능 개선
  - 오류 분석 및 안정성 향상
  - 사용 통계 분석 (익명 집계)

retention: |
  자동 수집된 로그 및 분석 데이터는 Firebase 정책에 따라 최대 14개월간 보관 후 자동 삭제됩니다. 앱 자체적으로 별도 서버에 개인정보를 저장하지 않습니다.

processors_intro: |
  본 앱은 Google의 Firebase 서비스를 사용하며, 각 기능은 아래 목적으로 데이터를 수집합니다.
processors:
  - name: Google LLC
    service: Firebase Analytics
    task: 앱 사용 패턴 분석 및 서비스 개선
    data: 익명화된 사용 데이터
  - name: Google LLC
    service: Firebase Crashlytics
    task: 앱 충돌(크래시) 발생 시 오류 로그 수집, 버그 수정 및 앱 안정성 개선
    data: 기기 정보 및 스택 트레이스 (개인 식별 정보 미포함)
processors_note: |
  Firebase Analytics로 수집된 데이터는 Google의 서버에 저장되며, 개인을 특정할 수 없는 형태로 처리됩니다. Firebase의 데이터 처리 방침은 Google의 개인정보처리방침을 따릅니다: [https://policies.google.com/privacy](https://policies.google.com/privacy)

third_party: |
  앱은 이용자의 정보를 제3자에게 판매하거나 임의로 제공하지 않습니다. 다만, Firebase 등 서비스 운영에 필요한 위탁 처리 업체(Google LLC)에 한하여 해당 서비스 범위 내에서 처리될 수 있습니다.

rights: |
  이용자는 다음 권리를 행사할 수 있습니다.

  - 개인정보 처리 현황 열람 요청
  - Firebase Analytics 비활성화: 기기 설정 → Google → 광고 → 광고 ID 재설정 또는 삭제
  - 앱 삭제 시 앱 내 로컬 데이터는 완전히 삭제됩니다
---
