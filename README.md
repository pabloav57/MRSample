# 🕶️ MRSample

Este proxecto foi creado empregando a plantilla **Mixed Reality (MR) Core** en Unity. Serve como base para o desenvolvemento de experiencias de realidade mixta (MR).

## 📁 Estrutura da escena - `SampleScene`

A escena inclúe os seguintes GameObjects e compoñentes principais:

### 🌍 Environment
- Contén elementos do entorno e iluminación (`Directional Light`).

### 🎮 MR Interaction Setup Variant
- `Input Action Manager`: Xestiona as accións de entrada para XR.
- `XR Interaction Manager`: Coordina interaccións entre obxectos interactivos e dispositivos de entrada.
- `EventSystem`: Sistema necesario para interactuar con UI en XR.

### 🧍 XR Origin (XR Rig)
- Estrutura principal que representa ao usuario.
- `Camera Offset`: Permite axustar a posición da cámara respecto ao chan.
- `Locomotion`: Engade movemento (teletransporte, camiñar, etc.).
- `Hands Smoothing Post Processor`: Suaviza o movemento das mans.
- `AR Session`: Controla a sesión de realidade aumentada (pode desactivarse para simulación en PC).
- `Goal Manager` / `Object Spawner`: Usados para mostrar obxectos ou completar obxectivos.

### 🧩 UI
- `Coaching UI`: Interface de axuda e guía.
- `Hand Menu Setup MR Template Variant`: Menú que aparece vinculado ás mans.
  - `Left/Right Hand Tracked Anchor`: Define onde se coloca o menú en cada man.
  - `Follow GameObject`: Fai que o menú siga ao usuario.
- `Permissions Manager`: Controla os permisos necesarios (cámara, micrófono, etc.).