# HealthDCAT-KR Dataset Description Assistant

보건의료 데이터셋을 HealthDCAT-KR 명세에 맞는 RDF 메타데이터로 작성하는 도구입니다.
설치나 계정 없이 브라우저에서 동작하며, 입력한 내용은 서버로 전송되지 않습니다.

## 바로 쓰기

- 사용 안내 — <https://kdyoung100.github.io/HealthDCAT-KR-Dataset-Description-Assistant/guide.html>
- 생성 도구 — <https://kdyoung100.github.io/HealthDCAT-KR-Dataset-Description-Assistant/tool.html>

프로파일 명세는 [HealthDCAT-KR](https://kdyoung100.github.io/HealthDCAT-KR/) 문서를 따릅니다.

## 무엇을 만드나

데이터세트(`dcat:Dataset`)와 배포 형식(`dcat:Distribution`)을 파일 두 개로 나눠 내보냅니다.

```
HealthDCAT-KR_데이터셋이름_데이터셋.rdf
HealthDCAT-KR_데이터셋이름_배포.rdf
```

JSON-LD(`.jsonld`) · Turtle(`.ttl`) · RDF/XML(`.rdf`) 중에서 고를 수 있습니다.

## 두 가지 작성 방식

| | 직접 입력 | 엑셀로 일괄 등록 |
|---|---|---|
| 알맞은 때 | 데이터셋 1건 | 여러 건 한 번에 |
| 방법 | 항목별 입력 칸에 작성 | 양식(.xlsx)을 받아 채운 뒤 올리기 |
| 결과 | 파일 2개 | 데이터셋 이름별로 각각 2개씩 |

데이터셋 양식의 `식별자`와 배포 양식의 `데이터셋식별자`가 같으면 두 줄이 이어집니다.

## 항목 구성

- 데이터세트 29개 — 필수 9 / 권장 20
- 배포 형식 5개 — 필수 1(접근 URL) / 권장 4

필수·권장 구분은 HealthDCAT-AP의 제한(Restricted) 권한 기준을 준용합니다.

## 파일

| 파일 | 설명 |
|---|---|
| `guide.html` | 사용 안내 페이지 |
| `tool.html` | 메타데이터 생성 도구 (단일 HTML, 의존성은 SheetJS CDN 하나) |

## 배포

GitHub Pages — Settings → Pages → Source: `main` / `(root)`
