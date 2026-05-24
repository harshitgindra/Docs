---
layout: default
title: Acknowledgements — MindKnot
---

# Acknowledgements

**MindKnot** — iOS & iPadOS Puzzle App
**Developer:** Harshit Gindra
**Version:** 1.0 (V2 features in development)
**Bundle ID:** com.hgindra.mindknot

---

## Open-Source Libraries

### GRDB.swift

**Author:** Gwendal Roué
**Version used:** See Package.resolved for exact version
**Repository:** https://github.com/groue/GRDB.swift
**Purpose:** Reading the bundled SQLite riddle database at runtime
**Licence:** MIT License

```
MIT License

Copyright (c) 2015-present Gwendal Roué

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## Apple Frameworks

MindKnot is built using the following Apple-provided frameworks, which are
part of the iOS SDK and are used under Apple's standard developer licence:

| Framework | Purpose |
|-----------|---------|
| **SwiftUI** | User interface construction |
| **SwiftData** | Local data persistence (session history, streak, preferences) |
| **CloudKit** | iCloud Sync for Pro users; cloud storage for future multiplayer features (Duel Mode, Remote Party — coming in a future update) |
| **MultipeerConnectivity** | Local peer-to-peer networking for Local Party Mode |
| **StoreKit 2** | In-app purchase processing for MindKnot Pro |
| **Security (Keychain)** | Secure local storage of Pro entitlement status |
| **UserNotifications** | On-device daily reminder scheduling |
| **UIKit** | Haptic feedback engine; App Store review prompt |

---

## Riddle Content Sources

### Open-Source Riddle Dataset

A portion of the base riddle content used in this app was derived from the
following open-source dataset:

**Repository:** https://github.com/crawsome/riddles
**Licence:** Public Domain / Creative Commons Zero (CC0)
**Author:** crawsome (GitHub)

All riddles sourced from this dataset were paraphrased, reformatted, and
enriched before inclusion in the app. The original dataset is dedicated to
the public domain and carries no restrictions on use.

---

## AI-Assisted Content Development

The riddle database bundled with this app was developed with the assistance
of AI language models during an offline data processing pipeline. This
assistance was used for:

- Paraphrasing and rewriting base riddle content
- Generating progressive hint text (direction hints)
- Pre-computing letter-reveal hint patterns
- Classifying riddles into categories and difficulty levels
- Generating multiple-choice answer options for Party Modes

**AI services used during development (not at runtime):**

**Amazon Bedrock — Claude (by Anthropic)**
Used as part of the developer's offline ETL (Extract-Transform-Load)
pipeline to enrich riddle content. This service is used only by the
developer on their own machine to build the riddle database. The processed
riddle database is bundled with the app as a static SQLite file.

**The app itself makes no calls to any AI service at runtime.
Users' riddle answers and interactions are never sent to any AI service.**

---

## Special Thanks

To the open-source community, whose generosity in sharing code, data, and
knowledge makes projects like this possible.

---

*MindKnot — © 2026 Harshit Gindra. All rights reserved.*
