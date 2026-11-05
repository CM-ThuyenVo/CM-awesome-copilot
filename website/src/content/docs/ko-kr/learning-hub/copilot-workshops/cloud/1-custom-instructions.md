---
title: "연습 1 - 사용자 지정 지침(Cloud agent)"
authors:
  - GitHub Copilot Learning Hub Team
lastUpdated: 2026-11-05
---

[← 이전 레슨: 사전 준비][previous-lesson] · [다음 레슨: Copilot cloud agent →][next-lesson]

생성형 AI를 사용할 때는 컨텍스트가 중요합니다. 특정 방식으로 작업해야 하거나 Copilot이 알아야 할 배경 정보가 있다면, 해당 컨텍스트를 Copilot이 사용할 수 있도록 해야 합니다. [지침 파일][instruction-files]은 Copilot에 지침을 제공하여 원하는 작업뿐 아니라 작업 방식도 이해하도록 돕습니다.

이 연습에서는 다음을 수행합니다.

- 리포지토리 사용자 지정 지침과 경로 범위 지침 파일을 통해 프로젝트 컨텍스트, 코딩 지침, 문서 표준이 Copilot에 전달되는 방식을 살펴봅니다.
- `.github/copilot-instructions.md`에 새로운 리포지토리 전체 표준을 추가합니다.

> [!NOTE]
> VS Code 및 CLI 과정과 달리 여기서는 전후 결과를 비교하는 프롬프트를 실행하지 않습니다. Copilot cloud agent는 GitHub 이슈를 비동기적으로 처리하므로 실시간으로 나란히 비교하기 어렵습니다. 이 과정의 뒷부분에서 cloud agent가 만든 풀 리퀘스트를 검토할 때 지침 파일의 영향을 확인합니다.

## 지침 파일

### 시나리오

Tailspin Toys에는 개발 관행에 관한 표준과 요구 사항이 있습니다.

- 데이터 계층에는 항상 단위 테스트가 필요합니다.
- UI는 어두운 모드와 현대적인 느낌을 사용해야 합니다.
- 코드에는 TSDoc 문서 주석을 추가해야 합니다.
- 각 파일의 맨 위에는 파일의 역할을 설명하는 주석 블록을 추가해야 합니다.

지침 파일을 사용해 Copilot이 이러한 관행에 따라 작업하는 데 필요한 정보를 제공합니다.

## 이 프로젝트의 사용자 지정 지침 파일 살펴보기

이 리포지토리에는 핵심 `copilot-instructions.md` 파일 하나와 다양한 작업을 위한 `*.instructions.md` 파일 모음이 있습니다. 편집기 또는 GitHub 웹 UI에서 파일을 엽니다.

1. `.github/copilot-instructions.md`를 엽니다.
2. 프로젝트에 대한 간단한 설명과 **Agent notes**, **Code standards**, **Scripts**, **Repository Structure** 등의 섹션을 살펴봅니다.
3. `.github/instructions` 폴더를 열어 파일을 살펴봅니다.

## 새로운 리포지토리 표준 추가하기

1. Codespace 터미널에서 새 브랜치를 만들고 전환합니다.

   ```bash
   git checkout -b custom-instructions-cloud
   ```

2. `.github/copilot-instructions.md`를 엽니다.
3. **Code formatting requirements** 섹션을 찾습니다.
4. 기존 표준 바로 아래에 다음 Markdown을 추가합니다.

   ```markdown
   - 내보내는 모든 함수에는 목적, 매개 변수, 반환 값을 설명하는 TSDoc 주석을 작성합니다.
   - 가져오기 구문이나 코드를 작성하기 전에 파일의 목적을 설명하는 주석 블록을 추가합니다.
   ```

5. `copilot-instructions.md`를 저장합니다.

## 지침 업데이트 커밋, 푸시, 병합하기

1. 스테이징하고 커밋합니다.

   ```bash
   git add .github/copilot-instructions.md
   git commit -m "Add doc comment and file-header standards to copilot instructions"
   ```

2. 브랜치를 푸시하고 `main`으로 풀 리퀘스트를 열고 병합합니다.

## 요약 및 다음 단계

지침 파일을 살펴보고 `.github/copilot-instructions.md`에 리포지토리 전체 표준을 추가했습니다.

다음으로 [첫 이슈를 Copilot cloud agent에 할당합니다][next-lesson].

## 리소스

- [GitHub Copilot 사용자 지정 지침 파일][instruction-files]

[previous-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/0-prerequisites/
[next-lesson]: /ko-kr/learning-hub/copilot-workshops/cloud/2-cloud-agent/
[instruction-files]: https://docs.github.com/copilot/customizing-copilot/about-customizing-github-copilot-chat-responses
