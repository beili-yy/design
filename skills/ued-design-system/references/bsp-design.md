---
name: ued-design-system
description: Use the UED design system when creating, modifying, reviewing, or handing off Figma designs. Apply existing design rules, Variables, Components, Variants, Auto Layout, page patterns, states, responsive rules, naming, and assets before creating new design decisions.
---

# UED Design System

## Purpose

Use the existing UED design specification as the source of truth for interface design.

The goal is to ensure that design work is consistent, reusable, structured, and suitable for direct implementation by frontend agents.

## Reference

Before performing related design work, read:

`references/design.md`

Use the relevant sections instead of assuming or inventing design rules.

## When to use this skill

Use this skill when:

- creating a new Figma page
- modifying an existing Figma page
- selecting or creating UI components
- using colors, typography, spacing, radius, icons, or layout rules
- defining component states or Variants
- designing responsive layouts
- reviewing Figma designs
- checking whether a design is ready for frontend implementation
- deciding whether a new design-system rule or component is required

## Workflow

### 1. Check the existing design system first

Before creating any design solution, check whether the design specification already defines:

- Variables
- Colors
- Typography
- Spacing
- Radius
- Grid
- Icons
- Components
- Variants
- Auto Layout rules
- Page patterns
- States
- Responsive rules
- Naming conventions

### 2. Reuse before creating

If an existing rule or component can satisfy the requirement:

- use it
- do not recreate it
- do not create a visually similar duplicate
- do not detach an existing component without a clear reason

### 3. Do not invent design rules

Do not arbitrarily create:

- new colors
- new font sizes
- new spacing values
- new radius values
- new component styles
- new interaction patterns

unless the current design system cannot support the requirement.

### 4. Handle missing rules

If the design system cannot satisfy a requirement, do not silently invent a permanent rule.

Output a:

`Design System Proposal`

The proposal must include:

- what is missing
- why the current design system cannot satisfy the requirement
- proposed rule or component
- usage scenario
- expected reuse value
- affected pages or components

The proposal must be reviewed before becoming part of the official design system.

## Figma requirements

When applying this design system in Figma:

- prefer existing Variables
- prefer existing Components
- use Variants for meaningful component states
- use Auto Layout to express real layout relationships
- preserve semantic layer and component naming
- represent required page and component states
- document necessary interactions
- define responsive behavior where applicable

## Review checklist

Before considering a design complete, check:

- Does it follow the current design system?
- Are existing components reused?
- Are Variables used where available?
- Are component states represented correctly?
- Is Auto Layout used appropriately?
- Are page states complete?
- Are names semantic and understandable?
- Are responsive rules clear?
- Would a frontend agent understand the design without guessing?

## Stop and ask for confirmation when

Stop and raise the issue when:

- product requirements conflict with the design system
- the design specification contains contradictory rules
- no existing component or rule can satisfy the requirement
- a new global design rule is required
- the correct design behavior cannot be determined from available information
