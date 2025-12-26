# Chapter 1 README 생성
cat > chapter-01/README.md << 'EOF'
# Chapter 1: Terraform의 한계 이해하기

## 학습 목표

- Terraform 기본 워크플로우 복습
- 멀티 환경 관리의 실제 문제 경험
- 코드 중복 문제 인식

## 실습 순서

### 1. 기본 VPC 생성 (01-basic-vpc)
단일 VPC를 Terraform으로 생성하는 기초 실습

### 2. 멀티 환경 문제 (02-multi-env-problem)
dev, staging, prod 3개 환경을 만들면서 문제점 발견

### 3. 코드 중복 분석 (03-code-duplication)
실제로 얼마나 코드가 중복되는지 측정

## 예상 소요 시간
- 이론: 30분
- 실습: 1시간
- 총: 1.5시간
EOF