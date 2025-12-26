# 01: 기본 VPC 생성

## 목표

Terraform으로 기본적인 VPC 네트워크를 생성합니다.

## 생성되는 리소스

- VPC (10.0.0.0/16)
- Public Subnet x 2 (Multi-AZ)
- Private Subnet x 2 (Multi-AZ)
- Internet Gateway
- Route Table

## 실습 순서

1. 코드 검토
```bash
# 파일 구조 확인
ls -la
```

2. Terraform 초기화
```bash
terraform init
```

3. 실행 계획 확인
```bash
terraform plan
```

4. 리소스 생성
```bash
terraform apply
```

5. 결과 확인
```bash
# Output 값 확인
terraform output

# AWS 콘솔에서 확인
# VPC > Your VPCs > "book-vpc" 검색
```

6. 리소스 삭제
```bash
terraform destroy
```

## 예상 비용

- VPC, Subnet, IGW, Route Table: **무료**
- 실습 시간: 약 20분

## 주요 학습 포인트

1. Terraform 기본 워크플로우 (init → plan → apply)
2. VPC 리소스 간 의존성 (VPC → Subnet → IGW)
3. Output을 통한 정보 확인
4. Multi-AZ 구성의 기초