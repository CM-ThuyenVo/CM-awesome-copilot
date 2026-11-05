---
title: "연습 2 - GitHub Copilot cloud agent"
authors:
  - GitHub Copilot Learning Hub Team
lastUpdated: 2026-11-05
---

| [← 이전 레슨: 사용자 지정 지침][previous-lesson] |
|:--|

기술 부채로 어려움을 겪지 않는 조직은 거의 없습니다. GitHub Copilot cloud agent는 코드를 업데이트하고 기능을 추가하는 등의 작업을 자율적으로 수행합니다. 작업을 마치면 사람이 검토할 수 있도록 초안 PR을 엽니다.

이 연습에서는 Copilot cloud agent를 다음과 같이 활용합니다.

- 코드 생성 환경을 사용자 지정합니다.
- 작업이 안전하게 수행되는지 확인합니다.
- 범위가 명확한 이슈의 중요성을 살펴봅니다.
- 이슈를 Copilot에 할당합니다.

## 시나리오

Tailspin Toys에는 해결할 기술 부채가 있습니다. 초기 웹사이트를 만든 계약 업체가 문서를 충분히 작성하지 않았습니다. 먼저 애플리케이션에서 내보내는 모든 함수에 TSDoc 문서 주석을 추가하려고 합니다.

## 문서 추가하기

1. 새 브라우저 탭에서 github.com의 리포지토리로 이동합니다.
2. **Issues** 탭을 선택합니다.
3. **New issue**를 선택하여 새 이슈 대화 상자를 엽니다.
4. **Blank issue**를 선택합니다.
5. **Title**에 `코드에 문서가 부족합니다`를 입력합니다.
6. **Description**에 다음을 입력합니다.

    ```plaintext
    우리 조직에서는 함수와 메서드에 도움이 되는 경우 TSDoc 문서 주석을 포함하도록 요구합니다. 동작을 명확히 하는 경우 문서 주석이 포함되도록 기존 코드를 업데이트해야 합니다.
    ```

7. **Create**를 선택하여 이슈를 만듭니다.
8. 오른쪽에서 **Assign to Copilot**을 선택하여 할당 대화 상자를 엽니다.

    ![이슈에 Copilot을 할당하는 화면](/images/learning-hub/copilot-workshops/shared-assign-copilot.png)

9. **Assign**을 선택합니다.
10. **Pull Requests** 탭을 선택합니다.
11. 새 풀 리퀘스트(PR)를 엽니다.
12. Copilot이 할 일 목록을 만든 것을 확인합니다.

## 게임 상세 페이지에 관련 게임 섹션 추가하기

1. github.com의 리포지토리로 돌아갑니다.
2. **Issues** 탭을 선택합니다.
3. **New issue**를 선택합니다.
4. **Title**에 `게임 상세 페이지에 관련 게임 표시`를 입력합니다.
5. **Description**에 다음을 입력합니다.

    ```markdown
    사용자가 더 많은 게임을 발견할 수 있도록 각 게임 상세 페이지에 관련 게임을 표시하려고 합니다. 요구 사항은 다음과 같습니다.

    - `src/lib/`에 지정한 게임을 제외하고 같은 카테고리의 다른 게임을 반환하는 데이터 접근 도우미를 추가합니다.
    - 해당 도우미를 사용하는 "관련 게임" 섹션을 게임 상세 페이지에 표시합니다.
    - 관련 게임이 없는 경우를 처리합니다.
    - 새 도우미에 대한 단위 테스트를 작성합니다.
    - PR을 만들기 전에 모든 테스트가 통과하는지 확인합니다.
    ```

6. **Create**를 선택하여 이슈를 만듭니다.
7. **Assign to Copilot**을 선택하고 **Assign**을 선택합니다.

## 요약 및 다음 단계

이 연습에서는 Copilot cloud agent에 이슈를 할당하는 방법을 살펴봤습니다.

## 리소스

- [Copilot cloud agent 정보][copilot-agents]
- [GitHub 이슈를 Copilot에 할당하기][assign-issue]

| [다음 레슨: 사용자 지정 에이전트 →][next-lesson] |
|--:|

[previous-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/1-custom-instructions/
[next-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/3-custom-agents/
[copilot-agents]: https://docs.github.com/copilot/concepts/agents/cloud-agent/about-cloud-agent
[assign-issue]: https://docs.github.com/copilot/how-tos/use-copilot-agents/cloud-agent/start-copilot-sessions
