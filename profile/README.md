# [🏠전 새내기]
### KB IT's Your Life 6기 최종 프로젝트 (2025.07.09 ~ 2025.08.21)

▶️[서비스 바로가기 Click!](https://new-bie.o-r.kr/)

<br>

## 📚 목차  
[![프로젝트 소개](https://img.shields.io/badge/프로젝트_소개-FF6B6B?style=flat-square)](#1-프로젝트-소개)  
[![프로젝트 배경](https://img.shields.io/badge/프로젝트_배경-F78DA7?style=flat-square)](#2-프로젝트-배경)  
[![서비스 화면](https://img.shields.io/badge/서비스_화면-FFD93D?style=flat-square)](#3-서비스-화면)  
[![핵심 기능](https://img.shields.io/badge/핵심_기능-4D96FF?style=flat-square)](#4-핵심-기능)  
[![개발 환경](https://img.shields.io/badge/개발_환경-6BCB77?style=flat-square)](#5-개발-환경)  
[![설계 문서](https://img.shields.io/badge/설계_문서-A0A0A0?style=flat-square)](#6-설계-문서)  
[![전새내기를 만든 사람들](https://img.shields.io/badge/전새내기를_만든_사람들-3A506B?style=flat-square&logo=github&logoColor=white)](#7-전새내기를-만든-사람들)  

<br>

## 1. 프로젝트 소개
### 부동산 안심 계약 플랫폼 "전 새내기"  
![Image](https://github.com/user-attachments/assets/49239ffc-a7ca-43bd-893a-387b22757131)  ![Image](https://github.com/user-attachments/assets/793e6173-07e1-4b88-8656-74a11b3fdd26)  

  &nbsp;  
  
## 2. 프로젝트 배경

### 문제 인식
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

  &nbsp;  
  
[![맨_위로](https://img.shields.io/badge/맨_위로-FFD93D?style=flat-square)](#-목차)   

## 3. 서비스 화면 
### (1) 로그인 
- spring security를 사용한 회원가입 / 로그인
- 계약서 및 계좌 활용을 위한 개인정보 수집 동의
<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/0a5cfc2f-c354-4492-bcc6-9fab34629c21" />

<br>

### (2) 마이페이지 / 추천
- 임차인/임대인 마이페이지
- 임대인은 지연이체 활성화 토글로 서비스 사용 여부 결정
- 지연이체 로딩바로 현제 지연이체 상태 확인
- 첫 로그인시 입력한 정보 기반으로 매물 추천

<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/58251027-cb0d-45c3-a701-0ba0ea49c0c1" />  
<br>  
  
### (3) 지도 
- Kakao Map API, Daum 우편번호 API를 사용해서 지도 보기, 검색 가능
- 지도에 매물 마커가 표시되고 범위에 맞는 리뷰와 매물이 조회  

<img width="1246" height="751" alt="Group 1989" src="https://github.com/user-attachments/assets/b3fa3243-426a-4a2f-be2f-7b68fb154181" />

<br>

### (4) 매물 상세 - 리뷰 - 채팅방  
- 매물 상세페이지에서 매물에 달린 리뷰 조회
- 리뷰에는 납부 인증 뱃지, 장단점, 해당 리뷰가 작성된 시점의 계절 아이콘 등이 표시
- 리뷰 리스트에 있는 채팅하기 버튼을 통해 퇴거자(리뷰 작성자)와 실시간 채팅 가능
  
<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/964c03bb-cc5f-47ba-b386-2106e5646f07" />
<br>

### (5) 전세계약 유형 테스트    
- 집 계약시 본인에게 일어날 수 있는 사기 유형 테스트 기능
- 결과로는 공통적으로 조심해야할 부분, 취약한 사기 유형을 출력

<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/e0160555-4a8c-45a6-9500-7aa410860734" />
<br>

### (6) 계약서 업로드   
- 실제 본인 집 계약서를 업로드
- Chat GPT API를 사용해 ocr 분석 후 출력
- 만약 일치하지 않는 부분이 있다면 수동으로 수정 후 제출  
  
<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/fedf192a-c07a-41c8-9618-28adae42a11e" />
<br>

### (7) 지연 이체 - 보증금 납부 
- 계약서를 업로드 하였다면 지연 이체 납부 가능
- 계약서 정보를 가져와 자동으로 입력해 주고, 한 번 더 확인 후 이체
- 아무 이상이 없다면 7일 후 자동으로 이체 완료  
  
<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/08074f42-ff21-47fd-ab68-86a3e3b873f0" />

<br>

### (8) 등기부등본 분석 위험도 안전/경고
- 업로드 되어있는 계약서와 등기부등본을 대조
- 등기부등본은 codef의 등기부등본 열람 API를 사용하여 자동으로 조회
- 등기부등본 내용과 계약서 내용을 대조한 결과를 출력. 만약 불일치 항목 존재시 지연 이체 취소 신청 가능
  
<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/b831c135-c17f-4f03-b743-d284ecb33dc9" />

<br>

### (8) 리뷰 작성 - 내 혜택함
- 계약금 납부 후 일정 기간 납부 완료시(3개월) 리뷰 작성 가능
- 계절별로 리뷰를 작성할 수 있으며, 해당 계절에 맞는 ui로 계절감 어필
- 리뷰 작성 완료시 내 혜택함에서 쿠폰 발급 가능
<img width="1246" height="751" alt="Image" src="https://github.com/user-attachments/assets/dbb76983-ff5e-4e57-a77c-0c4cd81ff054" />
<br>
<br>

  &nbsp;  
  [⬆️ 맨 위로](#-목차)
  
## 4. 핵심 기능

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


  &nbsp;  

  
## 5. 개발 환경
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

  &nbsp;  
  [⬆️ 맨 위로](#-목차)

## 6. 설계 문서 
### ▶️[ERD 보러가기](https://www.erdcloud.com/d/Ce29KPQL8rBtiy4qd)  
* 아래 이미지는 주요 기능을 정리한 것으로 실제 다이어그램과 차이가 있습니다 
<img width="975" height="2343" alt="Image" src="https://github.com/user-attachments/assets/0b4aa7f3-2ab3-450b-b97f-af45101c360a" />
<br>
<br>

### ▶️[API 명세서 보러가기](https://ultra-playground-0a9.notion.site/API-2542350d416c80208c98c09c1b1033fc?source=copy_link)

<br>
 
  &nbsp;  
  
## 7. 전새내기를 만든 사람들   

<img width="900" height="1024" alt="Image" src="https://github.com/user-attachments/assets/fd2d8c7f-4648-49c7-b798-8af65254ae6a" />   

![2025-08-20 21-14-02](https://github.com/user-attachments/assets/cb089e00-f891-417f-ac26-564ff27ace7b)


