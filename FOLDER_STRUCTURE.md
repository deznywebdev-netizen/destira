# DESTIRA Folder Structure

Version: 0.5 Foundation

---

# Philosophy

Every file has one obvious home.

If a developer cannot immediately know where a file belongs,
our structure has failed.

The repository must scale from one developer
to hundreds without becoming confusing.

---

# Root Structure

```
destira/

├── apps/
├── packages/
├── services/
├── infrastructure/
├── docs/
├── scripts/
├── public/
├── .github/
├── README.md
├── LICENSE
└── package.json
```

---

# apps/

Contains every user-facing application.

```
apps/

web/

mobile/

desktop/

admin/
```

---

## web/

Next.js Application

```
web/

app/

components/

features/

hooks/

lib/

styles/

types/

public/
```

---

## mobile/

React Native Application

```
mobile/

components/

screens/

navigation/

hooks/

assets/

services/
```

---

## desktop/

Electron Desktop App

```
desktop/

src/

components/

services/

assets/
```

---

## admin/

Internal administration dashboard.

Only Destira staff can access this.

---

# packages/

Reusable code shared across every app.

```
packages/

ui/

icons/

utils/

config/

ai/

database/

auth/
```

---

# services/

Business logic.

```
services/

employee-engine/

knowledge-engine/

workflow-engine/

notification-engine/

analytics-engine/
```

---

# infrastructure/

Infrastructure configuration.

```
infrastructure/

database/

docker/

terraform/

supabase/

vercel/
```

---

# docs/

Engineering documentation.

```
docs/

Engineering Bible

Product Requirements

System Architecture

Design System

Folder Structure

Database Schema

API Specification

Security

Roadmap
```

---

# scripts/

Automation scripts.

Database migrations

Seed data

Deployment

Testing

Maintenance

---

# public/

Static assets.

Logos

Fonts

Images

Icons

Videos

---

# .github/

GitHub configuration.

Workflows

Issue Templates

Pull Request Templates

Actions

---

# Feature Structure

Every feature follows the same layout.

```
employees/

components/

hooks/

api/

types/

utils/

tests/
```

---

# Naming Rules

Folders

lowercase

hyphen-case

Files

PascalCase for React Components

camelCase for utilities

UPPERCASE only for constants

---

# Component Rules

Every component must:

Be reusable

Be typed

Support Dark Mode

Support accessibility

Have no duplicated logic

---

# Goals

The repository should remain organized after:

100 developers

100,000 files

10 years of development.

No feature should ever require restructuring the repository.
