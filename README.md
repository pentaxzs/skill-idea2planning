# skill-idea2planning

아이디어를 **1-pager → PRD → ASCII 와이어프레임**으로 변환해주는 Claude Code 스킬.

PM, PD 직군의 주니어부터 시니어까지, 막연한 아이디어로도 바로 시작할 수 있습니다.

---

## 설치 방법

```bash
# 1. 스킬 디렉토리에 클론
git clone https://github.com/pentaxzs/skill-idea2planning ~/.claude/skills/idea2planning
```

끝. Claude Code를 재시작하면 `/idea2planning`으로 바로 사용 가능합니다.

---

## 사용 방법

Claude Code에서 입력:

```
/idea2planning
```

아래 메뉴가 나타납니다:

```
무엇을 만들어볼까요?

1) 1-pager     — "이 제품이 왜 필요한가"를 한 장으로 정리한 요약 문서
2) PRD         — "무엇을 어떻게 만들어야 하는가"를 정리한 요구사항 문서
3) 와이어프레임 — 텍스트로 그리는 화면 구조 스케치
4) 처음부터 차근차근 (1→2→3 순서로)
5) 잘 모르겠어요, 아이디어부터 설명할게요
```

---

## 참조 파일 추가 방법

예시 파일을 추가하면 자동으로 품질 기준에 반영됩니다. SKILL.md 수정 불필요.

```bash
# PRD 예시 추가
cp your-prd.md ~/.claude/skills/idea2planning/references/prd_example04.md

# 1-pager 예시 추가
cp your-1pager.md ~/.claude/skills/idea2planning/references/1pager_example04.md
```

### 파일 명명 규칙

| 파일명 패턴 | 용도 |
|---|---|
| `1pager_example*.md` | 1-pager 예시 (품질 기준) |
| `1pager_template.md` | 1-pager 구조 템플릿 |
| `1pager_understanding.md` | 1-pager 작성 원칙 |
| `prd_example*.md` | PRD 예시 (품질 기준) |
| `prd_template.md` | PRD 구조 템플릿 |
| `prd_understanding.md` | PRD 작성 원칙 |
| `wireframe_example*.md` | 와이어프레임 예시 |
| `wireframe_template.md` | 와이어프레임 구조 템플릿 |
| `wireframe_understanding.md` | 와이어프레임 작성 원칙 |

---

## 디렉토리 구조

```
~/.claude/skills/idea2planning/
  SKILL.md
  references/
    1pager_example01.md
    1pager_example02.md
    1pager_example03.md
    1pager_template.md
    1pager_understanding.md
    prd_example01.md
    prd_example02.md
    prd_example03.md
    prd_template.md
    prd_understanding.md
    wireframe_template.md
    wireframe_understanding.md
```

---

## 기여 방법

좋은 예시 문서가 있다면 PR로 공유해주세요.
`references/` 폴더에 파일을 추가하는 것만으로 기여할 수 있습니다.
