---
title: "연습 4 - 에이전트 모니터링 및 관리"
authors:
  - GitHub Copilot Learning Hub Team
lastUpdated: 2026-11-05
---

앞선 두 연습에서는 Copilot cloud agent에 사용자 경험을 개선하고 기능을 추가하는 세 가지 작업을 요청했습니다. Cloud agent는 비동기적이고 자율적으로 작동하지만, 작업을 모니터링하는 것도 중요합니다.

이 레슨에서는 다음을 수행합니다.

- agents 페이지에서 cloud agent 작업을 모니터링합니다.
- 진행 중인 세션에 추가 기능을 요청합니다.

## 시나리오

접근성 에이전트가 고대비 모드를 만들도록 요청한 뒤, 팀은 밝은 모드도 함께 추가하기로 했습니다. 에이전트에 추가 지침을 보내 고대비 모드와 밝은 모드를 모두 구현하도록 합니다.

## Copilot cloud agent 작업 검토하기

1. [Copilot agents 페이지](https://github.com/copilot/agents)로 이동합니다.
2. 기본 창과 왼쪽 창에 표시되는 작업 목록을 살펴봅니다.
3. 실행 중인 작업 하나를 선택하고 Copilot이 수행한 작업을 검토합니다.

## Cloud agent에 추가 지침 보내기

1. 고대비 모드 작업을 진행 중인 세션을 선택합니다.

    ![제어 센터의 접근성 세션](/images/learning-hub/copilot-workshops/ex6-accessibility-session.png)

2. **Steer active session while Copilot is working** 대화 상자에 다음 프롬프트를 입력합니다.

    ```plaintext
    고대비 모드를 만드는 김에 밝은 모드도 추가해 주세요. 사용자가 원하는 표시 모드를 선택할 수 있도록 밝은 모드 토글도 제공해야 합니다.
    ```

    ![agents 페이지의 cloud agent 작업에서 활성 세션 안내 대화 상자를 강조한 스크린샷](/images/learning-hub/copilot-workshops/ex6-steer-cloud-agent-task.png)

3. <kbd>Enter</kbd>를 눌러 프롬프트를 보냅니다.

## 요약 및 다음 단계

Copilot cloud agent 작업을 모니터링하고 안내하는 중심 공간인 Copilot agents 페이지를 살펴봤습니다.

## 리소스

- [Copilot agents 페이지][agents-page]

---

| [← 이전 레슨: 사용자 지정 에이전트][previous-lesson] |
|:--|

[previous-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/3-custom-agents/
[agents-page]: https://github.blog/changelog/2025-07-03-agents-page-for-copilot-coding-agent-in-public-preview
