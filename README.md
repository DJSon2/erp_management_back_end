# erp_management
결제, 관리 시스템

# 프로그램 구조 구성
REST API를 활용하며 React, Spring Boot로 웹을 구성 
기존에 경험했었던 DB가 아닌 NOSQL 방식을 사용해 다른 DB를 사용할 예정

# 적용된 Starter
- JDBC API
- Oracle Driver
- Spring Boot DevTools
- Spring Web
- Spring Security
- Spring Data Jpa

# 사용 프로그램
IDE : VsCode, STS4
DB : OracleDB

# 주 목적 기능
1. 전산 회계 시스템
2. 결제 시스템과 액셀 표 저장
3. 카드 결제 매출 카드사 별 표시

# 상세 기능
- 결제
  - pos 마감 -> 내역 저장(현금 포함)
  - 카드 결제 = 카드사 별 나눠서 저장
  - 결제 예시
    - 매출 1000만원 
        - 현금 200만원
        - 카드 800만원
          - BC, KB, 롯데, 신한 등 
    - 하루 전체 매출, 현금 and 카드 구분 표시, 카드사 별 결제 금액 표시

- 입금
  - 카드사 별 다른 사항
    - 입금 날짜 -> 3 ~ 5 영업일 
      - 영업일 = 공휴일 제외
      - 공휴일 껴있는 경우 2 ~ 3일 매출 한번에 입금
    - 카드 수수료 0.2% or 0.1%
      - 직불, 신용에 따라 수수료 다름 -> 일부 반환
    - 이중결제 고려
  - 입근된 데이터 엑셀로 저장
    - 카드사 별 매출 확인 및 매출일 확인(수수료 계산 후)

# 필요 DB 스키마
- 회원 관리
  - 회원 정보
- 매출 관리
  - 영업일
  - 매출
  - 입금
  - 카드사 종류

# DB 테이블 구조
[https://www.erdcloud.com/](https://www.erdcloud.com/d/hoa4sedK9iJsQkNEh)

# 피그마 
https://www.figma.com/file/I3vqQzjSq29VsWMuUHXw5F/Untitled?type=design&t=V2Or9KpXKYnBT8gG-0

# React 주소
