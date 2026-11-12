# 앱 개인정보처리방침

CoderStudios 앱들의 개인정보처리방침을 이 레포 하나에서 관리합니다.
새 앱이 생기면 레포를 새로 만들지 않고 **앱 파일(.md) 하나만 추가**하면 됩니다.

- 링크 형식: `https://coderstudiosdevelopers-coder.github.io/privacy/<파일 이름>`
- 전체 목록: https://coderstudiosdevelopers-coder.github.io/privacy/

## 앱 목록

| 앱 | 파일 | 새 링크 | 기존 링크(옛 레포) |
|---|---|---|---|
| 문서 리더 | `docreader.md` | https://coderstudiosdevelopers-coder.github.io/privacy/docreader | (신규) |
| 하루사주 | `saju.md` | https://coderstudiosdevelopers-coder.github.io/privacy/saju | https://coderstudiosdevelopers-coder.github.io/saju/ |
| 스톡메이트 | `stockmate.md` | https://coderstudiosdevelopers-coder.github.io/privacy/stockmate | https://coderstudiosdevelopers-coder.github.io/StockMate/ |
| 심플메모 | `simplememo.md` | https://coderstudiosdevelopers-coder.github.io/privacy/simplememo | https://coderstudiosdevelopers-coder.github.io/SimpleMemo/ |
| 메모라 | `memora.md` | https://coderstudiosdevelopers-coder.github.io/privacy/memora | https://coderstudiosdevelopers-coder.github.io/Memora/ |
| 펫포올 | `petforall.md` | https://coderstudiosdevelopers-coder.github.io/privacy/petforall | https://coderstudiosdevelopers-coder.github.io/PetForAll/ |
| CashMate | `cashmate.md` | https://coderstudiosdevelopers-coder.github.io/privacy/cashmate | https://coderstudiosdevelopers-coder.github.io/CashMate/ |
| 읽어주는 앱 | `textreading.md` | https://coderstudiosdevelopers-coder.github.io/privacy/textreading | https://coderstudiosdevelopers-coder.github.io/TextReading/ |
| 심플 QR | `simpleqr.md` | https://coderstudiosdevelopers-coder.github.io/privacy/simpleqr | https://coderstudiosdevelopers-coder.github.io/SimpleQR/ |

스토어(Play Console 등)의 링크를 새 링크로 바꾼 뒤에 옛 레포를 지우세요.

## 새 앱 추가하기

1. `_template.md`를 열어 내용을 전부 복사합니다.
2. **Add file → Create new file**에서 파일 이름을 `앱이름.md`(영문 소문자)로 정하고 붙여넣습니다.
3. 값을 채우고 **Commit changes**를 누르면 1~2분 뒤 `…/privacy/앱이름`으로 열립니다.

## 고치기

| 바꿀 것 | 위치 |
|---|---|
| 특정 앱 내용 | 그 앱의 `.md` 파일 (고치면 `updated_date`도 바꾸기) |
| 모든 앱 공통 문구·디자인 | `_layouts/privacy.html` |
| 개발자명·문의 이메일 | `_config.yml` |

## 앱 파일에 쓰는 항목

| 항목 | 필수 | 내용 |
|---|---|---|
| `app_name` | 필수 | 앱 이름 |
| `effective_date` | 필수 | 시행일 |
| `updated_date` | | 최종 수정일 |
| `app_desc` | | 소개 문장에 들어가는 앱 종류 (예: 사주·운세 앱) |
| `summary` | | 맨 위 핵심 요약 박스 |
| `items` | 필수 | 수집 항목 표. `type` 구분 · `data` 항목 · `why` 목적 · `how` 수집 방법 · `where` 저장 위치 중 쓴 칸만 표시 |
| `items_intro`, `items_note` | | 표 위·아래 문장 |
| `storage` | | 개인정보의 저장 위치 조항 |
| `purposes` | 필수 | 이용 목적 |
| `retention` | 필수 | 보유 및 파기 |
| `processors` | | 위탁 표 (`name`, `service`, `task`, `data`). 없으면 "위탁하지 않습니다"가 자동으로 표시 |
| `processors_intro`, `processors_note` | | 위탁 표 위·아래 문장 |
| `overseas` | | 국외 이전 안내 (쓰면 제목이 '위탁 및 국외 이전'으로 바뀜) |
| `third_party` | | 제3자 제공 (안 쓰면 공통 문구) |
| `sections` | | 앱만의 추가 조항 (`title`, `body`) |
| `permissions` | | 권한 표 (`name`, `need`, `why`). 권한이 없으면 `none` |
| `permissions_note` | | 권한 표 아래 문장 |
| `rights`, `children`, `safety` | | 이용자 권리 · 아동 · 안전성 조치 (안 쓰면 공통 문구) |
| `email` | | 이 앱만 문의 이메일을 다르게 할 때 |

문의처, 권익침해 구제 방법, 방침 변경 조항은 모든 앱에 자동으로 들어갑니다.
글 항목(`summary`, `purposes` 등)은 `|` 다음 줄부터 두 칸 들여 써서 마크다운으로 적습니다.
