<div align="center">
  <img width="200" alt="SEER Logo" src="https://github.com/user-attachments/assets/2b8664b0-884d-4e1b-9c62-8aae893bea96" />

  # SEER
  **Sepsis Early Emergency Response**
  
  <br>

  > **"Time is Life."**<br>
  > SEER는 응급실 환자의 골든타임을 지키기 위한<br>
  > **실시간 패혈증 조기 탐지 및 대응 솔루션**입니다.

  <br>

  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/SolidJS-2C4F7C?style=for-the-badge&logo=solid&logoColor=white">
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white">
</div>

<br>
<br>

## 1. Project Overview 

**SEER**는 응급실(ER) 환경에서 의료진이 놓칠 수 있는 환자의 미세한 바이탈 변화를 실시간으로 추적합니다.
패혈증(Sepsis) 위험 환자를 조기에 감지하고, **한눈에 파악 가능한 대시보드와 직관적인 알람**을 제공하여 신속한 대응을 돕습니다.

- **핵심 목표**: 데이터 기반의 조기 감지를 통한 환자 생존율 증대
- **타겟 질환**: 패혈증 (Sepsis) - *조기 발견 시 생존율 급상승*

<br>

## 2. Problem Definition

긴박한 응급실 현장에서는 다음과 같은 어려움이 존재합니다.

| Pain Points | 상세 내용 |
| :--- | :--- |
| **데이터 파편화** | 수기 차트 및 분산된 입력 시스템으로 환자 상태 통합 파악 난해 |
| **변화 감지 한계** | 시간 흐름에 따른 바이탈 트렌드(Trend)를 직관적으로 보기 힘듦 |
| **우선순위 혼선** | 다수의 환자 중 '누가 지금 가장 위험한지' 즉각적인 판단 어려움 |

<br>

## 3. Solution & Key Features 

SEER는 **qSOFA 기준**과 **시계열 바이탈 분석**을 결합하여 다음 솔루션을 제공합니다.

### 1. 실시간 모니터링 (Real-time Monitoring)
- 환자 방문(Visit) 단위의 실시간 데이터 수집
- **수집 지표**: `HR`(심박), `BP`(혈압), `RR`(호흡), `SpO₂`(산소포화도), `Temp`(체온)

### 2. AI 위험도 평가 (Risk Assessment)
- 단순 수치 모니터링을 넘어 복합적인 위험 징후 포착
- 위험 단계에 따른 **Color-coded Risk Level** 부여

### 3. 직관적 대시보드 (Dashboard & Alert)
- **Patient List**: 전체 환자의 위험도를 한눈에 시각화
- **Smart Alert**: 위급 상황 발생 시 의료진에게 즉각 알림
- **Explainable**: "왜 위험한지"에 대한 근거 데이터 제공

<br>

## 4. Tech Stack

최신 기술 트렌드를 반영하여 **고성능, 고가용성**을 목표로 설계되었습니다.

### **Backend**
<img src="https://img.shields.io/badge/Java 21-ED8B00?style=flat-square&logo=openjdk&logoColor=white"> <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/Spring Data JPA-gray?style=flat-square&logo=spring&logoColor=white">

* **Language**: Java 21 (LTS)
* **Framework**: Spring Boot (WebFlux/Reactive Stack 지원)
* **Database**:
    * **JPA**: 안정적인 데이터 영속성 관리
* **Build**: Gradle

### **Frontend**
<img src="https://img.shields.io/badge/SolidJS-2C4F7C?style=flat-square&logo=solid&logoColor=white"> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"> <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white"> <img src="https://img.shields.io/badge/Tailwind CSS v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white">

* **Core**: SolidJS (Fine-grained reactivity for high performance)
* **Routing & State**: TanStack Router, TanStack Query (Solid)
* **Styling**: Tailwind CSS v4, Sass
* **Validation**: Zod
