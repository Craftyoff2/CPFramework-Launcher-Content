# CPFramework Launcher – Content Repository

Centralized content repository for **CPFramework Launcher**, developed by **Crafty Productions**.

This repository stores the content displayed inside CPFramework Launcher, including news articles, game information, social content and associated media assets.

Content is managed through a custom desktop application and published to GitHub, allowing the launcher to retrieve updated information without requiring a new launcher release.

---

## Overview

The repository acts as the online content source for CPFramework Launcher.

Instead of manually editing files on GitHub, content is managed through a dedicated desktop application developed by Crafty Productions.

The application handles content creation, editing and publishing. Git integration synchronizes the local repository with GitHub, where the launcher can retrieve the published content.

### Main Features

- **News System** – Publish launcher announcements, studio updates and articles.
- **Game Information** – Store information about games developed or published by Crafty Productions.
- **Social Content** – Manage content intended for the launcher's social section.
- **Image Management** – Manage and publish images associated with content.
- **Automatic Publishing** – Synchronize changes from the desktop application to GitHub.
- **Centralized Content** – Keep launcher information organized in one repository.

---

## Repository Structure

Current repository structure:

```text
CPFramework-Launcher-Content/
└── content/
    ├── manifest.json
    ├── news.json
    ├── games.json
    └── social.json
```

### File Descriptions

| File | Description |
|---|---|
| `manifest.json` | Contains repository metadata and the list of content files. |
| `news.json` | Stores news articles and announcements. |
| `games.json` | Stores game-related information. |
| `social.json` | Stores content for the social section. |

Additional media assets, such as article images, can be published and managed through the desktop Content Manager when needed.

---

## News System

The `news.json` file stores the articles displayed in CPFramework Launcher.

Each news article can contain information such as:

| Property | Description |
|---|---|
| `id` | Unique article identifier. |
| `title` | Article title. |
| `slug` | URL-friendly article identifier. |
| `category` | Article category. |
| `excerpt` | Short article description. |
| `content` | Main article content. |
| `featured` | Indicates whether the article is featured. |
| `published` | Determines whether the article is published. |
| `publishedAt` | Publication date and time. |

Articles can be created, edited and published through the custom desktop application.

Images associated with articles can also be managed through the application.

---

## Manifest System

The `manifest.json` file provides metadata about the content repository.

It currently contains:

- `schemaVersion` – Version of the content structure.
- `updatedAt` – Timestamp of the latest manifest update.
- `files` – List of content files available in the repository.

The manifest helps identify the available content files and their structure.

---

## Publishing Workflow

Content is managed locally and then published to GitHub.

The general workflow is:

```text
┌──────────────────────────────┐
│      Desktop Content Manager │
│                              │
│  Create and edit content     │
│  Manage articles and images  │
│  Update games and social     │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│        Git Integration       │
│                              │
│  Commit local changes        │
│  Push changes to GitHub      │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│       GitHub Repository      │
│                              │
│  Stores published content   │
│  and associated assets       │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│      CPFramework Launcher   │
│                              │
│  Retrieves published data   │
│  Displays updated content   │
└──────────────────────────────┘
```

### Publishing Steps

1. Create or edit content in the desktop Content Manager.
2. The application updates the appropriate content files.
3. Images and other associated assets are managed when included.
4. Git integration commits and uploads the changes to GitHub.
5. CPFramework Launcher retrieves the published content.
6. Users can see the latest available information inside the launcher.

The exact Git workflow depends on the implementation of the desktop application.

---

## Project Components

| Component | Responsibility |
|---|---|
| **Desktop Content Manager** | Creates, edits and manages content locally. |
| **Git / GitHub** | Synchronizes and stores published content. |
| **Content Repository** | Acts as the centralized online content source. |
| **CPFramework Launcher** | Retrieves and displays the published content. |

---

## Technologies & Languages

Technologies, programming languages, formats and development platforms used or explored across Crafty Productions projects.

### Programming Languages

![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

### Web Development

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![TSX](https://img.shields.io/badge/TSX-3178C6?style=for-the-badge&logo=react&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=for-the-badge&logo=electron&logoColor=white)

### Data & Configuration

![JSON](https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white)
![XML](https://img.shields.io/badge/XML-FF6600?style=for-the-badge&logo=xml&logoColor=white)
![YAML](https://img.shields.io/badge/YAML-CB171E?style=for-the-badge&logo=yaml&logoColor=white)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)

### Development Tools & Platforms

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-0E1128?style=for-the-badge&logo=unrealengine&logoColor=white)
![NeoForge](https://img.shields.io/badge/NeoForge-FF6600?style=for-the-badge&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D4?style=for-the-badge&logo=windows&logoColor=white)

---

## About Crafty Productions

**Crafty Productions** is an independent development studio focused on creating video games, software, tools and digital experiences.

This repository is part of the CPFramework ecosystem and supports the content delivery system used by CPFramework Launcher.

---

<sub>Developed and maintained by Crafty Productions.</sub>

**Crafty Productions** – Building projects, creating tools and developing games.
