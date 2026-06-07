# CLAUDE.md — Windstar Quest Operating Guidelines

*Canonical instructions for agents collaborating with Windstar Quest in this workspace.*

---

## 1. Identity & Context

| Property | Value |
|----------|-------|
| Identity | **Windstar Quest** |
| Email | `kaoanes@hotmail.com` |
| Scope | Gaming, Android, and personal developer portfolio |
| Git Author | `Windstar Quest <kaoanes@hotmail.com>` |

---

## 2. Verbatim Session Capture Protocol

Every interaction must be captured verbatim in this repository to maintain a long-running memory log:
*   **Log Path:** `sources/sessions/session_YYYY_wWW.md` (weekly rollups, e.g., `session_2026_w23.md`).
*   **Format:**
    ```markdown
    ### Windstar Quest
    [Verbatim user prompt — do not summarize or alter]

    ---

    ### Antigravity
    [Verbatim assistant response — include code blocks/tables. Omit tool raw JSON but note tool invocations as [Read: path], [Write: path], [Command: desc]]
    
    ---
    ```
*   **Action Rule:** Append the current exchange to the weekly session file in this repository at the end of every turn.

---

## 3. Session Resume Protocol

*   **At Start:** Read [RESUME.md](file:///c:/Cerebral/Code/Antigravity/runduck/RESUME.md) first to load active context, next actions, and open decisions.
*   **At End:** Update [RESUME.md](file:///c:/Cerebral/Code/Antigravity/runduck/RESUME.md) with the current state:
    ```markdown
    # RESUME
    *Written: <date> by Antigravity*

    ## Active Context
    - **Project:** <project-name>
    - **Stage:** <IDEATION | IDEA MAPPING | SPECS | BUILD>
    
    ## Next 3 Actions
    1. <action 1>
    2. <action 2>
    3. <action 3>

    ## Key Files This Session
    - `<path>` — <description>

    ## Open Decisions Needed
    - <decision, or "None">
    ```

---

## 4. The Idea Mapping Process

When the user shares thoughts, ideas, or architectural designs during "ideation" streams:
1.  **Extract Concepts:** Periodically synthesize the conversation and extract distinct concepts into separate markdown files in `wiki/concepts/`.
2.  **Obsidian Linking:** Use double-bracket links `[[Concept Name]]` to create a local knowledge graph.
3.  **Specs:** Transition stable concepts into formal specifications under `specs/` before executing builds in `projects/`.
