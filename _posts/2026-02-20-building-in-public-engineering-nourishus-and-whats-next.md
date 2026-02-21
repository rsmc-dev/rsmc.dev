---
title: "Building in Public: Engineering NourishUs and What's Next"
date: 2026-02-20
categories: [meta]
tags: [swiftui, architecture, ios, swiftdata]
---

This site serves two purposes:

1. To document how I design and build iOS applications.
2. To deepen my understanding of Apple frameworks through writing.

My current focus is improving and expanding **NourishUs**, a cycle-phase-based nutrition app available on the App Store. Along the way, I plan to publish technical deep dives into the architectural and engineering decisions behind it.

---

## Why Write About It?

Writing forces clarity.

Shipping an app demonstrates execution.  
Explaining its architecture demonstrates understanding.

Over the next several months, I’ll be breaking down real implementation details from NourishUs — not hypothetical examples, but production decisions.

---

## Technical Areas I’ll Be Exploring

Here are a few of the engineering topics I plan to write about:

### 1. SwiftUI State Management in a Production App

NourishUs relies heavily on `Observable` and environment-driven dependency injection.

Some upcoming topics:
- Avoiding redundant re-renders
- Managing derived state cleanly
- Structuring view models for scalability

---

### 2. SwiftData for Local Data Storage

Our customers do not want their private health data in the cloud. We use SwiftData to keep it on device

I’ll be outlining:
- Data modeling strategies
- SwiftData in MVVM architecture
- Keeping UI responsive during recomputation

---

### 3. HealthKit Integration with Privacy in Mind

NourishUs integrates with Apple Health to read cycle data.

Future posts will explore:
- Requesting and managing permissions
- Sync timing considerations
- Designing features around on-device privacy

### 4. Local Notifications for App Engagement

Local notifications are an easy way to encourage app engagement. We use them to remind our customers of upcoming cycle phase change is a good time to review recommended recipes.

I'll be showing:
- Requesting and handling permissions
- Setup and schedule notifications
- Handling fired notification interactions

### 5. Build UI Element with Swift Charts, Path, and View Composition

The main UI element in the cycle tracking feature is built with Swift Charts and Path to dynamically represent the phase and days in the cycle.

I'll be showing:
- Charts SectorMark to layout phases of cycle
- Path to layout series of Circles to layout days of cycle
- Use of composition to build complex UI from smaller, task specific components

---

## What’s Next

In the near future, I plan to:

- Refactor DataStorage class to improve cycle calculation
- Improve performance with Instruments
- Expand automated UI and unit testing
- Publish one in-depth technical article every 2–3 weeks

This site will serve as both documentation and reflection as the app evolves.

If you’re interested in thoughtful iOS architecture, SwiftUI behavior, and real-world engineering tradeoffs, follow along.

*last updated: Feb 20, 2026*
