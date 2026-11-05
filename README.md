<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="images/logo-dark.png">
    <img src="images/logo-light.png" width="420" alt="Ontology Copilot">
  </picture>
</div>

# Ontology Copilot 0.9.24

A plugin for [Protégé](https://protege.stanford.edu) that helps you draft and edit ontologies with an LLM assistant,
using methods from peer-reviewed research (NeOn-GPT, Ontogenia, RIGOR-Lite and a direct draft). Every change is shown
in Change Preview first; nothing changes in your ontology until you press Apply.

> **Tested with Protégé 5.6.7 on macOS only.** It may not work with other Protégé versions.

## Install

### Option 1: Protégé's plugin installer

1. In Protégé, open the preferences and go to the **Plugins** tab. In **Plugin registry**, paste
   `https://raw.githubusercontent.com/NadeenAhmad/Ontology_Copilot_0.9.24/main/ontology-copilot.repository`
   and confirm.
2. Choose **File ▸ Check for plugins…**, tick **Ontology Copilot** and click **Install**.
3. Restart Protégé.

### Option 2: by hand

1. Download [`protege-ontology-copilot-0.9.24.jar`](protege-ontology-copilot-0.9.24.jar).
2. Quit Protégé and copy the file into Protégé's `plugins` folder:
   - macOS: right-click Protégé.app ▸ **Show Package Contents** ▸ `Contents` ▸ `plugins`;
   - Windows / Linux: the `plugins` folder inside the Protégé folder.

   Delete any older `protege-ontology-copilot-…jar` there.
3. Start Protégé.

## First start

1. Open or create an ontology, then choose **Window ▸ Views ▸ Ontology views ▸ Ontology Copilot (0.9.24)** and click
   where the view should go. A short guided tour starts the first time.
2. Click **Settings…**, choose a **Provider** (OpenRouter, OpenAI or a local Ollama) and a **Model**, paste your API key
   and click **Use for this session only** (or **Save to Keychain** on macOS), then **Test connection**.

## Your data

- Your API key stays on your computer: in the macOS Keychain, or only for the current session.
- The plugin keeps a local activity log of what you do in it (`Documents/OntologyCopilot/activity`). It is never sent
  anywhere, and you can switch it off in Settings.

## Licence

MIT, see [LICENSE](LICENSE).
