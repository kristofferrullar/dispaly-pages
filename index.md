# Email Sending Workflow & List Management  
*(Main Use Case – Promotional / List-Based Sending)*

---

## Introduction

This document defines a **safe, disciplined way to send emails** when working with contact lists of mixed quality.

It was created after earlier problems with:
- sending too much volume too fast
- low engagement harming deliverability
- accounts being paused to protect infrastructure

The purpose of this guide is to:
- prevent those problems from repeating
- reduce guesswork and stress
- protect sending reputation
- ensure emails are only sent to people who show interest

This is **not** a growth hack or copywriting guide.  
It is a **process guide** for daily execution.

You do not need to understand email infrastructure to follow this document.  
You only need to observe behavior and follow the steps.

---

## The Core Rule

**People earn more emails by showing interest.  
People lose emails by staying silent.  
People who say no are respected immediately.**

Everything below enforces this rule.

---

## High-Level Workflow Overview

Each cycle follows the same structure:

1. Take a small segment of contacts  
2. Send one appropriate email  
3. Observe behavior  
4. Decide next action based on behavior  
5. Clean the list  
6. Repeat with discipline  

---

## Integrated Workflow Flowchart

```mermaid
flowchart TD
    A[Start day / Select small contact segment] --> B[Send first calm, neutral email]

    B --> C{Any reaction?}

    C -->|Opened / Clicked / Replied| D[Interest detected]
    C -->|No reaction| E[Uncertain interest]
    C -->|Unsubscribe / Complaint / Bounce| F[Remove immediately]

    D --> G{Strength of engagement?}
    G -->|Strong replies / clicks| H[Sales email allowed<br/>Clear but respectful]
    G -->|Light opens only| I[Soft sale or recommendation<br/>No hype]

    E --> J[Send softer follow-up<br/>Check-in tone]

    J --> K{Reaction now?}
    K -->|Opened / Replied| L[Medium interest]
    K -->|No reaction again| M[Last-call / preference check]
    K -->|Unsubscribe / Complaint| F

    L --> I

    M --> N{Explicit yes?}
    N -->|Yes| I
    N -->|No response or No| O[Stop sending / Suppress]

    H --> P[Continue paced sending]
    I --> Q[Continue low-pressure content]
    O --> R[End for this contact]
    F --> R
