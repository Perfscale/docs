# docs

Documentation content for the PerfScale platform. MDX files rendered by the `site` repo at `/docs`.

## Structure

```
docs/
  en/                   # English
    getting-started/
      index.mdx         # overview
      installation.mdx  # installing perfscaled on a machine
      quick-start.mdx   # first test walkthrough
    concepts/
      machines.mdx      # what machines are and how registration works
      tests.mdx         # test definitions and configuration
    api-reference/
      index.mdx         # REST API overview
  ru/                   # Russian / Русский
    getting-started/
      index.mdx         # обзор
      installation.mdx  # установка агента на машину
      quick-start.mdx   # первый тест
    concepts/
      machines.mdx      # что такое машины и как работает регистрация
      tests.mdx         # определения тестов и конфигурация
    api-reference/
      index.mdx         # обзор REST API
  privacy.md            # privacy policy
  terms.md              # terms of service
```

## Usage

This repo is included as a git submodule in `site` at `content/`:

```bash
# in site repo — update docs to latest
git submodule update --remote content
```

## Contributing

Edit MDX files directly. Frontmatter is supported:

```mdx
---
title: Getting Started
description: How to set up your first performance test
---

Content here...
```

Changes are picked up by `site` on the next submodule update or deploy.
