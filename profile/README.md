# 🏠전 새내기
### KB IT's Your Life 6기 최종 프로젝트 (2025.07.09 ~ 2025.08.21)

<br>

## 📚목차
1️⃣ [프로젝트 소개](#1-프로젝트-소개)
<br>
2️⃣ [팀원 소개](#2-팀원-소개)
<br>
3️⃣ [개발 환경](#3-개발-환경)
<br>
4️⃣ [프로젝트 배경](#4-프로젝트-배경)
<br>
5️⃣ [설계 문서](#5-설계-문서)
<br>
6️⃣ [서비스 화면](#6-서비스-화면)
<br>
7️⃣ [핵심 기능](#7-핵심-기능)
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
|박해세 (팀장)|안병우|김은민|김하나|
|:-:|:-:|:-:|:-:|
|<img width="235" height="208" alt="image" src="https://github.com/user-attachments/assets/23f1403f-7afd-411c-89e1-703b7fe14b80" />|<img width="212" height="173" alt="image" src="https://github.com/user-attachments/assets/799b7472-b17f-40f4-9a1c-1b7e745b62ec" />|<img width="189" height="175" alt="image" src="https://github.com/user-attachments/assets/4bd2a948-bf63-413a-9dbb-cd7145aeefd6" />|<img width="214" height="183" alt="image" src="https://github.com/user-attachments/assets/7958ebd5-9756-435e-81bb-54535b2f0173" />|
|기획, 영상 편집 및 발표<br>계약서 Open API 연동<br>리뷰 작성 기능 개발|사용자 계정 관련 기능<br>요구사항 명세서<br>유스케이스 다이어그램|전세 계약 유형 테스트<br>매물 리뷰 기능<br>포트폴리오 제작|이체 및 지연이체 기능<br>채팅방 기능<br>Class Diagram 작성|

<br>

|문시윤|우현서|이동진|이세연|
|:-:|:-:|:-:|:-:|
|<img width="235" height="234" alt="image" src="https://github.com/user-attachments/assets/1360af2b-8684-4fd8-bc40-aca74dc0f227" />|<img width="212" height="225" alt="image" src="https://github.com/user-attachments/assets/f3063a1d-c147-466f-9cb4-2014fb6e0def" />|<img width="189" height="185" alt="image" src="https://github.com/user-attachments/assets/f18a753d-2774-4cbb-b1e0-faa9e46e9c31" />|<img width="214" height="208" alt="image" src="https://github.com/user-attachments/assets/605916d7-9ff6-4a1f-890d-14b0d0467138" />|
|채팅방 기능<br>회원가입 후 모달창 기능<br>포트폴리오, UI/UX 설명서 제작|지도 내 리뷰 및 매물 조회 기능<br>서비스 배포<br>간트 차트 작성|매물 상세 페이지<br>매물 추천 페이지<br>추천 로직/대출 페이지 연결|등기부등본 Codef API 연동<br>등기부등본 결과/계약서 대조<br>기술명세서, API 명세서 등|

## 3. 개발 환경
**Programming Language**

 ![JAVA](https://img.shields.io/badge/Java-007396?style=flat-square&logo=data:image/svg%2bxml;base64,PCFET0NUWVBFIHN2ZyBQVUJMSUMgIi0vL1czQy8vRFREIFNWRyAxLjEvL0VOIiAiaHR0cDovL3d3dy53My5vcmcvR3JhcGhpY3MvU1ZHLzEuMS9EVEQvc3ZnMTEuZHRkIj4KDTwhLS0gVXBsb2FkZWQgdG86IFNWRyBSZXBvLCB3d3cuc3ZncmVwby5jb20sIFRyYW5zZm9ybWVkIGJ5OiBTVkcgUmVwbyBNaXhlciBUb29scyAtLT4KPHN2ZyB3aWR0aD0iMTUwcHgiIGhlaWdodD0iMTUwcHgiIHZpZXdCb3g9IjAgMCAzMi4wMCAzMi4wMCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIiBmaWxsPSIjZmZmZmZmIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS13aWR0aD0iMC4yNTYiPgoNPGcgaWQ9IlNWR1JlcG9fYmdDYXJyaWVyIiBzdHJva2Utd2lkdGg9IjAiLz4KDTxnIGlkPSJTVkdSZXBvX3RyYWNlckNhcnJpZXIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIvPgoNPGcgaWQ9IlNWR1JlcG9faWNvbkNhcnJpZXIiPiA8cGF0aCBmaWxsPSIjZmZmZmZmIiBkPSJNMTIuNTU3IDIzLjIyYzAgMC0wLjk4MiAwLjU3MSAwLjY5OSAwLjc2NSAyLjAzNyAwLjIzMiAzLjA3OSAwLjE5OSA1LjMyNC0wLjIyNiAwIDAgMC41OSAwLjM3IDEuNDE1IDAuNjkxLTUuMDMzIDIuMTU3LTExLjM5LTAuMTI1LTcuNDM3LTEuMjN6TTExLjk0MiAyMC40MDVjMCAwLTEuMTAyIDAuODE2IDAuNTgxIDAuOTkgMi4xNzYgMC4yMjQgMy44OTUgMC4yNDMgNi44NjktMC4zMyAwIDAgMC40MTEgMC40MTcgMS4wNTggMC42NDUtNi4wODUgMS43NzktMTIuODYzIDAuMTQtOC41MDgtMS4zMDV6TTE3LjEyNyAxNS42M2MxLjI0IDEuNDI4LTAuMzI2IDIuNzEzLTAuMzI2IDIuNzEzczMuMTQ5LTEuNjI1IDEuNzAzLTMuNjYxYy0xLjM1MS0xLjg5OC0yLjM4Ni0yLjg0MSAzLjIyMS02LjA5MyAwIDAtOC44MDEgMi4xOTgtNC41OTggNy4wNDJ6TTIzLjc4MyAyNS4zMDJjMCAwIDAuNzI3IDAuNTk5LTAuODAxIDEuMDYyLTIuOTA1IDAuODgtMTIuMDkxIDEuMTQ2LTE0LjY0MyAwLjAzNS0wLjkxNy0wLjM5OSAwLjgwMy0wLjk1MyAxLjM0NC0xLjA2OSAwLjU2NC0wLjEyMiAwLjg4Ny0wLjEgMC44ODctMC4xLTEuMDIwLTAuNzE5LTYuNTk0IDEuNDExLTIuODMxIDIuMDIxIDEwLjI2MiAxLjY2NCAxOC43MDYtMC43NDkgMTYuMDQ0LTEuOTV6TTEzLjAyOSAxNy40ODljMCAwLTQuNjczIDEuMTEtMS42NTUgMS41MTMgMS4yNzQgMC4xNzEgMy44MTQgMC4xMzIgNi4xODEtMC4wNjYgMS45MzQtMC4xNjMgMy44NzYtMC41MSAzLjg3Ni0wLjUxcy0wLjY4MiAwLjI5Mi0xLjE3NSAwLjYyOWMtNC43NDUgMS4yNDgtMTMuOTExIDAuNjY3LTExLjI3Mi0wLjYwOSAyLjIzMi0xLjA3OSA0LjA0Ni0wLjk1NiA0LjA0Ni0wLjk1NnpNMjEuNDEyIDIyLjE3NGM0LjgyNC0yLjUwNiAyLjU5My00LjkxNSAxLjAzNy00LjU5MS0wLjM4MiAwLjA3OS0wLjU1MiAwLjE0OC0wLjU1MiAwLjE0OHMwLjE0Mi0wLjIyMiAwLjQxMi0wLjMxOGMzLjA3OS0xLjA4MyA1LjQ0OCAzLjE5My0wLjk5NCA0Ljg4Ny0wIDAgMC4wNzUtMC4wNjcgMC4wOTctMC4xMjZ6TTE4LjUwMyAzLjMzN2MwIDAgMi42NzEgMi42NzItMi41MzQgNi43ODEtNC4xNzQgMy4yOTYtMC45NTIgNS4xNzYtMC4wMDIgNy4zMjMtMi40MzYtMi4xOTgtNC4yMjQtNC4xMzMtMy4wMjUtNS45MzQgMS43NjEtMi42NDQgNi42MzgtMy45MjUgNS41Ni04LjE3ek0xMy41MDMgMjguOTY2YzQuNjMgMC4yOTYgMTEuNzQtMC4xNjQgMTEuOTA4LTIuMzU1IDAgMC0wLjMyNCAwLjgzMS0zLjgyNiAxLjQ5LTMuOTUyIDAuNzQ0LTguODI2IDAuNjU3LTExLjcxNiAwLjE4IDAgMCAwLjU5MiAwLjQ5IDMuNjM1IDAuNjg1eiIvPiA8L2c+Cg08L3N2Zz4=)
<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat-square&logo=javascript&logoColor=ffffff" />
<br>

**FrontEnd**

<p>
 <img src="https://img.shields.io/badge/Vue-1e1f26.svg?style=flat-square&logo=vuedotjs&logoColor=4FC08D" />
 <img src="https://img.shields.io/badge/Tailwind-06B6D4.svg?style=flat-square&logo=tailwindcss&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/Axios-5A29E4.svg?style=flat-square&logo=axios&logoColor=ffffff" />
</p>

**BackEnd**

<p>
 <img src="https://img.shields.io/badge/Spring-6DB33F.svg?style=flat-square&logo=spring&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/Kakako Map API-FFCD00.svg?style=flat-square&logo=googlemaps&logoColor=4285F4" />
 <img src="https://img.shields.io/badge/CODEF API-24CBD0.svg?style=flat-square&logo=rhinoceros&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/OpenAI API-412991.svg?style=flat-square&logo=openai&logoColor=ffffff" />
</p>

**DataBase**

<p>
 <img src="https://img.shields.io/badge/MySQL-4479A1.svg?style=flat-square&logo=mysql&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/AWS S3-B73939.svg?style=flat-square&logo=icloud&logoColor=ffffff" />
</p>

**Authentication**

<p>
 <img src="https://img.shields.io/badge/Spring Security-6DB33F.svg?style=flat-square&logo=springsecurity&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/JSON Web Tokens-000000.svg?style=flat-square&logo=jsonwebtokens&logoColor=ffffff" />
</p>

**Infra**

<p>
 <img src="https://img.shields.io/badge/AWS EC2-F38020.svg?style=flat-square&logo=icloud&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/Docker-2496ED.svg?style=flat-square&logo=docker&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/Ubuntu-E95420.svg?style=flat-square&logo=ubuntu&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/Nginx-009639.svg?style=flat-square&logo=nginx&logoColor=ffffff" />
 <img src="https://img.shields.io/badge/Apache Tomcat-F8DC75.svg?style=flat-square&logo=apachetomcat&logoColor=ffffff" />
</p>

<br>

## 4. 프로젝트 배경

## 5. 설계 문서
### ▶️[ERD 보러가기](https://www.erdcloud.com/d/Ce29KPQL8rBtiy4qd)
<img width="4810" height="3502" alt="image" src="https://github.com/user-attachments/assets/165d61ec-89c0-4ca6-b223-362596de0cfa" />

### 시스템 아키텍처

### API 명세
<img width="1598" height="655" alt="image" src="https://github.com/user-attachments/assets/be8f5ca6-5e39-407a-8f22-d2f38af06973" />
<img width="1599" height="621" alt="image" src="https://github.com/user-attachments/assets/955aacca-41bf-4d16-8f80-315b22aaeed9" />
<img width="1598" height="571" alt="image" src="https://github.com/user-attachments/assets/b6c0bb2a-f433-4468-a79f-e288197d399e" />
<img width="1601" height="586" alt="image" src="https://github.com/user-attachments/assets/2f94f4f9-b2a5-4722-804f-f578f7e4308f" />
<img width="1598" height="425" alt="image" src="https://github.com/user-attachments/assets/008e2a7d-8292-4a27-b8e3-48a27db2ddd0" />
<img width="1600" height="373" alt="image" src="https://github.com/user-attachments/assets/31683af6-3d33-4e15-aaae-b8f1805daaa9" />
<img width="1598" height="598" alt="image" src="https://github.com/user-attachments/assets/4c57ec81-6fc1-4089-8dc4-b740b9b235a5" />
<img width="1598" height="643" alt="image" src="https://github.com/user-attachments/assets/20a4cbf6-c429-4f23-9bf0-0dd91307e187" />
<img width="1600" height="523" alt="image" src="https://github.com/user-attachments/assets/e382ed9a-7e0b-483b-9905-265f2ceda4df" />
<img width="1598" height="660" alt="image" src="https://github.com/user-attachments/assets/fd3942f9-0ed2-4aa1-b822-63a0b334b45b" />






## 6. 서비스 화면
## 7. 핵심 기능

### 1. 🏠 안전하고 투명한 계약 검증 시스템

- **지연이체 기능 도입**: 부동산 계약 거래 전 충분한 안전 점검 시간을 확보하여, 사용자가 거래 내용을 재확인하고 위험 요소를 분석할 수 있도록 돕습니다.
- **OCR + AI 계약서 분석 (계약서 ↔ 등기부등본 대조)**: AI 기반의 OCR 기술을 활용하여 사용자가 업로드한 계약서와 등기부등본의 내용을 자동으로 추출하고 대조합니다. 이를 통해 오기재, 불일치 등 잠재적 위험 요소를 사전에 정확히 파악하여 사기 피해를 예방합니다.
- **등기부 변동 알림 서비스 (KB국민은행 연계)**: 등기부등본 내용에 변동이 생길 경우 사용자에게 실시간으로 알림을 제공하여 계약 중 또는 잔금 전 위험 발생 시 즉각적으로 대응할 수 있도록 돕습니다.

### 2. ⭐ 신뢰도 높은 실거주자 리뷰 시스템

- **퇴거 시점 공개**: 퇴거가 완료된 시점에 리뷰를 공개하도록 하여, 실제 거주 경험에 기반한 생생하고 솔직한 후기를 제공합니다.
- **강력한 신뢰성 확보**: 관리자 검수, 스팸 필터링, 신고 기능 도입을 통해 리뷰의 신뢰도를 극대화합니다.
- **리뷰 작성자 신뢰도 강화**: 리뷰 작성자의 거주 기간 표시 및 KB국민은행 인증 납부 이력 기반 뱃지 제공(✔️ 23개월 납부 인증 예시)으로 정보의 신뢰성을 더욱 높입니다.
- **리뷰 누적 보상 시스템**: 리뷰 작성 횟수에 따라 쿠폰, 혜택 등 점진적인 보상을 제공하여 양질의 리뷰 작성 참여를 유도합니다.

### 3. ✅ 스마트 계약 준비 지원

- **체크리스트 기능**: 계약 전 필수적으로 확인해야 할 항목들을 체계적인 체크리스트로 제공하여 사용자가 놓치기 쉬운 부분을 꼼꼼히 점검할 수 있도록 돕습니다.
- **퇴거자 채팅 시스템**: 입주 예정자가 해당 주택의 퇴거자와 1:1 실시간 상담을 진행할 수 있도록 연결합니다. 이를 통해 집 상태, 관리비, 집주인 성향 등 서류만으로는 알 수 없는 생생한 실거주 정보를 얻고 궁금증을 해소할 수 있습니다.


