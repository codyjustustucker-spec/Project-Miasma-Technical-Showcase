# Project Miasma: Prelude

### Independently designed, developed, and released sci-fi survival horror game

**Project Miasma: Prelude** is a first-person sci-fi survival horror game built independently in Unity and C#.

The currently released Steam demo is a complete ~30-minute vertical slice containing the major systems, progression, enemies, environments, narrative, UI, persistence, and release infrastructure of the larger project.

[▶ Play the free demo on Steam](PASTE_STEAM_LINK_HERE)

---

## Project Overview

I built Project Miasma independently from concept through public Steam release.

My work included:

- Software architecture
- Gameplay programming
- Enemy AI
- Level design and implementation
- Power and oxygen systems
- Doors and environmental interactions
- Navigation systems
- UI
- Save/load and persistent state
- Progression and sequencing
- Narrative implementation
- Art and asset integration
- Audio and atmosphere integration
- Debugging and testing
- Build preparation
- Steam deployment and release

The project demonstrates my ability to take a complicated idea through:

**Concept → Architecture → Implementation → Integration → Debugging → Released Product**

---

# Technical Architecture

Project Miasma is built around modular systems rather than tightly coupled one-off scripts.

Major architectural areas include:

### Enemy AI

Enemy behavior is separated into focused responsibilities such as:

- Sensors
- Movement systems
- Actions
- Behavior/planning logic
- World registries
- Shared coordination
- Targeting
- Claims and ownership
- Attack windows
- Failure handling
- Debug visibility

The goal is to allow enemies to share infrastructure while preserving enemy-specific behavior.

The architecture includes explicit results for actions such as:

- Approved
- Denied
- Delayed
- Downgraded
- Cancelled
- Fail-safe

This makes behavior easier to debug, tune, and reason about.

---

### Persistent State & Save Systems

The game distinguishes between:

- Static design data
- Durable runtime state
- Temporary enemy state
- Temporary coordination state
- Shared world state

Persistent systems are reconstructed after loading rather than blindly serializing every runtime object.

Stable IDs and explicit ownership rules are used to keep state consistent across scenes and save/load cycles.

---

### Ship Systems

The game contains interconnected ship infrastructure including:

- Electrical power
- Oxygen
- Lighting
- Navigation
- Doors
- Environmental hazards
- Player progression

Systems affect each other rather than operating as isolated mechanics.

The intent is to make the ship itself behave like a coherent environment.

---

### Gameplay & Progression

The demo includes a complete playable progression path rather than a collection of disconnected mechanics.

The player:

- explores abandoned spacecraft
- restores and manages systems
- navigates environmental obstacles
- discovers narrative information
- encounters multiple enemy behaviors
- progresses through structured objectives
- reaches a defined demo conclusion

---

# Engineering Approach

My development style focuses heavily on:

- Modular architecture
- Clear component ownership
- State management
- Reusable systems
- Explicit inputs and outputs
- Validation
- Failure states
- Debug observability
- Acceptance testing
- Incremental refactoring

I use modern AI tools extensively as an engineering accelerator for implementation, investigation, debugging, refactoring, and documentation while retaining responsibility for architecture, requirements, integration, validation, and product decisions.

---

# Technical Stack

- **Engine:** Unity
- **Primary language:** C#
- **Platform:** Windows / Steam
- **Version control:** Git / GitHub
- **Development:** Visual Studio
- **Additional tools:** Blender, Photoshop/GIMP, AI-assisted development tools

---

# What This Project Demonstrates

Project Miasma is intentionally modest in content length, but it contains the essential layers of a complete software product.

It demonstrates:

- End-to-end product ownership
- Systems architecture
- Complex state management
- AI and behavior systems
- Cross-system integration
- Debugging and failure handling
- Rapid technical learning
- Independent project execution
- Shipping software through a commercial distribution platform

---

# Screenshots

_Add several strong gameplay screenshots here._

Example:

```html
<img src="images/gameplay-01.jpg" width="800">
