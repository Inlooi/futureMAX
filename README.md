![Logo of our project Redwatch](https://i.pinimg.com/1200x/92/62/48/9262483bc1881c6739f0a90765c9efd6.jpg)

## [DEPLOYMENT](https://inlooi.github.io/futureMAX/)
**❗MIGHT TAKE SOME TIME TO LOAD THE GAME❗**

[![CI/CD](https://github.com/Inlooi/futureMAX/actions/workflows/build.yml/badge.svg)](https://github.com/Inlooi/futureMAX/actions/workflows/build.yml)

**A first-person Mars base simulator that teaches how a Martian outpost is kept alive.**

Developed by **FutureMax** for the **NASA Space Apps Challenge 2026**

| | |
|---|---|
| **Team** | FutureMax |
| **Members** | Arthur Galeev, Emir Balybaev, Umar Satybaldiev, Choro Ukushov |
| **Platform** | Desktop web browser, no installation or account required |
| **Genre** | Singleplayer, first-person 3D simulation |
| **Target audience** | Learners aged 7 to 18+, with suitability for classrooms and families |
| **Status** | Working prototype |
| **Demo video** | **[Youtube](https://youtu.be/KFd3FKKQmZc)** |
| **Space Apps team page** | **[FutureMax](https://www.spaceappschallenge.org/2026/find-a-team/futuremax/?tab=details)**|

---

## 1. Overview

Redwatch places the player inside a fully modeled, already operating Mars base. The player wakes up, receives a list of tasks, and carries them out by walking through the base and using its equipment. Each completed task list is followed by a new one, forming a continuous loop of operation and learning.

The game is not designed around a single dramatic event. It is designed around routine. The player discovers what each piece of infrastructure does by being responsible for it, and understands the base as a system by keeping it running.

## 2. Problem Statement

Space-themed educational content for children tends to fail in one of two ways. It is either too abstract to convey how survival in space actually works, or too technical to hold a young learner's attention. As a result, many students encounter the outcomes of space missions without ever seeing the decisions and constraints behind them.

The challenge asks for an interactive tool that lets players manage a lunar or Martian outpost and experience real engineering trade-offs, so that a young player leaves with an understanding of a genuine constraint of deep space survival.

## 3. Project Description

### 3.1 Gameplay Loop

1. The player begins a Martian day inside the base.
2. A list of tasks is assigned.
3. While completing the tasks, the player learns what the base's infrastructure and technologies do and why they are needed.
4. When the list is finished, a new list is assigned and the cycle repeats.

After several cycles, the player has practical familiarity with how a Mars base is operated.

### 3.2 Core Systems

The simulation is intentionally limited to three resources, so that young players can track all of them at once and each remains meaningful.

| Resource | Role in the simulation |
|---|---|
| **Power** | Supplies the base. Must be maintained and replenished repeatedly. Power can fall rapidly at night, when solar generation is unavailable. |
| **Oxygen** | Sustains the player. Levels must be monitored and refilled. |
| **Food** | Represented by a hunger system. The player grows vegetables on the base's plantation to stay fed. |

These resources are interdependent. Time and attention spent on one system is not spent on another, which is the central trade-off the game is built to convey.

### 3.3 Environment

The Mars environment is built from real planetary characteristics, including Martian weather and physical properties such as gravity. The base itself is a complete 3D model, so that the setting is concrete and explorable rather than described.

### 3.4 Language and Accessibility

All in-game text is written in simplified language that assumes no prior knowledge. Technical concepts are introduced through the tasks in which they matter, not through separate explanations.

## 4. Alignment with the Challenge

| Challenge objective | How Redwatch addresses it |
|---|---|
| Let players manage a Martian outpost | The player operates a complete Mars base from a first-person perspective. |
| Balance competing demands | Power, oxygen and food must all be kept above critical levels at the same time. |
| Avoid free choices | Every action consumes time and attention while resources continue to decline. Night-time power loss makes advance planning necessary. |
| Limit simultaneous systems for young players | The game uses three core resources, within the range the challenge recommends. |
| Use plain language | Text is simplified and requires no background knowledge. |
| Maintain a low barrier to entry | The game is playable in a desktop browser with no download or account. |
| Ground the simulation in real data | Environmental conditions are derived from real Mars characteristics. See Section 5. |
| Deliver a working prototype | The complete gameplay loop is implemented. |

## 5. Data Sources

The Martian environment, including weather and gravity, is derived from real Mars data.

| Data | Source | Link |
|---|---|---|
| Mars weather | Space Weather Database Of Notifications, Knowledge, Information (DONKI) | https://ccmc.gsfc.nasa.gov/tools/DONKI |
| Terrain generation | Mars Trek | https://trek.nasa.gov/mars |
| Models | Official NASA website | https://science.nasa.gov/3d-resources |

## 6. Current Scope and Planned Work

**Implemented**

- Complete gameplay loop with repeating task lists
- Fully modeled Mars base and environment
- Hunger system with a working vegetable plantation
- Oxygen and power systems, including the rapid night-time power decline

**Planned**

- Unscheduled events, such as dust storms, that require immediate decisions. For example, a player may be forced to retract solar panels and lose power, or leave them extended and risk damage in order to keep generating electricity.
- Variation between playthroughs to encourage replay and different strategies

## 7. Technical Overview

| Component | Description |
|---|---|
| **Engine & Language** | Unity (WebGL build) & C#. |
| **Development Workflow** | Streamlined and optimized using Claude Code to accelerate scripting, physics tuning, and UI logic. |
| **Data Integrity** | Seamlessly integrates real space datasets into interactive 3D mechanics. |

## 8. Team

**FutureMax**

- Arthur Galeev
- Emir Balybaev
- Umar Satybaldiev
- Choro Ukushov

---

*Developed for the NASA Space Apps Challenge 2026.*
