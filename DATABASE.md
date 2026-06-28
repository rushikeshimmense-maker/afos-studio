# AFOS Studio Database Design

## Purpose

The AFOS database stores every production asset from the first idea to the final exported film.

Every project has its own production workspace.

---

# Entity Relationship

Workspace

↓

Projects

↓

Scenes

↓

Shots

↓

Assets

↓

Production Outputs

---

# Projects

Stores overall project information.

Fields

* Project ID
* Project Name
* Description
* Genre
* Runtime
* Visual Style
* Target Platform
* Production Status
* Created Date
* Updated Date

---

# Characters

Stores approved character information.

Fields

* Character ID
* Project ID
* Name
* Role
* Age
* Personality
* Costume
* Appearance
* Expressions
* Character Bible
* Status

---

# Environments

Stores environment data.

Fields

* Environment ID
* Project ID
* Name
* Description
* Lighting
* Weather
* Time of Day
* Environment Bible
* Status

---

# Scenes

Stores every scene.

Fields

* Scene ID
* Project ID
* Scene Number
* Title
* Purpose
* Characters
* Environment
* Emotional Beat
* Duration
* Status

---

# Shots

Stores every cinematic shot.

Fields

* Shot ID
* Scene ID
* Shot Number
* Camera Angle
* Camera Movement
* Lens
* Composition
* Dialogue
* Action
* Sound
* Transition
* Storyboard Status

---

# Storyboards

Stores storyboard assets.

Fields

* Storyboard ID
* Shot ID
* Image
* Director Notes
* Approval Status
* Version

---

# Images

Stores generated production images.

Fields

* Image ID
* Storyboard ID
* Prompt
* Version
* Status
* Generated Date

---

# Animation

Stores generated videos.

Fields

* Animation ID
* Shot ID
* Prompt
* Video
* Duration
* Status

---

# Editing

Stores editing information.

Fields

* Editing ID
* Scene ID
* Transition
* Color Grade
* VFX
* Notes

---

# Sound

Stores sound assets.

Fields

* Sound ID
* Scene ID
* Music
* Foley
* Ambience
* Dialogue
* Mix Status

---

# Quality Review

Stores production review.

Fields

* QA ID
* Project ID
* Stage
* Reviewer
* Issues
* Approval
* Notes

---

# Export

Stores final deliverables.

Fields

* Export ID
* Project ID
* Package Version
* Export Date
* Download URL
* Status

---

# Core Rules

* Every Project owns all production data.
* Every Scene belongs to one Project.
* Every Shot belongs to one Scene.
* Every Storyboard belongs to one Shot.
* Every Image belongs to one Storyboard.
* Every Animation belongs to one Shot.
* Approved assets are locked until intentionally revised.
* All revisions create new versions instead of overwriting previous work.
