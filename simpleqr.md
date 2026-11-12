---
layout: privacy
app_name: 심플 QR
effective_date: 2026년 5월 25일
updated_date: 2026년 11월 12일

items_intro: |
  본 앱은 이용자의 개인정보를 직접 수집, 저장, 활용하지 않습니다. 다만 서비스 개선 및 통계 분석을 위해 구글의 파이어베이스(Firebase) 라이브러리를 사용하며, 이 과정에서 아래 정보가 구글 측에 수집될 수 있습니다.
items:
  - type: 기기·이용 정보
    data: 개인을 식별할 수 없는 기기 정보 및 앱 이용 기록
    how: Firebase를 통한 자동 수집

purposes: |
  - 서비스 개선 및 통계 분석(Firebase)

retention: |
  본 앱은 개인정보를 직접 수집하지 않으므로, 별도로 보유하거나 파기하는 개인정보가 없습니다. Firebase를 통해 수집된 정보는 구글의 개인정보처리방침에 따라 관리됩니다.

processors:
  - name: Google
    service: Firebase
    task: 서비스 개선 및 통계 분석
    data: 기기 정보, 앱 이용 기록
processors_note: |
  수집된 정보는 구글의 개인정보처리방침에 따라 관리됩니다. ([Firebase 개인정보 보호 안내](https://firebase.google.com/support/privacy))
---
