# AFOS Studio Architecture

## Purpose

This document defines the high-level architecture of AFOS Studio.

AFOS Studio is designed as a modular AI filmmaking operating system. Each module handles one stage of the film production workflow.

---

## Core System

AFOS Studio has three main layers:

1. User Interface
2. Production Engine
3. AI Departments

---

## 1. User Interface

The user interface is what the creator sees.

Main screens:

* Dashboard
* Project Workspace
* Story
* Director Vision
* Characters
* Environments
* Camera Journey
* Scene Breakdown
* Shot List
* Storyboard
* Image Generation
* Animation
* Editing
* Sound Design
* Quality Control
* Export

---

## 2. Production Engine

The Production Engine controls the workflow.

Responsibilities:

* Track project status
* Decide the next production stage
* Prevent skipped steps
* Lock approved assets
* Manage continuity
* Store production outputs
* Prepare export packages

---

## 3. AI Departments

AFOS uses specialized AI departments:

* Production Manager AI
* Writer AI
* Director AI
* Cinematographer AI
* Character Designer AI
* Environment Designer AI
* Storyboard AI
* Image Director AI
* Animation Director AI
* Editor AI
* Sound Designer AI
* Quality Control AI

Each department has one responsibility and contributes to the full production pipeline.

---

## Data Flow

Story Input

↓

Story Analysis

↓

Production Plan

↓

Character & Environment Design

↓

Camera Journey

↓

Scene Breakdown

↓

Shot List

↓

Storyboard

↓

Image & Animation

↓

Editing & Sound

↓

Quality Review

↓

Export

---

## Core Rule

AFOS must never behave like a random prompt generator.

Every output must pass through the production pipeline and support the final film.
