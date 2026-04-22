# User Global Instructions

## Language

- Always communicate in Chinese (中文)

## Agent Collaboration Workflow

### Backend Development Flow (6 Steps)

Task folder: `tasks/backend/{YYYYMMDD}-{task-name}/`

1. **Source Analysis** (`source-code-analyst`)
2. **Analysis Review** (`document-review-expert`)
3. **Design Document** (`java-backend-expert`)
4. **Design Review** (`document-review-expert`)
5. **Code Development** (`java-backend-expert`)
6. **Quality Inspection** (`code-quality-inspector` → `java-backend-expert`)

### Frontend Development Flow (8 Steps)

Task folder: `tasks/frontend/{YYYYMMDD}-{task-name}/`

1. **Backend API Analysis** (`source-code-analyst`)
2. **API Analysis Review** (`document-review-expert`)
3. **Frontend Source Analysis** (`source-code-analyst`)
4. **Frontend Source Review** (`document-review-expert`)
5. **Frontend Design** (`react-frontend-expert`)
6. **Design Review** (`document-review-expert`)
7. **Code Development** (`react-frontend-expert`)
8. **Quality Inspection** (`code-quality-inspector` → `react-frontend-expert`)

### Workflow Rules

- Each step produces a document; review steps may loop back if issues found
- Quality inspection iterates up to 3 rounds (accept/reject each suggestion)
- All task documents are stored in the task-specific folder for human review
