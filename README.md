# 이병용

* Email: ybyo@yibyeongyong.com
* Github: [https://github.com/ybyo](https://github.com/ybyo)
* 이력서: [resume-ko.yibyeongyong.com](https://resume-ko.yibyeongyong.com/)

학부 시절엔 정보보안을 학습하고 대학원에서 클라우드, 자원 사용량 모니터링, 분산 추적 등을 연구했습니다. 자원 사용량 모니터링 기술로 1건의 특허를 갖고 있습니다. 이런 지식과 연구 경험을 바탕으로 DevOps로서 커리어를 쌓아나가고 싶습니다. 이를 위해 AWS, DevOps 관련 서비스 및 기술들을 학습하고 있으며 개인 프로젝트도 진행하고 있습니다. 특히 관심이 많은 분야는 분산 추적 기술입니다. DevOps로서 계속 실력을 쌓아나가 분산 추적 분야의 전문가가 되는 것이 목표입니다.

---

# 프로젝트

수행했던 프로젝트 목록입니다. `resume-on-aws`는 졸업 후 개인적으로 진행한 프로젝트이며, `OpenFx-metering`은 석사 과정 중 진행했습니다.

| Title | Description | Used Techs |
| --- | --- | --- |
| resume-on-aws | AWS 리소스, DevOps 관련 기술들을 활용한 정적 웹 이력서 배포 | Python3, AWS, Github Actions |
| OpenFx-metering | 매우 낮은 오버헤드로 컨테이너 메모리 사용량을 모니터링하는 기술 | C, Python3, Linux Kernel Module |

# 프로젝트 상세

## Resume on AWS

AWS, DevOps 관련 기술들을 활용한 정적 웹 이력서 배포 프로젝트입니다. [Cloud Resume Challenge](https://cloudresumechallenge.dev/docs/the-challenge/aws/)라는 도전 과제들을 풀어나가며 진행했습니다. 단순히 ’이력서’만을 배포하는 일회성으로 프로젝트로 끝내는 것이 아니라 프로젝트 진행 중 의문이 들었던 내용 혹은 추가 개선이 가능한 아이디어가 생기면 이들을 개별 정리하고, 이러한 점들을 계속 프로젝트에 적용할 계획입니다.

도전 과제를 해결해나가며 AWS에 대해 많은 것을 배울 수 있었던 좋은 경험이었기에 이를 공유하고 싶었습니다. 게다가 한글로 작성된 가이드 자료가 없어 혹시 같은 도전 과제를 진행할 사람들에게 도움을 주고자 가이드 자료를 작성하고 있습니다.

### 주요 도전 과제

본래 제시된 도전 과제는 16항목이 존재하지만, 하나의 섹션으로 통합할 수 있는 부분들을 통합하여 다음과 같이 정리했습니다. 문서화 또한 다음 섹션 순서에 따라 진행하고 있습니다.

| Challenges | Description | Used Techs |
| --- | --- | --- |
| Resume | 이력서 작성 | HTML, CSS |
| HTTPS | 사용자, 엔드포인트 간의 안전한 연결 구성 | AWS CloudFront, Certificate Manager |
| View Count | 이력서에 들어갈 방문자 수 카운트 기능 구현 | Javascript, AWS DynamoDB, Lambda, API Gateway |
| IaC | AWS 리소스를 코드를 통해 API로 배포 | AWS CloudFormation, SAM |
| CI/CD | 이력서가 자동으로 배포되도록 구성 | Github Actions |

### 수행 기간

2022/05 ~ 지속 개선 중

### 관련 링크

* [레포지토리](https://github.com/ybyo/resume-on-aws)
* [배포 중인 이력서](http://resume-ko.yibyeongyong.com)
* [가이드](https://dev-wiki.yibyeongyong.com/projects/cloud-resume-challenge)

## API 호출 단위 자원 할당 및 사용량 계량이 가능한 서버리스 클라우드 컴퓨팅 기술 개발

석사 재학 중 메인으로 수행한 프로젝트입니다. 서버리스 클라우드 플랫폼 개발 및 배포를 위한 [OpenFX](https://github.com/keti-openfx/openfx) 프로젝트의 일환으로 진행했으며, 연구실이 맡은 부분은 컨테이너의 메모리 사용량을 아주 낮은 오버헤드로 모니터링하는 기술 개발이었습니다.

연구 결과 예상을 훨씬 웃도는 좋은 성능을 보였지만 몇 가지 아쉬운 점이 있었던 과제입니다.

* 실무에서의 활용 가능성
  * 연구했던 기술을 실제로 현업에서 활용할 수 있는지 혹은 실무에서 활용하려면 추가로 어떠한 개선이 필요한지 등에 대해서 현업에 계신 분들의 코멘트를 받지 못한 점
* 호환성 문제를 해결하지 못한 점
  * 리눅스 커널 모듈의 특성상 커널 버전에 따른 호환성이 매우 좋지 못했는데, 이를 해결하지 못한 점입니다. [eBPF](https://ebpf.io/) 같이 상대적으로 유연하면서 커널 내부에 유저 레벨 코드를 넣을 수 있는 기술을 활용하면 문제 해결이 가능할 수도 있을 거로 가설 정도만 세우고 있습니다. 나중에라도 함께 연구했던 연구실 선배와 후속 연구를 진행하고 싶습니다.

이 프로젝트를 진행하며 클라우드, 컨테이너, 가상 머신, Faas 등의 개념과 OpenStack, Kubernetes 등의 클라우드 플랫폼, 자원 사용량 모니터링 기술, procfs, 리눅스 커널 모듈, Linux perf 등 정말 많은 것을 배우고 경험할 수 있었던 뜻깊은 프로젝트였습니다. 또한, 프로젝트 중 다양한 오픈소스를 접하며 오픈소스에 깊은 관심을 가지게됐습니다.

### 기능 및 구성

| Features | Description | Used Techs |
| --- | --- | --- |
| Monitoring Module | procfs에 컨테이너 정보와 함께 메모리 사용량을 기록하는 모듈 | C, Linux Kernel Module |
| Kernel Module Manager | 모니터링 모듈을 제어하면서, 모니터링 대상 컨테이너들의 PID 리스트를 추출함 | Python3 |

### 관련 수상 실적

* 2019년도 한국정보보호학회 동계학술대회 [우수논문상](https://resume-ko.yibyeongyong.com/cisc-w19-prize.pdf) 수상
* [특허](https://resume-ko.yibyeongyong.com/patent-procmon.pdf) 등록(출원번호: 1020200019490)

### 수행 기간

2019/03 ~ 2020/12

### 관련 링크

* [레포지토리](https://github.com/keti-openfx/OpenFx-metering)
* 실험([Linux perf](https://www.brendangregg.com/perf.html)로 측정한 지표들을 기준으로 [cAdvisor](https://github.com/google/cadvisor)와 성능 비교)
  * [성능 비교](https://resume-ko.yibyeongyong.com/demo-1.mp4)(with Prometheus, Pushgateway, Grafana)
  * [성능 측정](https://resume-ko.yibyeongyong.com/demo-2.mp4)(with Portainer)

## 프로젝트 외 운영 중인 레포지토리

* [dev-wiki](https://github.com/ybyo/dev-wiki)
  * 개인 공부 내용, 프로젝트 수행 과정, 트러블슈팅 기록 용도로 사용 중인 레포지토리 입니다.
  * 공부한 내용을 복습할 때, 스마트폰 Github 앱에서 코드를 보면 가독성이 좋지 않아 Gitbook으로 퍼블리쉬 하고 있습니다(dev-wiki.yibyeongyong.com).
* [problem-solving](https://github.com/ybyo/problem-solving)
  * 알고리즘 문제 풀이 기록용 레포지토리입니다.
  * 주로 Leetcode 문제를 풉니다(C++, Python3).
  * Leetcode는 프리미엄 구독을 하지 않으면 Editorial을 볼 수 없습니다. 그래서 정답을 모르면 `Discussion` 탭에서 설명이 잘된 글을 열심히 찾아야 하는 번거로움이 있습니다. 혹시나 이 레포지토리를 방문하는 다른 사람들은 이러한 번거로움을 겪지 않았으면 해서 개인적으로 정리가 잘 됐다고 생각한 해설들은 `Helpful Links`로 남겨두고 있습니다.
* [automation-scripts](https://github.com/ybyo/automation-scripts)
  * 업무 자동화 스크립트 공부 및 코드 공유 목적으로 운영중입니다.

## 오픈소스 기여

마음 같아선 버그 픽스, 기능 개선 등으로 기여하고 싶지만, 아직 오탈자 제보 등에 그치고 있습니다. 그래도 메인테이너가 빠르게 merge 해주어 기분 좋은 경험이었습니다.

* devops-exercises - [fix typo](https://github.com/bregman-arie/devops-exercises/pull/255)
