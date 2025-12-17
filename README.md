# Escro Project

**안전하고 투명한 중고 거래를 위한 블록체인 기반 Web3 플랫폼**

## 프로젝트 소개 (Introduction)
이 프로젝트는 기존 중고 거래의 신뢰성 문제를 해결하기 위해 블록체인 기술을 도입한 웹 애플리케이션입니다.  
사용자는 물품을 등록하고, 구매자는 원하는 가격을 **제안** 할 수 있으며, 판매자가 이를 수락하면 **스마트 컨트랙트**를 통해 안전하게 거래가 기록됩니다.

### 기획 의도
* **가격 제안 시스템**: 정가 구매뿐만 아니라, 구매자가 합리적인 가격을 제안하는 경매 방식을 차용했습니다.
* **상태 관리**: `finding(판매중)` → `waiting(수락 대기)` → `matched(매칭 완료)`의 명확한 상태 변화를 통해 거래 흐름을 시각화했습니다.
* **스마트 컨트랙트와 연동**: 거래가 확정되면 블록체인상에 거래 내용을 영구적으로 기록하여 위변조를 방지합니다.

## 주요 기능 및 화면 (Features & Screenshots)

### 1. 메인 및 상품 상세 (Marketplace)
사용자는 등록된 상품을 둘러보고, 상세 페이지에서 댓글을 남기거나 거래를 신청할 수 있습니다.

| 상품 목록 (List) | 상품 상세 (Detail) |
| :---: | :---: |
| <img width="1356" height="625" alt="스크린샷 2025-12-17 230923" src="https://github.com/user-attachments/assets/75ff454f-5307-46c1-b826-e3b84fe96d40" />| <img width="1278" height="744" alt="스크린샷 2025-12-17 230949" src="https://github.com/user-attachments/assets/165d3623-e334-494b-9ab2-421d52b986df" />|
| *직관적인 카드형 UI와 검색 기능* | *상품 정보 확인 및 댓글, 거래 신청 기능* |


### 2. 가격 제안 및 거래 요청 (Trade Offer)
구매자는 판매자에게 원하는 가격을 입력하여 거래를 요청합니다.

<img width="1350" height="204" alt="스크린샷 2025-12-17 231000" src="https://github.com/user-attachments/assets/c2f8e013-7691-4df4-8d2f-ae44895440b4" />

* **Custom Price**: 정해진 가격이 아닌 구매자가 원하는 가격 제시 가능 (`99,999` 등).

### 3. 판매자 관리 및 수락 (Seller Dashboard)
판매자는 들어온 요청 목록을 확인하고, 원하는 제안을 `수락(Select)`하거나 `거절(Reject)`할 수 있습니다.

| 거래 요청 목록 | 거래 수락/거절 |
| :---: | :---: |
| <img width="1354" height="602" alt="스크린샷 2025-12-17 231015" src="https://github.com/user-attachments/assets/fa1b0e82-d134-4ba2-959a-81cb14baaf68" />| <img width="1347" height="176" alt="스크린샷 2025-12-17 231036" src="https://github.com/user-attachments/assets/5d682619-c138-41fe-8d9d-9a22eba49a59" />|
| <img width="1354" height="602" alt="스크린샷 2025-12-17 231015" src="https://github.com/user-attachments/assets/80ee03aa-89f5-4cb5-8c76-69c5e6b8a64d" />| <img width="1340" height="651" alt="스크린샷 2025-12-17 231030" src="https://github.com/user-attachments/assets/4ca881f3-ab48-49be-81a0-8f2b0be90380"/>|

### 4. 마이페이지 및 컨트랙트 등록 (My Page & Smart Contract)
거래가 성사되면 상태가 `matched`로 변경되며, 스마트 컨트랙트에 거래 정보를 등록할 수 있습니다.

<img width="1333" height="668" alt="스크린샷 2025-12-17 231043" src="https://github.com/user-attachments/assets/d6a025ed-e67d-46f1-b51d-a3b627c3673b" />

* **지갑 연동**: 개인 지갑 주소 등록 및 관리.
* **Smart Contract Registration**: 매칭된 건에 대해 온체인(On-chain) 등록 버튼 활성화.

---
## 🛠 기술 스택 (Tech Stack)
### Frontend
* ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white) **Next.js**

### Backend & Database
* ![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white) **NestJS**
* ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white) **PostgreSQL**

### Blockchain
* ![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat&logo=solidity&logoColor=white) **Solidity**

---
### Prerequisites
* Node.js (v20.0.0 이상)
* Metamask (브라우저 익스텐션)

