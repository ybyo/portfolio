# 이병용

* Email: ybyo@yibyeongyong.com
* Resume: [resume-ko.yibyeongyong.com](https://resume-ko.yibyeongyong.com/)

정보보안과 클라우드를 어우르는 경험을 쌓아왔습니다. 학부 시절엔 정보보안을 학습하고 대학원에선 클라우드를 연구하였습니다. 이러한 경험을 바탕으로 최근엔 DevOps 기술들을 활용한 개인 프로젝트를 진행하고 있으며, 관련된 직무로 커리어를 쌓아나가고 싶습니다.

## 프로젝트

석사과정 및 개인적으로 수행한 프로젝트 목록입니다.

| Title                                                                         | Description                      | Used Techs                      |
|-------------------------------------------------------------------------------|----------------------------------|---------------------------------|
| [OpenFx-metering](https://github.com/keti-openfx/OpenFx-metering/tree/master) | Container, VM 대상 메모리 사용량 모니터링 도구 | C, Python3, Linux Kernel Module |
| [resume-on-aws](https://github.com/ybyo/resume-on-aws)                        | AWS 리소스를 활용한 정적 웹 이력서 배포         | Python3, AWS                    |

## 프로젝트 상세

### Resume on AWS

AWS 리소스를 활용한 정적 웹 이력서 배포. 개인 학습 목적으로 진행한 프로젝트

#### 기능 및 구성

|  Features  | Description                     | Used Techs                                            |
|:----------:|---------------------------------|-------------------------------------------------------|
| View Count | 이력서에 들어갈 방문자 수 카운트 기능 구현        | Javascript, AWS API Gateway, AWS Lambda, AWS DynamoDB |
|   HTTPS    | 사용자, 엔드포인트 간의 안전한 연결 구성         | AWS CloudFront, AWS Certificate Manager               |
|    IaC     | AWS 리소스를 코드를 통해 API로 배포         | AWS CloudFormation, AWS SAM                           |
|   CI/CD    | Github에 갱신된 변경사항이 자동으로 배포되도록 구성 | Github Actions                                        |

#### 수행 기간

2022/05 ~ 지속 개선 중

#### 관련 링크

* [레포지토리](https://github.com/ybyo/resume-on-aws)
* [이력서](https://resume-ko.yibyeongyong.com/)

### API 호출 단위 자원 할당 및 사용량 계량이 가능한 서버리스 클라우드 컴퓨팅 기술 개발(석사)

클라우드 환경에서 가상 머신, 컨테이너의 메모리 사용량을 낮은 오버헤드로 측정하는 기술 연구.

#### 기능 및 구성

|       Features        | Description                       | Used Techs             |
|:---------------------:|-----------------------------------|------------------------|
|   Monitoring Module   | Container, VM 대상 낮은 오버헤드로 모니터링 수행 | C, Linux Kernel Module |
| Kernel Module Manager | 모니터링 모듈 제어, 모니터링 대상 PID 추출        | Python3                |

#### 관련 수상 실적

 * 2019년도 한국정보보호학회 동계학술대회 [우수논문상](https://resume-ko.yibyeongyong.com/cisc-w19-prize.pdf) 수상
 * [특허](https://resume-ko.yibyeongyong.com/patent-procmon.pdf) 등록(출원번호: 1020200019490)

#### 수행 기간

2019/03 ~ 2021/12

#### 관련 링크

* [레포지토리](https://github.com/keti-openfx/OpenFx-metering)
* 데모 영상
   * [성능 비교](https://resume-ko.yibyeongyong.com/demo-1.mp4)
   * [성능 측정](https://resume-ko.yibyeongyong.com/demo-2.mp4)

## 운영 중인 레포지토리

| Title                                                            | Description                              | Used Techs |
|------------------------------------------------------------------|------------------------------------------|------------|
| [automation-scripts](https://github.com/ybyo/automation-scripts) | 반복 업무 자동화 스크립트                           | Python3    |
| [dev-wiki](https://github.com/ybyo/dev-wiki)                     | 개인 공부 내용, 프로젝트 수행 과정, Troubleshooting 기록 | Markdown   |
| [problem-solving](https://github.com/ybyo/problem-solving)       | 알고리즘 문제 풀이.<br/> 주로 Leetcode Daily 풀이 수행 | C++        |
