# Claude Code Tips

> Claude Code를 효율적으로 사용하기 위한 학습 정리 노트

Claude Code의 핵심 기능과 활용법을 공부하면서 주제별로 정리하는 개인 학습 저장소입니다. 새로운 기능이나 개념을 익힐 때마다 폴더를 추가하고, 각 폴더 안에 개념 설명 · 시각 자료 · 실습 가이드를 함께 묶어둡니다.

---

## 📚 목차 (Contents)

학습한 순서대로 정리되어 있습니다. 각 폴더 이름은 `주제-YY-MM-DD` 형식으로, 학습한 날짜를 함께 기록합니다.

| 학습일 | 주제 | 한 줄 요약 |
|---|---|---|
| 2026-03-14 | [Claude Code Skills](./claude-code-skills-26-03-14/) | Skills = AI에게 주는 SOP(업무 매뉴얼) |
| 2026-03-21 | [NotebookLM × Claude Code](./notebooklm-claude-code-26-03-21/) | nlm CLI로 NotebookLM을 자연어로 제어하기 |
| 2026-03-28 | [Claude Code Scheduler](./claude-code-scheduler-26-03-28/) | Skill + Schedule로 자동화 시스템 구축 (Local vs Remote) |
| 2026-04-04 | [Computer Use](./computer-use-26-04-04/) | AI 자동화 방법 전체 맵 — API / MCP / CLI / Chrome / Computer Use |
| 2026-04-11 | [LLM Wiki (LLM 나무위키)](./llmwiki-26-04-11/) | Claude Code + Obsidian으로 만드는 개인 지식 베이스 |
| 2026-04-18 | [Routines](./routines-26-04-18/) | 반복 작업을 루틴(Routine)으로 자동화하기 |

---

## 🗂️ 폴더 구조 (Folder Structure)

각 학습 주제별 폴더는 다음과 같은 구성을 따릅니다.

```
주제-YY-MM-DD/
├── README.md          ← 개념 설명 · 셋업 · 실습 가이드
├── *.png              ← 구조도 · 비교표 · 워크플로 다이어그램
└── (기타 자료)        ← 프롬프트 템플릿 · 코드 스니펫 등
```

---

## 🧭 주제별 핵심 한눈에 보기

### 🛠️ Skills (스킬) — `claude-code-skills-26-03-14`
**Skills = AI에게 주는 SOP(Standard Operating Procedure, 업무 매뉴얼)**
매번 구두로 지시하는 대신, `SKILL.md`라는 매뉴얼을 만들어두면 AI가 동일한 품질의 결과물을 반복적으로 만들어냅니다.

### 📓 NotebookLM × Claude Code — `notebooklm-claude-code-26-03-21`
**nlm CLI**로 NotebookLM을 Claude Code에서 자연어로 제어합니다. MCP 서버 대신 CLI + 스킬 조합을 쓸 때의 장단점도 정리.

### ⏰ Scheduler (스케줄러) — `claude-code-scheduler-26-03-28`
**Skill + Schedule = 자동화 시스템.** N8N처럼 복잡한 노드 연결 없이 자연어로 "언제, 무엇을, 어떻게" 만 정의하면 끝.
- **Local Task**: 내 PC에서 실행 (모든 Connectors + 로컬 MCP, 컴퓨터 켜져있어야 함)
- **Remote Task**: Anthropic 클라우드에서 실행 (컴퓨터 꺼져도 동작, repo에 커밋된 스킬만 사용 가능)

### 🖥️ Computer Use — `computer-use-26-04-04`
AI 자동화 방법 전체 맵을 정리합니다.
- **API / MCP / CLI**: 공식 연동 수단 (Google, Slack, Notion 등)
- **코드 스크립트**: Playwright 등 (반복에 강함)
- **Claude in Chrome**: 코딩 없이 브라우저 조작
- **Computer Use**: 코딩 없이 데스크톱 앱 조작 (카카오톡, Finder 등)

### 🌳 LLM Wiki (LLM 나무위키) — `llmwiki-26-04-11`
Andrej Karpathy의 LLM Wiki 아이디어를 기반으로, **Claude Code + Obsidian**으로 개인 지식 베이스를 만드는 방법.
**3층 구조**: Schema (`CLAUDE.md`) → Wiki (`wiki/`) → Raw (`raw/`)
NotebookLM이나 RAG와 달리 **지식이 복리(Compounding)로 축적**되는 것이 핵심.

### 🔁 Routines (루틴) — `routines-26-04-18`
반복적인 작업을 루틴으로 만들어 자동 실행하는 방법.

---

## 🎯 학습 정리 원칙

- **개념 → 비교 → 실습** 순서로 정리합니다.
- 시각 자료(다이어그램 · 비교표)를 적극 활용해 한눈에 이해할 수 있게 만듭니다.
- 한국어 본문에 **핵심 영어 용어를 병기**해서, 공식 문서와도 자연스럽게 매칭되도록 합니다.
- 외부 자료를 참고한 경우 각 폴더 README에 **출처를 명시**합니다.

---

## 📖 이 저장소 활용법

1. **목차에서 관심 있는 주제 선택** → 해당 폴더 클릭
2. **폴더 안의 README** 먼저 읽기 (개념 + 사용법)
3. **이미지 자료**로 구조를 한눈에 파악
4. **실습 섹션**을 따라 직접 셋업해보기

---

## 🔗 참고 자료 (References)

- [Claude Code 공식 문서](https://docs.claude.com)
- [Andrej Karpathy — LLM Wiki Gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
- [Obsidian](https://obsidian.md)
- 일부 자료는 외부 영상 · 블로그 · 타 GitHub 저장소를 참고했으며, 각 폴더 README에 구체적인 출처를 명시했습니다.

---

## 📝 Notes

- 이 저장소는 **개인 학습 기록**이며, Anthropic의 공식 가이드가 아닙니다.
- Claude Code 기능은 빠르게 업데이트되므로, 최신 정보는 [공식 문서](https://docs.claude.com)를 우선 참조하시기 바랍니다.
- 오류나 개선 제안은 Issues로 자유롭게 남겨주세요.
