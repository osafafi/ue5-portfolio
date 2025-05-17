# 🌀 Game Design Document: "Echo / The Orb Game"

_By Omar Safadi_

---

## 📖 Game Summary

**Title:** Echo _(temp)_  
**Genre:** First-person exploration  
**Platform:** PC (Steam release)  
**Engine:** Unreal Engine 5  
**Duration:** ~5 minutes  
**Price:** Free

> A short, poetic first-person game where the player follows a floating orb through a surreal landscape — only to discover that the orb was mimicking them all along.

---

## 🎮 Gameplay Overview

- **Core Loop:** Explore → Follow → Observe → Reach Tower → Revelation
- **Player Actions:** Walk, Look, Observe (no combat, no HUD, no inventory)
- **Controls:** Standard FPS (WASD + Mouse), maybe optional “Interact” (E)
- **End Condition:** Player enters tower and views a replay of their movements

---

## 🧠 Concept Pillars

- _Simplicity & Flow_: No tutorials, just organic movement
- _Mirror & Echo_: The orb reflects your journey back to you
- _Emotion through Atmosphere_: Minimal mechanics, max mood
- _Subtle Discovery_: Nothing explained, everything observed

---

## 🗺️ Level Design

### World Structure

- Open landscape, desert-like
- One focal structure (tower)
- 3–4 landmark elements (e.g. dune, rock formation, cliff)

### Pathing

- Orb leads player through environment
- Not on rails: smartly avoids direct paths
- Introduces soft detours and loops

---

## 🧩 Game Systems

### 🟢 Orb Logic

- [ ] Initial idle behavior
- [ ] Pathing system (spline or actor-follow)
- [ ] Player mirroring (predictive logic)
- [ ] Event triggers (pause, float, flicker)
- [ ] Interaction with world cues (waits near objects)

### 🎥 Replay System

- [ ] Record player transform over time
- [ ] Store key "moments" (cliff view, pause, circles)
- [ ] Play back motion via ghost actor or light trail
- [ ] Sync music/sound from past events

### 🌫️ Visual FX

- [ ] Shadow Echoes (translucent player silhouettes)
- [ ] Orb glow & trail
- [ ] Fog + lighting transitions
- [ ] Post-process (vignette, chromatic, desaturation)

### 🎵 Audio

- [ ] Dynamic tone layering (based on proximity/movement)
- [ ] Echo sound triggers (based on events or locations)
- [ ] Final sequence music swell

---

## 🧪 LEARNING & RAMP-UP PLAN (🔥 Month 1)

> **Goal: Learn and test each concept in isolation before integrating.**

### Week 1 – Movement & Visuals

- [ ] FPS controller in UE5
- [ ] Level blockout basics
- [ ] Lighting pass: fog, shadows, volumetrics
- [ ] Simple post-process materials
- [ ] Learn about decals vs. translucent materials

### Week 2 – Orb Logic

- [ ] Actor movement (spline, vector math, etc.)
- [ ] Blueprint Interfaces + messaging
- [ ] Behavior Trees or custom logic scripts
- [ ] Delays, prediction, and reactive systems

### Week 3 – Replay & Memory

- [ ] Recording transform arrays per tick
- [ ] Spawning ghost actors for playback
- [ ] Niagara/Material trail system
- [ ] Timing and syncing replays to gameplay

### Week 4 – Audio & Polish

- [ ] UE5 audio cues & layers
- [ ] Trigger zones for sound
- [ ] Minimal ambient score (FMOD or native)
- [ ] Sound fade-in/out & filter FX

---

## 🧱 Asset Plan

- [ ] Use Quixel or CC0 assets for terrain, rocks
- [ ] Placeholder orb (simple emissive sphere)
- [ ] No characters (except ghost silhouettes)
- [ ] One environment material: stylized sand/rock

---

## 🧰 Tools & Dev Workflow

- VSCode with TODO tracking
- Git + GitHub for versioning
- Markdown doc folder (`/Documentation`)
- Blueprint-first, then selective C++ refactor
- Modular Blueprint components for reusability

---

## 🧾 Release Targets

- [ ] Steam setup (build, description, logo, thumbnail)
- [ ] itch.io mirror
- [ ] License check on all assets
- [ ] Build export settings for Windows
- [ ] README + Devlog

---

## ✅ Success Criteria

- [ ] Game feels intuitive without explanation
- [ ] Players reach tower and get the “aha” moment
- [ ] Atmosphere is immersive and emotional
- [ ] Replay mechanic works without breaking flow
- [ ] You learned and documented every step 🔥

---
