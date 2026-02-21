---
layout: page
permalink: /apps/nourishus/
---

![NourishUs](/assets/img/nourishus.png){: .left w="100"}  
# NourishUs

> Personalized nutrition and recipe guidance aligned with each phase of the menstrual cycle.

[![View on the App Store](/assets/img/download_black.svg)](https://apps.apple.com/us/app/nourishus-cycle-nutrition/id6739262149)   
---

## The Problem

Most cycle-tracking apps focus on symptom logging and date prediction. 
Very few connect cycle phases to actionable nutrition guidance in a structured way.

Users often rely on fragmented information:
- Blog posts
- Social media
- Generic recipe apps
- Calorie-focused tools

NourishUs was built to provide structured, phase-aware nutritional support without emphasizing calorie tracking or weight loss.

---

## Product Goals

- Provide phase-specific recipe recommendations
- Support multiple dietary preferences
- Maintain strict user privacy
- Keep the experience lightweight and intuitive

---

## Architecture

**UI Layer**
- Built entirely with SwiftUI
- Component-driven view composition
- Environment-based dependency injection

**Pattern**
- MVVM architecture
- Clear separation between view logic and data models
- Observable-driven state updates

**Data**
- Structured recipe model with phase metadata
- Filter engine for dietary preferences
- Local storage design using SwiftData

**Health Integration**
- Apple Health integration for cycle data
- All sensitive data remains on-device

---

## Technical Highlights

- Dynamic filtering across 400+ recipes
- Context-aware recommendations based on cycle phase
- Lightweight HealthKit/SwiftData sync
- Accessibility-first typography and layout
- Optimized list rendering for performance

---

## Engineering Challenges

### State Consistency
Ensuring the UI accurately reflects cycle phase changes without redundant view re-rendering.

### Dynamic Cycle Dial
Swift Charts to create dynamic Cycle Dial UI element.

### Privacy
Designing features around Apple Health without storing sensitive health data remotely.

---

## What I Would Improve Next

- Refactoring DataStorage class to reduce complexity and improve cycle/phase calculation logic
- Increase Instrumentation to find and improve performance bottlenecks
- Increasing automated UI and unit test coverage

---

## Reflection

NourishUs represents my approach to product engineering:

- Clear problem definition 
- Structured architecture 
- Respect for user privacy 
- Thoughtful UI decisions 
- Continuous iteration 