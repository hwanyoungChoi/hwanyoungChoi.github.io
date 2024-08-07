---
title: Gitlab CI/CD 도입기
date: 2024-07-10 11:58:47 +09:00
tags: [frontend]
description:
---

<img src="/gitlab-ci-cd/gitlab.png" alt="개별 import">

작성 이유|

팀에 새로 합류한 지 두 달이 지났다. 그 동안 프로젝트 파악 겸 버그 이슈들을 처리하고 있었고 다음 빌드를 위한 API/디자인 시안이 나오기 전 까지 잠시 여유가 생겼다. 이 기간동안 몇몇 개선사항을 시도해보았고 그 중 CI/CD 도입기를 작성해본다.

배경|

내가 합류하기 전 프론트엔드 개발 인원은 3명이었고 3~4번 정도 디자인 스펙이 변경되며 재개발한 경험이 있다고 했다. 소수인원이 빠르게 개발을 해야함에 따라 코드리뷰 등의 과정은 생략되고 있었다.

위와 같은 히스토리와 더불어 단기간 내에 강력한 규칙을 정하기 보다는 최소한의 안전장치가 필요하다고 생각했다. (나 또한 얼마되지 않아 놓치는 부분이 있을 수 있고)
