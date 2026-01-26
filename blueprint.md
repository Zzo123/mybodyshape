# Blueprint: AI 체형 진단 (My Body Shape)

## 1. 개요 (Overview)
이 프로젝트는 사용자의 전신 사진을 AI(Teachable Machine)로 분석하여 '골격 진단 이론'에 기반한 체형 타입(스트레이트, 웨이브, 내추럴)을 알려주는 웹 애플리케이션입니다. 단순한 진단을 넘어, 각 체형에 맞는 패션 스타일링 팁을 제공합니다.

## 2. 기술 스택 (Tech Stack)
*   **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
*   **AI/ML:** Google Teachable Machine Image Model, TensorFlow.js
*   **Utilities:** html2canvas (결과 이미지 저장)
*   **Deployment:** Firebase Hosting (예정/설정됨)

## 3. 주요 기능 (Features)
*   **AI 이미지 분석:** 사용자가 업로드한 사진을 실시간으로 분석하여 3가지 골격 타입 확률 계산.
*   **추가 설문조사:** AI 분석의 정확도를 보완하기 위한 자가 진단 설문 기능.
*   **결과 리포트:** 체형별 특징, 추천 스타일, 연예인 예시 등을 포함한 상세 리포트 제공.
*   **다국어 지원:** 한국어(KO) 및 영어(EN) 지원.
*   **AdSense 최적화:** 게시자 콘텐츠 확보를 위한 설명 텍스트 및 필수 페이지(개인정보처리방침 등) 구비.
*   **관련 콘텐츠 링크:** 메인 화면 하단에 외부 블로그 링크를 통한 추가 콘텐츠 제공.

## 4. 페이지 구조 (Page Structure)
*   **index.html:** 메인 앱 (SPA 구조).
    *   `#view-upload`: 메인 랜딩 및 업로드 화면 (설명 텍스트, 관련 콘텐츠 링크 포함).
    *   `#view-loading`: 분석 로딩 화면.
    *   `#view-survey`: 설문조사 화면.
    *   `#view-result`: 최종 결과 화면.
*   **privacy.html:** 개인정보처리방침 (AdSense 필수).
*   **about.html:** 서비스 소개.
*   **contact.html:** 문의하기.

## 5. 최근 변경 사항 (Recent Changes) - 2026.01.26
*   **콘텐츠 보강:** 메인 화면 하단에 체형 진단 원리 및 중요성에 대한 설명 텍스트(500자 이상) 추가. (AdSense '게시자 콘텐츠' 요건 충족)
*   **필수 페이지 구축:** `privacy.html`, `about.html`, `contact.html` 생성 및 푸터 링크 연결.
*   **관련 콘텐츠 링크 추가:** 메인 화면 하단에 "볼만한 글들" 섹션과 함께 외부 블로그 링크 2개 배치.
