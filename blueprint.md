# Blueprint: AI 체형 진단 (My Body Shape)

## 1. 개요 (Overview)
이 프로젝트는 사용자의 전신 사진을 AI(Teachable Machine)로 분석하여 '골격 진단 이론'에 기반한 체형 타입(스트레이트, 웨이브, 내추럴)을 알려주는 웹 애플리케이션입니다. 단순한 진단을 넘어, 각 체형에 맞는 패션 스타일링 팁을 제공합니다.

## 2. 기술 스택 (Tech Stack)
*   **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
*   **AI/ML:**
    *   Google Teachable Machine Image Model (체형 분류)
    *   TensorFlow.js `coco-ssd` (사람 감지 및 필터링)
*   **Utilities:** html2canvas (결과 이미지 저장)
*   **Deployment:** Firebase Hosting (예정/설정됨)

## 3. 주요 기능 (Features)
*   **AI 이미지 분석:**
    *   **1단계:** `coco-ssd` 모델로 사진 속에 사람이 있는지 확인 (동물/사물 필터링).
    *   **2단계:** 사람이 감지되면 Teachable Machine 모델로 3가지 골격 타입 확률 계산.
*   **추가 설문조사:** AI 분석의 정확도를 보완하기 위한 자가 진단 설문 기능.
*   **상세 결과 리포트:**
    *   체형별 긍정적인 멘트와 장점 강조 (7줄 이상).
    *   단점 보완을 위한 구체적인 스타일링 가이드.
    *   동일 체형의 연예인 예시 및 추천 아이템 제공.
*   **다국어 지원:** 한국어(KO) 및 영어(EN) 지원.
*   **AdSense 최적화:** 게시자 콘텐츠 확보를 위한 설명 텍스트 및 필수 페이지(개인정보처리방침 등) 구비.
*   **관련 콘텐츠 링크:** 메인 화면 하단에 외부 블로그 링크를 통한 추가 콘텐츠 제공.

## 4. 페이지 구조 (Page Structure)
*   **index.html:** 메인 앱 (SPA 구조).
    *   `#view-upload`: 메인 랜딩 및 업로드 화면 (설명 텍스트, 관련 콘텐츠 링크 포함).
    *   `#view-loading`: 분석 로딩 화면.
    *   `#view-survey`: 설문조사 화면.
    *   `#view-result`: 최종 결과 화면 (이미지, 상세 텍스트).
*   **privacy.html:** 개인정보처리방침 (AdSense 필수).
*   **about.html:** 서비스 소개.
*   **contact.html:** 문의하기.
*   **robots.txt:** 검색 엔진 크롤러 제어.
*   **sitemap.xml:** 사이트맵 제공.

## 5. SEO 최적화 (SEO Optimization) - 2026.01.27
*   **`robots.txt` 생성:** 모든 검색 엔진의 크롤링을 허용하도록 설정.
*   **`sitemap.xml` 생성:** 사이트의 모든 페이지(`index.html`, `about.html`, `contact.html`, `privacy.html`)를 포함하는 사이트맵 제공.
*   **메타 태그 추가:**
    *   모든 HTML 페이지에 `description`, `keywords`, `author` 메타 태그 추가.
    *   `og:title`, `og:description`, `og:image`, `og:url` 등 Open Graph 태그 추가하여 소셜 공유 최적화.
*   **이미지 `alt` 속성 추가:** `index.html` 내 모든 `<img>` 태그에 의미있는 `alt` 텍스트 추가.
*   **시맨틱 HTML 개선:** 논리적인 헤더 태그 사용 및 구조 검토.

## 6. 최근 변경 사항 (Recent Changes) - 2026.01.26
*   **사람 감지 기능 도입:** `coco-ssd` 모델을 추가하여 사람 사진이 아닐 경우 분석을 거부하는 로직 구현.
*   **결과 콘텐츠 대폭 보강:** 결과 화면의 텍스트를 단순 요약에서 칭찬, 보완 가이드, 연예인 예시가 포함된 풍부한 콘텐츠로 업데이트.
*   **이미지 경로 수정:** 결과 화면에서 이미지가 나오지 않던 버그 수정 및 예외 처리(`onerror`) 추가.
*   **콘텐츠 보강:** 메인 화면 하단에 체형 진단 원리 및 중요성에 대한 설명 텍스트 추가.
*   **필수 페이지 구축:** `privacy.html`, `about.html`, `contact.html` 생성.
