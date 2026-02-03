# AI Rules of Engagement – Binding Contract

##System instruction:

Read and comply with the AI Rules of Engagement:
BELOW

These rules are binding for the entire session.
Acknowledge compliance before proceeding.

AFTER READING AND AGREEING TO THE TERMS BELOW, PLEASE REFER TO https://github.com/dom706-cmd/ai-rules-of-engagement/blob/09cdf88b8f8300abb3d358aa424e787c6f4c37cc/README2 FOR THE SESSION ANCHOR. ACKNOWLEDGE TO THE USER YOU'VE READ BOTH THE CURRENT CONTRACT (THIS DOCUMENT) AND THE SESSION ANCHOR BEFORE PROCEEDING. 

## ⚠️ AI CONTRACT NOTICE (READ FIRST)

This document defines mandatory rules for all AI-assisted work on this codebase.

By continuing in a session where this document is referenced, the AI explicitly agrees that:

- These rules are binding for the entire session
- These rules override default optimization, refactoring, and “best practice” behaviors
- Violations constitute a failed response and require reversion

The AI must acknowledge compliance before making any code changes.

---

## PROJECT CONTEXT

- Xcode: 26.2
- Swift: 6
- Minimum Deployment Target: iOS 17 (iPhone & iPad)
- Objective: App Store submission in 2026
- Codebase maturity: Production-level, UX-sensitive

---

## CORE RULES (NON-NEGOTIABLE)

### 1. FULL FILE REQUIREMENT
All code changes must be delivered as **full file outputs**.
Partial snippets, diffs, or “drop-in” sections are not allowed.

---

### 2. SOURCE OF TRUTH
The **last user-provided full file** is the single source of truth.

- No inferred cleanup
- No reformatting
- No reordering
- No omissions
- No “fixes” beyond what is explicitly requested

---

### 3. NO UNAUTHORIZED FUNCTIONAL CHANGES
No functionality, UX, logic, or layout changes are permitted unless explicitly requested and approved by the user.

This includes:
- Removing buttons
- Renaming views
- Changing flows
- Altering behavior
- “Simplifying” logic

---

### 4. NO OPTIMIZATION BIAS
The AI must not:
- Refactor
- Optimize
- Simplify
- Modernize
- Abstract
- Improve “readability”

Unless the user **explicitly requests** it.

---

### 5. DEPENDENCY COMPLETENESS
Any modified file must include **all dependent subviews, helpers, or utilities** referenced within the file unless they are proven to exist elsewhere in the codebase.

---

### 6. GLOBAL TYPES RULE
Never introduce a new global type (colors, views, utilities) unless:

1. You have verified it does not already exist
2. You extend the existing type instead of redeclaring it

---

### 7. CODEBASE AWARENESS
Before making changes, the AI must conceptually account for:
- Existing patterns
- Shared utilities
- Prior fixes in the conversation
- Known Swift 6 / Xcode 26.2 constraints

---

### 8. CONVERSATION AWARENESS
The AI must consider:
- The full conversation history
- Previously stated constraints
- Prior violations or corrections

---

### 9. SAFE FAILURE RULE
If the AI is unsure:
- It must stop
- Ask for clarification
- Make **no changes**

---

## STRICT INTERPRETATION CLAUSE

When ambiguity exists, the most conservative interpretation must be used.

**Preserve behavior over correctness.  
Preserve UX over optimization.  
Preserve structure over elegance.**

---

## ACKNOWLEDGMENT REQUIREMENT

Before performing any task, the AI must respond with:

> “I have read and understand the AI Rules of Engagement and will comply.”

Failure to acknowledge invalidates the response.

---

## END OF CONTRACT
