---
title: "연습 3 - 사용자 지정 에이전트"
authors:
  - GitHub Copilot Learning Hub Team
lastUpdated: 2026-11-05
---

## 사용자 지정 에이전트란?

GitHub Copilot의 [사용자 지정 에이전트][custom-agents-concept]는 개발 워크플로의 특정 작업이나 영역에 맞춘 전문 AI 도우미를 만들 수 있게 합니다. 리포지토리의 `.github/agents` 폴더에 Markdown 파일로 에이전트를 정의합니다.

사용자 지정 에이전트로 다음을 살펴봅니다.

- 사용자 지정 에이전트를 정의하는 방법
- 사용자 지정 에이전트에 작업을 할당하는 방법

## 시나리오

Tailspin Toys는 모든 사용자가 크라우드 펀딩 플랫폼을 이용할 수 있도록 노력하고 있습니다. 디자인 팀은 고대비 모드 구현을 요청했습니다.

## 접근성 사용자 지정 에이전트 검토하기

Codespace로 돌아가 접근성 사용자 지정 에이전트 파일을 검토합니다.

1. `.github/agents/accessibility.md`를 엽니다.
2. `name` 및 `description` 필드가 있는 YAML frontmatter를 확인합니다.

> [!CAUTION]
> 사용자 지정 에이전트에는 `name` 및 `description` frontmatter가 필요합니다.

## 이슈 만들고 Copilot에 할당하기

1. 리포지토리로 이동합니다.
2. **Issues** 탭을 선택합니다.
3. **New issue**를 선택합니다.
4. **Title**에 `웹사이트에 고대비 모드 추가`를 입력합니다.
5. **Description**에 다음을 입력합니다.

    ```plaintext
    사이트에 고대비 모드를 추가해야 합니다. 사용자가 설정할 수 있는 고대비 토글이 있어야 하며, 브라우저의 로컬 스토리지에 설정을 저장해야 합니다.
    ```

6. **Create**를 선택하여 이슈를 만듭니다.
7. **Assign to Copilot**을 선택합니다.
8. 목록에서 **Accessibility agent**를 선택합니다.

    ![고대비 모드 이슈에 접근성 에이전트를 할당하는 화면](/images/learning-hub/copilot-workshops/ex5-select-custom-agent.png)

9. **Assign**을 선택합니다.

## 요약 및 다음 단계

GitHub Copilot의 [사용자 지정 에이전트][custom-agents]는 특정 작업과 영역을 위한 전문 AI 도우미입니다.

Copilot이 고대비 모드를 구현하는 동안 다음으로 [에이전트 세션을 모니터링하고 안내합니다][next-lesson].

## 리소스

- [사용자 지정 에이전트 정보][custom-agents]

---

| [← 이전 레슨: GitHub Copilot cloud agent][previous-lesson] | [다음 레슨: 에이전트 모니터링 및 관리 →][next-lesson] |
|:--|--:|

[previous-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/2-cloud-agent/
[next-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/4-managing-agents/
[custom-agents]: https://docs.github.com/copilot/concepts/agents/cloud-agent/about-custom-agents
[custom-agents-concept]: https://docs.github.com/copilot/concepts/agents/cloud-agent/about-custom-agents
