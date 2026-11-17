# CPFramework Launcher Content

**The centralized content repository powering CPFramework Launcher.**

This repository provides structured content for the CPFramework Launcher, including launcher news, game information, studio announcements, and social content.

Content is managed through a custom application developed for the Crafty Productions ecosystem. Instead of manually editing JSON files or updating the launcher itself, administrators can create and manage publications through the application, which automatically synchronizes the changes with this repository.

The launcher retrieves the latest content and uses it to populate its interface.

---

## Repository Structure

```text
CPFramework-Launcher-Content/
│
└── content/
    ├── manifest.json
    ├── news.json
    ├── games.json
    └── social.json
```

### Content Files

| File | Description |
|---|---|
| `manifest.json` | Repository manifest containing schema information, update timestamps, and available content files. |
| `news.json` | News articles, announcements, development updates, and studio publications. |
| `games.json` | Game catalog information used by the launcher. |
| `social.json` | Social content and related publications. |

---

## News System

The news system supports structured articles with the following properties:

- **ID** – Unique identifier for each article.
- **Title** – Article headline.
- **Slug** – URL-friendly article identifier.
- **Category** – Article classification.
- **Excerpt** – Short article description.
- **Content** – Full article content.
- **Featured** – Determines whether an article is highlighted.
- **Published** – Controls publication visibility.
- **Published At** – Publication date and time.

This structure allows the launcher to organize, display, and filter publications without requiring application updates.

---

## Manifest System

The `manifest.json` file acts as the central index for the repository.

It contains:

- `schemaVersion` – Version of the content structure.
- `updatedAt` – Timestamp of the latest repository content update.
- `files` – List of available content files.

The launcher can use the manifest to identify available content sources and determine when the repository was last updated.

---

## Publishing Workflow

All content is intended to be managed through the custom CPFramework Content Manager application.

The publishing workflow:

1. Create a new article or content entry.
2. Configure its title, category, description, and content.
3. Configure additional publication properties.
4. Publish the content through the application.
5. The application automatically updates the appropriate repository files.
6. CPFramework Launcher retrieves the updated content.

This eliminates the need for manual repository editing during normal content management.

---

## Integration

This repository is designed to operate independently from the launcher application.

**CPFramework Content Manager**
- Creates and manages content.
- Handles publishing and repository synchronization.
- Maintains content metadata.

**CPFramework-Launcher-Content**
- Stores structured content.
- Provides a centralized source for launcher data.
- Maintains the content manifest.

**CPFramework Launcher**
- Retrieves repository content.
- Displays news and announcements.
- Presents game catalog information.
- Integrates available social content.

---

## Design Principles

- **Centralization** – One repository for launcher content.
- **Automation** – Content publishing without manual JSON editing.
- **Separation** – Content management remains independent of the launcher.
- **Scalability** – New content types and properties can be introduced as the ecosystem grows.
- **Maintainability** – Structured JSON makes content easy to manage and consume.

---

## Part of Crafty Productions

CPFramework Launcher Content is part of the Crafty Productions software ecosystem.

It serves as the content infrastructure behind CPFramework Launcher, helping connect studio publications, game information, and announcements in one centralized location.

**Crafty Productions**  
*Building tools, experiences, and games.*

