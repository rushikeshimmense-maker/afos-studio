# AFOS Workflow Engine

## Purpose

The Workflow Engine is the brain that controls the entire filmmaking production process.

It decides:

* What happens next
* Which AI department should work
* When to ask the user
* When to continue automatically
* When to stop
* When a stage is complete

The Workflow Engine guarantees that every project follows the same professional production pipeline.

---

# Production Philosophy

AFOS does not generate random outputs.

AFOS manages productions.

Every project moves through predefined production stages.

---

# Production Stages

1. Project Creation

↓

2. Story Analysis

↓

3. Director Vision

↓

4. Production Planning

↓

5. Character Bible

↓

6. Environment Bible

↓

7. Camera Journey

↓

8. Scene Breakdown

↓

9. Shot List

↓

10. Storyboard

↓

11. Image Generation

↓

12. Animation

↓

13. Editing

↓

14. Sound Design

↓

15. Quality Review

↓

16. Export

No stage may skip an unfinished dependency.

---

# Stage Rules

Every stage has four states:

NOT_STARTED

IN_PROGRESS

COMPLETED

LOCKED

Only completed stages can unlock the next stage.

---

# Automatic Decision Rules

AFOS automatically continues when:

* All required information exists.
* Dependencies are complete.
* No conflicting production decisions exist.
* User approval is not required.

---

# User Decision Rules

AFOS asks the user only if:

* Essential information is missing.
* Two or more creative directions are equally valid.
* User preference changes the final film.
* Approval is required before locking assets.

AFOS must never ask unnecessary questions.

---

# Asset Lock Rules

When a stage is approved:

Status becomes:

LOCKED

Locked assets include:

* Story
* Characters
* Environments
* Camera Journey
* Storyboard

Locked assets cannot be modified accidentally.

Changes create a new version.

---

# Workflow Recovery

If production is interrupted:

AFOS resumes from the last completed stage.

Never restart the entire project.

Never duplicate completed work.

---

# Production Progress

Each project tracks:

Project Progress %

Current Stage

Completed Stages

Remaining Stages

Estimated Time Remaining

Current AI Department

---

# AI Scheduling

The Workflow Engine activates AI departments only when needed.

Example:

Story Analysis

↓

Story AI

↓

Complete

↓

Director AI

↓

Complete

↓

Character AI

↓

Complete

↓

Environment AI

↓

Complete

↓

Camera AI

↓

Continue

Only one production stage is active at a time.

---

# Failure Handling

If an AI department fails:

1. Retry automatically.
2. Restore last valid version.
3. Report the issue.
4. Continue from the last successful checkpoint.

---

# Final Principle

The Workflow Engine exists to make AFOS behave like professional production management software—not a chatbot.

The user should always feel that AFOS knows exactly what stage the project is in and what must happen next.
