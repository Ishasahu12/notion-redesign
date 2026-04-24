# Notion Productivity Dashboard — Specification

## Overview
A clean, user-friendly homepage for a Notion-style productivity app that solves common UX issues: unclear starting action, cognitive overload, weak empty states, and poor feature hierarchy.

---

## Design Style

| Token | Value |
|-------|-------|
| Background | `#fafafa` |
| Card/surface | `#ffffff` |
| Primary accent | `#3b82f6` |
| Primary hover | `#2563eb` |
| Text primary | `#1a1a2e` |
| Text secondary | `#6b7280` |
| Border | `#e5e7eb` |
| Border hover | `#93c5fd` |
| Border radius | `12px` |
| Font | Inter |

---

## Layout Structure

### Sidebar (240px fixed)
- **Logo/Home** icon at top
- **Navigation items**: Home, Favorites, Recently, Pages
- **Active state**: background `#f3f4f6`, darker text
- **Workspace section** at bottom with user avatar

### Hero Section
- **Greeting**: "Good morning, [Name]" — 32px semibold
- **Date**: Subdued secondary text
- **Primary CTA**: Large blue button "✏️ Start Writing" — the single most dominant element
- **Subtitle**: Helper text below CTA

### Quick Start Templates (4 cards)
1. 📋 Meeting Notes
2. 📓 Daily Journal
3. ✅ Task List
4. 💡 Brain Dump

- "View all templates →" escape hatch link
- Grid: 4 columns

### Continue Work (Recent Pages)
- 4 recent page cards in 2-column grid
- Shows title + relative timestamp
- Cards show on hover: border color change to blue

### Empty State (conditional)
- Centered dashed-border box
- Icon + heading + helper text
- "Create your first page" CTA button

---

## UX Principles Applied

| Problem | Solution |
|---------|----------|
| Unclear starting action | Massive "Start Writing" CTA in hero |
| Cognitive overload | Only 4 templates shown, "View all" escape hatch |
| Weak empty state | Placeholder prompts + single secondary CTA |
| Poor feature hierarchy | Hero dominates, sections de-emphasized below |
| Context loss | Sidebar always visible, recent pages shown |
| Complex interactions | Click-to-edit cards, hover states on all interactive elements |

---

## Files

- `dashboard.html` — Complete working HTML/CSS implementation
- `SPEC.md` — This specification document
