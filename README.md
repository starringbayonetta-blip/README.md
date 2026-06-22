# README.md### 💀 Skull Groove: AI Video Physics & Guardrail Translation Engine

> **Status:** Architecture Spec & Logic Blueprint v2.0 (Seeking Contributors)  
> **Target Focus:** Local Geometric Pixel Force-Scaling & Automated Safe-Token Wrappers for AI Diffusion Video Pipelines.

* * *

### 💡 The Core Problem We Are Solving

Mainstream AI video generators (HunyuanVideo, LTX-Video, CogVideoX) suffer from severe mathematical and semantic drift during complex human size-shifting or physical transformation sequences.

1.  **Volumetric Ballooning:** Models expand a mesh's surface area equally in all directions rather than extending skeletal length, turning characters into soft inflation shapes.
2.  **Foot Slippage / Float Drift:** Characters lose traction and slide across floor planes or float off furniture because models choose "cheap camera tilt-up shots" over real physics.
3.  **Aggressive Lexical Cloud Filtering:** Rigid keyword blacklists block crucial artistic terms like *ripping*, *tearing*, or *tight*, paralyzing creative freedom for independent animators and Hollywood studios alike.

**Skull Groove** acts as an open-source standalone desktop middleware application that solves these visual failures by decoupling creative user text scripts from the target AI engines.

* * *

### ⚙️ Core Architecture & System Logic

    [User Long Script] ➔ [1. Automated Beat Slicer] ➔ [2. Local SAM 2 Masking] ➔ [3. Hidden Token Sanitizer] ➔ [AI Engine]
    

### Module 1: The Automated Script Segmenter

To prevent semantic drift, Skull Groove allows directors to write unrestricted narratives. The backend code automatically slices long text entries into high-density **120-word micro-beats** connected sequentially via video-to-video seed locks.

### Module 2: Local Geometry & Posture Anchor Engine

Integrates *Segment Anything Model 2 (SAM 2)* to cut the character out locally. It maps an immutable coordinate overlay based on user-selected postures:

*   `STANDING`: Locks absolute coordinates to the **soles of the feet** to ensure flatly planted stances.
*   `SITTING`: Locks coordinates to the **pelvis baseline**, pre-calculating and forcing a downward pixel displacement (e.g., mattress compression) on background objects before sending frames to the AI layer.
*   `FETAL_LYING`: Locks the layout horizontally, forcing the contact side heavily against the floor plane.

### Module 3: Prompt Token Sanitizer & Guardrail Evasion

Runs a real-time regex filter that intercepts flagged terms and replaces them with safe, highly clinical, structure-focused engineering vocabulary to slide cleanly under cloud safety guardrails:

*   `growth / growing` ➔ `skeletal scaling & proportional volumetric expansion`
*   `ripping / tearing` ➔ `fabric mechanical failure at tensile threshold`
*   `tight` ➔ `material deforms under structural load`

* * *

### 🛠️ Repository File Inventory

*   `/ui-mockup/` : Containments for the 1440x900 Desktop Figma Layout Tree.
*   `/core/sanitizer.py` : Python class module managing regex dictionary switches and the 120-word chunker engine.
*   `/schema/character_profile.json` : JSON validation schema for identity locks, high-contrast lighting parameters, and wardrobe materials to mitigate training data representation bias.

### 🤝 Contributing

Contributions are completely open. If you have experience in Python pipeline engineering, ComfyUI visual node maps, or custom machine learning masking models, look over our open modules and submit a pull request. Let's give creators their creative freedom back.
