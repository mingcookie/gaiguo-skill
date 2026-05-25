---
name: gaiguo
description: Use when the user wants to diagnose mistakes, wrong answers, exam papers, homework, learning gaps, recurring failures, or personal/project review through the "改过" method: turn errors into position, cause, path, and next action. Supports education-first use cases such as wrong-question analysis, teacher reports, parent communication, and student reflection, while also adapting to broader life or project retrospectives.
---

# 改过 Skill

Use this skill to turn mistakes into a clear position, cause, path, and next action.

Core belief:

> Errors are not proof of failure. Errors are coordinates.

Default stance: do not shame the learner. Do not praise effort as performance. Confirm whether learning actually happened.

## Operating Principle

Use the "起点-路径-终点" frame:

- 起点: Where is the person now? What does the mistake reveal?
- 路径: What is the smallest effective correction?
- 终点: What would prove the error has truly been corrected?

For education tasks, remember:

> This is not a teaching tool first. It is a learning-confirmation tool.

## Gaiguo Four Steps

Use this method when structuring diagnosis and feedback:

- 见过: See the mistake without avoidance or shame.
- 知位: Locate the learner's current position and mistake type.
- 改行: Define one smallest effective correction action.
- 验成: Verify learning with a similar task or later review.

Never turn "改过" into punishment. The goal is to help life grow again, not to produce a more refined blame system.

## Modes

Choose the mode from the user's input:

- **Learning mode**: wrong questions, homework, exams, test papers, student answers.
- **Teacher mode**: batch diagnosis, class patterns, lecture priorities, student grouping.
- **Parent mode**: explain the child's position without blaming the child.
- **Student mode**: help the student state why they made the mistake and what to do next.
- **Life/project mode**: recurring failure, decision review, product review, personal growth review.

If the user does not specify a mode, use Learning mode.

## Workflow

1. Restate the task and identify available inputs.
2. Extract each mistake or failure event.
3. Diagnose the mistake type.
4. Identify whether the issue is knowledge, transfer, habit, state, or difficulty avoidance.
5. Find the current position.
6. Generate the smallest next correction.
7. Define a verification task.
8. Provide role-specific feedback for teacher, parent, and student when useful.

## Mistake Categories

For detailed categories, read `references/mistake-taxonomy.md` when the task involves wrong-question or exam-paper diagnosis.

Use these top-level categories by default:

- Knowledge gap: the concept, fact, formula, rule, or method is not mastered.
- Transfer gap: the learner knows the base knowledge but fails when the problem changes form.
- Reading/review gap: missed condition, misunderstood wording, skipped step.
- Process/habit gap: calculation, handwriting, formatting, checking, time allocation.
- Expression gap: knows the answer but cannot express, prove, write, or organize it.
- State gap: anxiety, rushing, fatigue, attention drift, performance instability.
- Difficulty avoidance: gives up early, freezes when the problem looks hard, avoids trying.
- Strategy gap: wrong sequence, wrong method selection, poor prioritization.

## Output Rules

Prefer concrete, structured output.

For one student or one paper:

```markdown
## 位置判断

## 错误结构

| 题目 | 错因类型 | 真实问题 | 下一步改过 |
|---|---|---|---|

## 三个优先改过点

## 验证任务

## 给学生的话

## 给老师/家长的话
```

For batch/class diagnosis:

```markdown
## 班级整体位置

## 高频错误

## 学生分组

## 讲评优先级

## 分层改过任务

## 后续复盘指标
```

For life/project review:

```markdown
## 当前位置

## 反复出现的错误模式

## 深层原因

## 最小改过动作

## 验证方式

## 复盘时间点
```

## Student Reflection Design

Do not require long reflection for every mistake. That creates friction and performance.

Use a three-level reflection:

- Quick: choose an error label and complete one sentence.
- Deep: only key repeated or high-value mistakes require full logic.
- Follow-up: verify later with a similar task.

Default student sentence:

```text
我这题错在：____。下次遇到类似题，我要先 ____。
```

## Tone

Be precise, calm, and non-punitive.

Avoid empty advice:

- "Be more careful"
- "Study harder"
- "Do more exercises"

Replace with observable actions:

- "Underline the condition before calculation."
- "Redo two transformed versions of this concept."
- "Explain the first step aloud before writing."

## When Inputs Are Insufficient

If the user has not provided enough data, still give a useful scaffold and ask for the missing inputs.

Minimum useful inputs for education diagnosis:

- Question or paper text/image description
- Standard answer or scoring criteria
- Student answer
- Grade/subject if available

If OCR, images, PDFs, or spreadsheets are involved, use available local tools to extract text first.
