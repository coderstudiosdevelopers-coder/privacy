---
layout: privacy
app_name: 심플메모(SimpleMemo)
effective_date: 2026년 7월 12일
updated_date: 2026년 11월 12일

items:
  - data: 메모, 할 일, 일정 내용
    why: 앱 핵심 기능 제공
    where: 기기 로컬 (구글 계정 백업 시 이용자의 구글 드라이브 앱 전용 저장공간)
  - data: 기기 식별자, 앱 사용 로그
    why: 이용 통계 분석 및 서비스 개선(Firebase Analytics)
    where: Google(Firebase)
  - data: 오류 및 충돌 로그
    why: 오류 진단 및 안정성 개선(Firebase Crashlytics)
    where: Google(Firebase)
  - data: 푸시 알림 토큰
    why: 알림 발송
    where: Firebase, Supabase
  - data: 카메라로 촬영/선택한 사진
    why: 메모 첨부 기능
    where: 기기 로컬
  - data: 마이크 음성
    why: 음성 입력을 텍스트로 변환
    where: 기기 로컬 (변환 후 음성 데이터는 저장하지 않음)
  - data: 광고 식별자
    why: 광고 제공 및 맞춤 광고(광고 SDK 사용 시)
    where: 제휴 광고 네트워크
  - data: 구글 계정 정보(이메일 등 기본 프로필)
    why: 구글 드라이브 백업/복원 로그인
    where: Google

retention: |
  앱을 삭제하면 기기에 저장된 메모·일정 데이터는 함께 삭제됩니다. 구글 드라이브에 백업한 데이터는 이용자가 직접 삭제하기 전까지 이용자의 드라이브에 보관됩니다. 분석·로그 데이터는 각 서비스(Firebase 등)의 보관 정책에 따릅니다.

processors_intro: |
  앱은 서비스 운영을 위해 다음 업체에 개인정보 처리를 위탁합니다.
processors:
  - name: Google
    service: Firebase
    task: 이용 통계 분석, 오류 진단, 알림 발송
  - name: Google
    service: Google Drive API
    task: 구글 드라이브 백업/복원
  - name: Supabase
    task: 알림 토큰 동기화

third_party: |
  개발자는 법령에 특별한 규정이 있는 경우를 제외하고 이용자의 개인정보를 외부에 판매하거나 제공하지 않습니다.

sections:
  - title: 구글 드라이브를 통한 백업
    body: |
      이용자가 설정 화면에서 "구글 계정으로 내보내기"를 실행하면, 앱의 메모·일정 데이터가 이용자 본인의 구글 드라이브 내 앱 전용 저장공간(appDataFolder)에 저장됩니다. 이 공간은 앱 자신만 접근할 수 있으며, 이용자의 다른 드라이브 파일에는 접근하지 않습니다. 백업 데이터는 이용자가 "가져오기"를 실행할 때만 앱으로 다시 불러와지며, 이용자가 언제든지 자신의 구글 계정에서 앱 연결을 해제하거나 백업을 삭제할 수 있습니다.

rights: |
  이용자는 언제든지 앱 내 설정에서 백업 데이터를 삭제하거나, 구글 계정 설정에서 앱의 접근 권한을 해제할 수 있습니다. 개인정보 관련 문의, 열람, 삭제 요청은 아래 이메일로 연락해 주세요.
---
