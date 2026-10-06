# DP chips 교과서 · 투자 기초 개념 교과서

SOXL을 사례로 배우는 한국어 인터랙티브 투자 입문서. 제공된 전자책 이론의 흐름을 기본 개념 중심으로 재구성했습니다. SoCBook의 챕터 중심 학습 구성에서 영감을 받았으며 본문의 문장, 그림과 코드는 새로 작성했습니다.

## 구성

11개 학습 챕터, 19개 개념 실험, 54개 용어, 해설이 있는 10개 확인 문제. 모바일 화면, 밝은/어두운 테마, 브라우저에 저장하는 읽기 기록과 공부 메모를 지원합니다.

퀀트 사고방식 → 네 가지 투자 관점 → SOXL과 복리 → 데이터 → 주문과 지표(LOC/MOC · MA/EMA/FI · RSI) → 수익과 위험 읽기(위험 지표 · 기대값 · 비용 · 비중 · 증거) → 확률과 경로 → 레짐 → 심리와 운영.

특정 매매법의 주문 로직, 비공개 모드 추정, 매매 시뮬레이터, 파이썬 코드 블록은 제외했습니다. 모든 실험은 가상 수치와 명시된 가정을 사용하며 실제 성과나 미래 예측을 제공하지 않습니다.

## 실행

index.html을 브라우저에서 직접 열면 동작합니다. 외부 서버, API 키, 패키지 설치가 필요하지 않습니다. 폰트도 로컬 파일로 포함되어 있습니다.

## GitHub Pages

1. 저장소의 main 브랜치에 이 폴더의 내용을 업로드합니다. `.github/workflows/pages.yml`도 포함합니다.
2. Settings → Pages → Build and deployment → Source를 **GitHub Actions**로 선택합니다.
3. Actions → Deploy DP chips 교과서 to GitHub Pages → Run workflow로 배포합니다. 최초 push로 실행됐다면 완료 결과를 확인합니다.
4. deploy 작업의 github-pages 환경 URL을 엽니다.

상대 자산 경로와 hash 기반 챕터를 사용하므로 프로젝트 하위 경로에서도 동작합니다.

## 자료

- 전자책 이론: https://chatgpt.com/share/6ac4991c-613c-83ee-ba64-248b9069ad3f?ogimg=plain
- 구성 참고: https://socbook.euiyun.com/
- SOXL: https://www.direxion.com/product/daily-semiconductor-bull-bear-3x-etfs
- 레버리지 ETF: https://www.investor.gov/introduction-investing/general-resources/news-alerts/alerts-bulletins/investor-alerts/sec
- 종가 경매: https://www.nyse.com/trade/auctions
- FRED: https://fred.stlouisfed.org/
- EDGAR: https://www.sec.gov/edgar/search/

## 검증

`node verify.cjs`로 이동평균·Wilder RSI·LOC 가격 조건을 확인합니다. 전체 학습 화면의 입력 경계, 수치 유효성, 주문 판정, 경로 재배열, 용어 검색, 퀴즈, 메모, 모바일 너비와 메뉴·테마 동작을 브라우저에서 확인했습니다.


## 현재 학습 범위
기본 개념과 시각 실험을 중심으로 구성했습니다. 도구 설치·데이터 수집 실습·코드·과거 전략 성과 계산과 검증 절차는 제외합니다. 8계명 팝업은 한국 시간 기준 오늘 그만 보기를 지원하며 수동으로 다시 열 수 있습니다.


쉬운 설명과 직접 만지는 실험으로 개편했습니다. 규칙 만들기, 관점별 차트 재생, 일일 3배와 횡보, 거래일 달력, 손익 크기, 휩쏘와 심리 실험을 포함합니다. 확률 실험은 부록으로 이동했습니다. MOO조건은 HCM의 무조건 매도 별칭이며 실제 주문은 MOC입니다.
