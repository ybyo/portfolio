# 이병용
Email: ybyo@yibyeongyong.com

정보보안과 클라우드를 어우르는 경험을 쌓아온 이병용입니다. 학부 시절엔 정보보안을 학습하고 대학원에선 클라우드를 연구하였습니다. 이러한 경험을 바탕으로 최근엔 DevOps 기술들을 활용한 개인 프로젝트를 진행하고있으며, 관련된 직무로 커리어를 쌓아나가고 싶습니다.

## Projects

| Title | Description | Used Techs |
|---|---|---|
| [OpenFx-metering](https://github.com/keti-openfx/OpenFx-metering/tree/master) | Container, VM 대상 메모리 사용량 모니터링 도구 | C, Python3, Linux Kernel Module |
| [Resume on AWS](https://github.com/ybyo/resume-on-aws) | AWS 리소스를 활용한 정적 웹 이력서 배포 | Python3, AWS |
| Carver(WIP) | Git 기반 복습 도구 | Python3, Golang |

## Projects Details

### Resume on AWS

AWS 리소스를 활용한 정적 웹 이력서 배포. 개인 프로젝트

#### Features

| Features | Description | Used Techs |
|:---:|---|---|
| View Count | 이력서에 들어갈 방문자 수 카운트 기능 구현 | Javascript, AWS API Gateway, AWS Lambda, AWS DynamoDB |
| HTTPS | 사용자, 엔드포인트 간의 안전한 연결 구성 | AWS CloudFront, AWS Certificate Manager |
| IaC | AWS 리소스를 코드를 통해 API로 배포 | AWS CloudFormation, AWS SAM |
| CI/CD | Github에 갱신된 변경사항이 자동으로 배포되도록 구성 | Github Actions |

#### 수행 기간

2022/05 ~ 지속 개선 중

#### 관련 링크

 * [이력서](https://resume-ko.yibyeongyong.com/)
 * [레포지토리](https://github.com/ybyo/resume-on-aws)

### API 호출 단위 자원 할당 및 사용량 계량이 가능한 서버리스 클라우드 컴퓨팅 기술 개발

클라우드 환경에서 가상 머신, 컨테이너의 메모리 사용량을 낮은 오버헤드로 측정하는 기술 연구

석사 과정 중 진행한 프로젝트

#### Features

 * 가상머신, 컨테이너를 대상으로 메모리 사용량을 낮은 오버헤드로 측정하는 리눅스 커널 모듈 개발
 * 상기 리눅스 커널 모듈을 제어하는 커널 모듈 매니저 개발
 * 2019년도 한국정보보호학회 동계학술대회 [우수논문상](https://resume-ko.yibyeongyong.com/cisc-w19-prize.pdf) 수상
 * [특허](https://resume-ko.yibyeongyong.com/patent-procmon.pdf) 등록(출원번호: 1020200019490)
 * 팀 구성
   * 커널 모듈 개발3, 커널 모듈 매니저 개발1, 개발 환경 구성1
 * 맡은 역할
   * 커널 모듈 개발 및 개발 환경 구성 담당

#### 수행 기간

2019/03 ~ 2021/12

#### 관련 링크

 * [레포지토리](https://github.com/keti-openfx/OpenFx-metering)
