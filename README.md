# Dylan's Agent Skills

A collection of high-quality, reusable **Skills** (agent capabilities) designed for AI coding agents such as **Claude Code**, **Gemini**, **Cursor**, and **Windsurf**. These skills equip your AI assistants with specialized workflows for product design, Apple development infra, and aesthetic translations.

This repository is fully compatible with **[skills.sh](https://skills.sh)**, the package manager and registry for AI agent behaviors.

---

## 🚀 Quick Start (Installation)

You can easily install these skills directly from GitHub into your project or globally using `skills.sh`.

### 1. Install All Skills in this Repo
To install all available skills in this repository to your current project:
```bash
npx skills add enzoding/dylan_skills
```

### 2. Install a Specific Skill
If you only need a single capability (e.g., `classic-braun-design`):
```bash
npx skills add enzoding/dylan_skills --skill classic-braun-design
```

### 3. Install Globally
To make a skill available across all your projects, append the `-g` flag:
```bash
npx skills add enzoding/dylan_skills --skill classic-braun-design -g
```

### 4. Updating Skills
To check and pull the latest updates for your installed skills, run:
```bash
npx skills update
```

---

## 🗂️ Skills Directory (Classification)

Here is a categorized list of skills available in this repository:

### 🎨 Design & Aesthetics
*Skills focused on visual polish, art direction, and converting physical or product design philosophies into digital UIs.*

| Skill Name | Trigger / When to Use | Description |
| :--- | :--- | :--- |
| **[classic-braun-design](./classic-braun-design)** | When asking for Braun, Dieter Rams style, retro calculator/clock UIs | Translate the classic physical product language of Braun into responsive digital UIs. |
| **[less-but-better-design](./less-but-better-design)** | General minimalism, restraint, good taste audit requests | A broader guide to clean, functional, and durable product design aesthetics. |
| **[object-to-design](./object-to-design)** | Translating any physical brand (Dyson, Nothing, Apple, Brompton, etc.) into UI | Create AI-ready `DESIGN.md` tokens and layout rules from iconic industrial objects. |

### 🛠️ Tooling & Infrastructure
*Skills that automate complex technical pipelines, environment setup, and development operations.*

| Skill Name | Trigger / When to Use | Description |
| :--- | :--- | :--- |
| **[asc-signing-setup](./asc-signing-setup)** | iOS/macOS bundle IDs, cert rotation, provisioning profiles | Set up secure signing syncing, capabilities, and certificates with the App Store Connect CLI (`asc`). |
