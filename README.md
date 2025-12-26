# Terraform to Terragrunt: AWS 인프라 구축 실전 가이드

## 소개

이 저장소는 "Terraform to Terragrunt: AWS 인프라 구축 실전 가이드" 책의 실습 코드를 담고 있습니다.

## 대상 독자

- Terraform 기본 문법을 알고 있는 중급 개발자
- AWS 인프라를 운영 중이지만 코드 중복과 관리 복잡도로 고민하는 DevOps 엔지니어
- 의료기기/규제 산업에서 컴플라이언스를 고려한 인프라 관리가 필요한 개발자

## 책 구성

### Chapter 1: Terraform의 한계 이해하기 (Week 1)
- Terraform 기본 복습
- 실무에서 발생하는 문제점
- 멀티 환경 관리의 어려움

### Chapter 2: Terraform 모듈 설계 패턴 (Week 2)
- 재사용 가능한 모듈 작성
- Data Sources와 Remote State
- 의존성 관리

### Chapter 3: Terragrunt 핵심 개념 (Week 3)
- Terragrunt 소개와 DRY 원칙
- 계층적 디렉토리 구조
- Backend 자동 구성

### Chapter 4: 환경별 변수 관리 전략 (Week 4)
- inputs 블록 활용
- Secrets 관리
- 의료기기 규정 준수 사례

### Chapter 5: CI/CD와 자동화 (Week 5)
- GitOps 워크플로우
- Policy as Code
- 자동화 파이프라인

### Chapter 6: 실전 마이그레이션 (Week 6)
- Terraform → Terragrunt 전환
- 프로덕션 환경 적용
- 트러블슈팅

### Chapter 7: 실전 프로젝트 (Week 7)
- 의료 재활 로봇 플랫폼 인프라 구축
- ECS + RDS + S3 통합
- 운영 베스트 프랙티스

## 사전 요구사항

- Terraform >= 1.0
- Terragrunt >= 0.48
- AWS CLI
- Git
- 개인 AWS 계정 (Free Tier 권장)

## 실습 환경 설정
```bash
# Terraform 설치 확인
terraform version

# Terragrunt 설치 (macOS)
brew install terragrunt

# AWS CLI 설정
aws configure
```

## 프로젝트 구조
```
terraform-to-terragrunt-book/
├── chapter-01/          # Week 1: Terraform 기초
├── chapter-02/          # Week 2: 모듈 설계
├── chapter-03/          # Week 3: Terragrunt 기초
├── chapter-04/          # Week 4: 변수 관리
├── chapter-05/          # Week 5: CI/CD
├── chapter-06/          # Week 6: 마이그레이션
├── chapter-07/          # Week 7: 실전 프로젝트
└── README.md
```

## 저자

조효성 (Rainbow Robotics)
- 13년+ 웹 개발 및 데이터 분석 경험
- 의료기기 FDA 사이버보안 규정 준수 인프라 구축
- AWS 인프라 관리 및 IaC 전문

## 라이선스

MIT License