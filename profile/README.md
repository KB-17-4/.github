# [🏠전 새내기](https://new-bie.o-r.kr/)
### KB IT's Your Life 6기 최종 프로젝트 (2025.07.09 ~ 2025.08.21)

▶️[서비스 바로가기 Click!](https://new-bie.o-r.kr/)

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


## 1. 프로젝트 소개
### 부동산 안심 계약 플랫폼 "전 새내기"  
![Image](https://github.com/user-attachments/assets/49239ffc-a7ca-43bd-893a-387b22757131)  
**전** 문가처럼 등기부등본을 분석하고,
<br>
**새** 로운 기준으로 계약서를 꼼꼼히 비교해요.
<br>
**내** 불안했던 부동산 거래는 이제 안심!
<br>
**기** 존의 걱정을 싹 지워주는 앱, 바로 우리 프로젝트랍니다!

## 2. 팀원 소개  

<img width="970" height="600" alt="Image" src="https://github.com/user-attachments/assets/8c9bc3bc-b6ad-4c25-bc39-455761632fba" />  

| 팀원 | 역할 / 기술 스택 |
|:-:|:-|
| 박해세 (팀장) | 기획 및 프로젝트 총괄, 계약서 Open API 연동, 리뷰 작성 기능 개발 |
| 안병우 | Spring Security 기반 사용자 계정 관리, 서비스 배포 |
| 김은민 | 전세 계약 유형 테스트, 매물 리뷰 기능 구현 |
| 김하나 | 이체 및 지연이체 기능 개발, WebSocket 채팅 시스템, 서비스 배포 |
| 문시윤 | 채팅방 기능 개발, 회원가입 모달 기능 구현 |
| 우현서 | 지도 기반 리뷰/매물 조회, Kakao Map API 활용, 서비스 배포 |
| 이동진 | 매물 상세/추천 페이지 구현, 추천 로직 및 대출 페이지 연동 |
| 이세연 | 등기부등본 Codef API 연동, 등기부등본 결과와 계약서 대조 |



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

**Architecture**

<p>
 <img width="970" height="600" alt="아키텍처" src="https://github.com/user-attachments/assets/db7b4c36-93f1-43a1-aafb-66976638db01" />
</p>

<br>

## 4. 프로젝트 배경

### 4-1. 문제 인식
사회 초년생들은 부동산 거래 경험이 부족하고, 계약 관련 정보가 제한적입니다.  
그로 인해 **전세 사기, 이중 계약, 깡통 전세** 등 위험에 노출될 가능성이 높습니다.

<table> 
<tr>
<td>

<img src="https://github.com/user-attachments/assets/32a27201-e31d-4c22-b7d6-f71b0af2d858" width="300">

</td>
<td>

### 프로젝트 목적
- 👨‍💼 **사회 초년생 안전 거래 문화 조성** → 전세 사기, 이중 계약 등 위험 예방  
- 📄 **계약서 납부 이력 기반 뱃지/태그 제공** → 매물 신뢰도 향상, 정보 부족 문제 해결  
- 🏘 **실거주자 리뷰 시스템** → 실제 거주 경험 공유로 매물 정보 강화  
- ⏱ **지연이체 및 체크리스트 기능** → 사전 위험 예방  
- 💬 **퇴거자·입주자 간 채팅 시스템** → 신뢰 기반 정보 제공, 문제 해결 지원

</td>
</tr>
</table>




## 5. 설계 문서
### ▶️[ERD 보러가기](https://www.erdcloud.com/d/Ce29KPQL8rBtiy4qd)  
* 아래 이미지는 주요 기능을 정리한 것으로 실제 구성과 차이가 있습니다 
<img width="975" height="2343" alt="Image" src="https://github.com/user-attachments/assets/0b4aa7f3-2ab3-450b-b97f-af45101c360a" />
<br>
<br>

### ▶️[API 명세서 보러가기](https://ultra-playground-0a9.notion.site/API-2542350d416c80208c98c09c1b1033fc?source=copy_link)
<img width="1028" height="1583" alt="image" src="https://github.com/user-attachments/assets/f8a6d65c-096c-4566-8deb-7d38cb99b612" />

<br>
<br>

## 6. 서비스 화면
|회원가입|로그인|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/83c9682b-4381-45a6-a274-d90ec5b2c5b3" />|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/210e1616-1781-4dfc-8d02-66f6dc3d910e" />|

<br>

|마이페이지(임차인)|마이페이지(임대인)|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/ce9d6461-08cf-4379-b481-37edc7bd7c96" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/40424e43-13ae-45ee-980b-cb7286471b24" />|

<br>

|매물 지도 검색|매물 상세 페이지|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/42ee9fb7-c8fa-4663-9f38-50d607103d61" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/83500f64-058d-447b-869d-8f83db703786" />|

<br>

|매물 리뷰 리스트|채팅방|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/bd87916d-01de-4010-8886-410ccfcf32de" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/39d33e3c-18fc-4fb3-92cd-ab36cdd346f4" />|

<br>

|사용자 맞춤 매물 추천|전세계약 유형 테스트|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/2f5257da-6e36-4fa2-9701-86b7e6519f17" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/323e980e-72a9-47b5-9c02-d86b61a47d58" />|

<br>

|계약서 업로드|계약서 업로드 완료|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/55d37279-343e-4bef-a6aa-5674f44c4f0f" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/0eadc494-c10c-4d97-94e7-bec9935c87b2" />|

<br>

|지연이체 완료|지연이체 목록|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/3904f58b-e195-4187-bbb9-eaea20e6956a" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/3a0e397a-8a7b-4fb4-983c-a895109f5c47" />|

<br>

|등기부등본 분석|위험도 안전|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/db3f4020-d1b4-477f-bdb0-3ac9658cd9bc" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/1de28c33-5510-4b6f-a72e-06599812024c" />|

<br>

|위험도 중간|위험도 심각|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/58aa52d1-7fb8-49c9-8c31-2a81bdc30d01" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/dcebc1bb-a741-4fea-a39e-059ccabd734a" />|

<br>

|리뷰 작성|내 혜택함|
|:-:|:-:|
|<img width="374" height="768" alt="image" src="https://github.com/user-attachments/assets/5ae97eea-f6be-48cf-b04c-b41f8998339a" />|<img width="374" height="767" alt="image" src="https://github.com/user-attachments/assets/4ced5281-f5d4-4652-b312-86f996c301a7" />|

<br>
<br>

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


