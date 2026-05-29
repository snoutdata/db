<div align="center">

<img src="icon.png" alt="PositronDB" width="128" height="128" />

# PositronDB

### An AI-driven SQL IDE

A fast, native SQL workbench with a built-in AI assistant that understands your schema.
Connect, explore, write, and run, with smart completion and an assistant that proposes
SQL grounded in your actual tables.

[![Download](https://img.shields.io/github/v/release/positron-labs/db?label=Download&style=for-the-badge&color=2f81f7)](https://github.com/positron-labs/db/releases/latest)
&nbsp;
[![Platform](https://img.shields.io/badge/Windows-10%2F11-blue?style=for-the-badge)](https://github.com/positron-labs/db/releases/latest)

</div>

---

## What it is

PositronDB is a desktop SQL IDE for working with MySQL/Aurora and PostgreSQL. It pairs
a schema-aware editor with an AI assistant that reads your database structure, so the
help you get is specific to *your* data, not generic boilerplate. Manage your
connections, browse the schema, write queries with real completion and hover docs, run
them against a live grid, and ask the assistant when you get stuck.

## Features

### 🤖 Schema-aware AI assistant
- A chat assistant that **proposes SQL grounded in your live schema**: it ranks the
  tables most relevant to your question, follows foreign-key relationships, and feeds
  the model the columns that actually matter.
- Replies render as rich **markdown**, with a per-conversation **token tally** so you
  always know the cost of a thread.
- **Insert proposed SQL** straight into the current editor or a fresh tab, one click.
- **Persistent chat history**: every conversation is saved and reopenable, with search
  and pagination.
- Stop a streaming reply mid-flight and keep the partial answer; start a new chat anytime.

### ✍️ A real SQL editor
- **Multi-tab editing** powered by the Monaco editor with **schema-aware completion and
  hover** (tables, columns, and relationships, served by a dedicated language server).
- **Open and save `.sql` files** with familiar shortcuts (Ctrl+N/O/S/W, Ctrl+Enter to run).
- A **command palette** (Ctrl+Shift+P) for fast, keyboard-first navigation.
- SQL formatting built in.

### 🗂️ Connections & schema explorer
- Manage multiple connections to **MySQL/Aurora** and **PostgreSQL**.
- A tree explorer drills from **connections → databases → tables → columns**.
- **Production connections are flagged**, with a destructive-statement guardrail that
  warns before you run something dangerous against prod.
- **SSH tunnel** support for reaching databases behind a bastion.
- A **live schema index** keeps completion and the AI assistant current as your database
  changes.

### 📊 Results & history
- Run queries against a clean, sortable **results grid**.
- **Query history** and **saved queries** are kept across sessions, so nothing you ran
  is ever lost.

### 🔐 Secure by design
- Database passwords, SSH keys/passphrases, and API keys are encrypted with your OS
  keychain (via Electron `safeStorage`) and never written to plain config files.
- Editor completion and hover are **fully deterministic and local**: no model is ever
  called on keystrokes, and nothing about your editing leaves the machine for those
  features.

### 🎨 Polished desktop experience
- Native **light and dark themes**.
- Resizable, collapsible panes you can lay out the way you work.
- **Automatic updates**: PositronDB checks for new versions on launch, downloads in the
  background, and installs on restart, with release notes shown in-app.

## Download & install

1. Head to the [**latest release**](https://github.com/positron-labs/db/releases/latest).
2. Download **`PositronDB-Setup-<version>.exe`** (installer) or **`PositronDB-<version>.exe`**
   (portable).
3. Run it. Windows SmartScreen may warn on the unsigned installer, choose **More info →
   Run anyway**.

Once installed, PositronDB keeps itself up to date automatically.

> **Platform:** Windows 10/11. Built on Electron.

## Getting started

1. **Add a connection** from the sidebar (host, port, credentials; optional SSH tunnel).
2. **Browse the schema** in the explorer to see your tables and columns.
3. **Open a tab and write SQL**, with completion and hover guiding you.
4. **Run** with Ctrl+Enter and read the results in the grid.
5. **Open the AI panel** and ask a question, the assistant answers using your schema and
   can drop the SQL right into your editor.

---

<div align="center">
<sub>PositronDB · An AI-driven SQL IDE · <a href="https://github.com/positron-labs/db/releases">Releases</a></sub>
</div>
