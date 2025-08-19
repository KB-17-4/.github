# 🏠전새내기
### KB IT's Your Life 6기 최종 프로젝트 (2025.07.09 ~ 2025.08.21)

<br>

## 📚목차
1️⃣ [프로젝트 소개](#1.-프로젝트-소개)
<br>
2️⃣ [팀원 소개](#2.-팀원-소개)
<br>
3️⃣ [개발 환경](#2.-개발-환경)
<br>
4️⃣ [프로젝트 배경](#3.-프로젝트-배경)
<br>
5️⃣ [설계 문서](#4.-설계-문서)
<br>
6️⃣ [서비스 화면](#5.-서비스-화면)
<br>
7️⃣ [핵심 기능](#6.-핵심-기능)
<br>
8️⃣
<br>
9️⃣
<br>
🔟

## 1. 프로젝트 소개
### 부동산 안심 계약 플랫폼 "전 새내기"
**전** 문가처럼 등기부등본을 분석하고,
<br>
**새** 로운 기준으로 계약서를 꼼꼼히 비교해요.
<br>
**내** 불안했던 부동산 거래는 이제 안심!
<br>
**기** 존의 걱정을 싹 지워주는 앱, 바로 우리 프로젝트랍니다!

## 2. 팀원 소개
**Programming Language**
<br>
<br>
 ![JAVA](https://img.shields.io/badge/Java-007396?style=flat-square&logo=data:image/svg%2bxml;base64,PCFET0NUWVBFIHN2ZyBQVUJMSUMgIi0vL1czQy8vRFREIFNWRyAxLjEvL0VOIiAiaHR0cDovL3d3dy53My5vcmcvR3JhcGhpY3MvU1ZHLzEuMS9EVEQvc3ZnMTEuZHRkIj4KDTwhLS0gVXBsb2FkZWQgdG86IFNWRyBSZXBvLCB3d3cuc3ZncmVwby5jb20sIFRyYW5zZm9ybWVkIGJ5OiBTVkcgUmVwbyBNaXhlciBUb29scyAtLT4KPHN2ZyB3aWR0aD0iMTUwcHgiIGhlaWdodD0iMTUwcHgiIHZpZXdCb3g9IjAgMCAzMi4wMCAzMi4wMCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiBmaWxsPSIjZmZmZmZmIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS13aWR0aD0iMC4yNTYiPgoNPGcgaWQ9IlNWR1JlcG9fYmdDYXJyaWVyIiBzdHJva2Utd2lkdGg9IjAiLz4KDTxnIGlkPSJTVkdSZXBvX3RyYWNlckNhcnJpZXIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIvPgoNPGcgaWQ9IlNWR1JlcG9faWNvbkNhcnJpZXIiPiA8cGF0aCBmaWxsPSIjZmZmZmZmIiBkPSJNMTIuNTU3IDIzLjIyYzAgMC0wLjk4MiAwLjU3MSAwLjY5OSAwLjc2NSAyLjAzNyAwLjIzMiAzLjA3OSAwLjE5OSA1LjMyNC0wLjIyNiAwIDAgMC41OSAwLjM3IDEuNDE1IDAuNjkxLTUuMDMzIDIuMTU3LTExLjM5LTAuMTI1LTcuNDM3LTEuMjN6TTExLjk0MiAyMC40MDVjMCAwLTEuMTAyIDAuODE2IDAuNTgxIDAuOTkgMi4xNzYgMC4yMjQgMy44OTUgMC4yNDMgNi44NjktMC4zMyAwIDAgMC40MTEgMC40MTcgMS4wNTggMC42NDUtNi4wODUgMS43NzktMTIuODYzIDAuMTQtOC41MDgtMS4zMDV6TTE3LjEyNyAxNS42M2MxLjI0IDEuNDI4LTAuMzI2IDIuNzEzLTAuMzI2IDIuNzEzczMuMTQ5LTEuNjI1IDEuNzAzLTMuNjYxYy0xLjM1MS0xLjg5OC0yLjM4Ni0yLjg0MSAzLjIyMS02LjA5MyAwIDAtOC44MDEgMi4xOTgtNC41OTggNy4wNDJ6TTIzLjc4MyAyNS4zMDJjMCAwIDAuNzI3IDAuNTk5LTAuODAxIDEuMDYyLTIuOTA1IDAuODgtMTIuMDkxIDEuMTQ2LTE0LjY0MyAwLjAzNS0wLjkxNy0wLjM5OSAwLjgwMy0wLjk1MyAxLjM0NC0xLjA2OSAwLjU2NC0wLjEyMiAwLjg4Ny0wLjEgMC44ODctMC4xLTEuMDIwLTAuNzE5LTYuNTk0IDEuNDExLTIuODMxIDIuMDIxIDEwLjI2MiAxLjY2NCAxOC43MDYtMC43NDkgMTYuMDQ0LTEuOTV6TTEzLjAyOSAxNy40ODljMCAwLTQuNjczIDEuMTEtMS42NTUgMS41MTMgMS4yNzQgMC4xNzEgMy44MTQgMC4xMzIgNi4xODEtMC4wNjYgMS45MzQtMC4xNjMgMy44NzYtMC41MSAzLjg3Ni0wLjUxcy0wLjY4MiAwLjI5Mi0xLjE3NSAwLjYyOWMtNC43NDUgMS4yNDgtMTMuOTExIDAuNjY3LTExLjI3Mi0wLjYwOSAyLjIzMi0xLjA3OSA0LjA0Ni0wLjk1NiA0LjA0Ni0wLjk1NnpNMjEuNDEyIDIyLjE3NGM0LjgyNC0yLjUwNiAyLjU5My00LjkxNSAxLjAzNy00LjU5MS0wLjM4MiAwLjA3OS0wLjU1MiAwLjE0OC0wLjU1MiAwLjE0OHMwLjE0Mi0wLjIyMiAwLjQxMi0wLjMxOGMzLjA3OS0xLjA4MyA1LjQ0OCAzLjE5My0wLjk5NCA0Ljg4Ny0wIDAgMC4wNzUtMC4wNjcgMC4wOTctMC4xMjZ6TTE4LjUwMyAzLjMzN2MwIDAgMi42NzEgMi42NzItMi41MzQgNi43ODEtNC4xNzQgMy4yOTYtMC45NTIgNS4xNzYtMC4wMDIgNy4zMjMtMi40MzYtMi4xOTgtNC4yMjQtNC4xMzMtMy4wMjUtNS45MzQgMS43NjEtMi42NDQgNi42MzgtMy45MjUgNS41Ni04LjE3ek0xMy41MDMgMjguOTY2YzQuNjMgMC4yOTYgMTEuNzQtMC4xNjQgMTEuOTA4LTIuMzU1IDAgMC0wLjMyNCAwLjgzMS0zLjgyNiAxLjQ5LTMuOTUyIDAuNzQ0LTguODI2IDAuNjU3LTExLjcxNiAwLjE4IDAgMCAwLjU5MiAwLjQ5IDMuNjM1IDAuNjg1eiIvPiA8L2c+Cg08L3N2Zz4=)
<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat-square&logo=javascript&logoColor=ffffff" />

<br>
<br>

**BackEnd**

![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)

<br>
<br>

**FrontEnd**

<p>
  <img src="https://img.shields.io/badge/Vue-1e1f26.svg?style=flat-square&logo=vuedotjs&logoColor=4FC08D" />
  <img src="https://img.shields.io/badge/Tailwind-06B6D4.svg?style=flat-square&logo=tailwindcss&logoColor=ffffff" />
</p>


## 3. 개발 환경
## 4. 프로젝트 배경
## 5. 설계 문서
### ERD https://www.erdcloud.com/d/u5xYQ42r9nD35bmRS
<img width="4810" height="3502" alt="image" src="https://github.com/user-attachments/assets/165d61ec-89c0-4ca6-b223-362596de0cfa" />

### 시스템 아키텍처

### API 명세
## 6. 서비스 화면
## 7. 핵심 기능

납부 이력 기반 뱃지 표시

KB국민은행 인증 납부 이력 뱃지 제공

예: ✔️ 23개월 납부 인증


실거주자 리뷰 시스템

퇴거 시점까지 보관 후 공개되는 실거주 후기

관리자 검수, 스팸 필터, 신고 기능 도입

리뷰 작성자 거주 기간/뱃지 표시로 신뢰성 강화


리뷰 누적 보상 시스템
리뷰 작성 횟수에 따라 쿠폰·혜택 지급
누적 작성 시 점진적 보상 구조 적용

사기 예방 및 계약서 검증
지연이체 기능: 거래 전 안전 점검 시간 확보
OCR+AI 계약서 분석: 계약서 ↔ 등기부등본 대조 자동 검증
등기부 변동 알림 서비스(KB 연계)로 위험 알림

체크리스트 기능
계약 전 확인해야 할 항목 체크리스트 제공

퇴거자 채팅 시스템
입주 예정자 ↔ 퇴거자 간 실시간 상담
집 상태, 관리비, 집주인 성향 등 실거주 정보 제공
