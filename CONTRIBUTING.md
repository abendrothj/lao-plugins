# Contributing to the LAO Plugin Registry

Thank you for strengthening the LAO agentic workflow ecosystem!  
You can contribute new plugins, documentation, or improvements.

---

## ✨ Adding a Plugin

1. **Fork this repo.**
2. **Create a new folder** under `/plugins/` for your plugin (e.g., `/plugins/MyPlugin/`)
3. **Add the following files:**
    - `plugin.yaml` (see [README.md](../README.md) for required format)
    - `README.md` (installation, usage, author/contact, compatible LAO version)
    - Any binaries, examples, or extra docs

4. (Optional) Add tests or GitHub Actions configs if your plugin can be CI-verified.

5. **Open a Pull Request** to submit your plugin for review.

---

## 📝 Manifest/Docs Requirements

- `plugin.yaml`: see example in [README.md](../README.md)
    - Required fields: name, version, description, author, license, tags, compatible_core, capabilities, etc.
    - Optionally: dependencies, repository, homepage, etc.
- `README.md`: must explain
    - How to install and use your plugin
    - Compatible LAO core versions
    - Example commands/workflows
    - License & author info

---

## 🔍 Review & Acceptance Workflow

- The LAO team will review PRs for:
    - Manifest and structure compliance
    - Usefulness
    - Clear documentation
    - Security/compatibility (where appropriate)
- Once accepted, your plugin will appear in the directory and on the Jekyll site at https://abendrothj.github.io/lao-plugins

---

## 👐 Need Help?

Open an issue or discussion in this repo, or ask in the core LAO repo.

Thank you for building the local AI workflow revolution!