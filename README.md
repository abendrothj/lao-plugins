# LAO Plugin Ecosystem

Welcome to the **official community plugin registry** for [LAO (Local AI Orchestrator)](https://github.com/abendrothj/lao)!  
This is the place to **discover, share, and contribute plugins** that supercharge your local AI workflows.

:rocket: **Explore plugins on our site:**  
https://abendrothj.github.io/lao-plugins

---

## 🌟 About LAO

LAO is an offline, agentic workflow engine for chaining local AI models and plugins into powerful, prompt-driven pipelines. This repo powers the **plugin ecosystem**—open to all!

---

## 📚 Plugin Directory Structure

Plugins live in `/plugins/YourPluginName/`:

```
/plugins/
  /MyPlugin/
    plugin.yaml     # Plugin metadata (manifest, see below)
    README.md       # Usage/install info
    [binaries, examples, source, etc.]
```

### Example plugin.yaml:
```
name: MyAwesomePlugin
version: 1.0.0
description: Adds next-gen AI processing to LAO
author: Contributor Name
license: MIT
repository: https://github.com/yourusername/my-awesome-plugin
tags: [ai, processing, text]
capabilities:
  - name: summarize
    description: Summarizes text with LLM
    input_type: text
    output_type: text
compatible_core: 0.5.0
dependencies: []
```

---

## 🚀 Quick Start

**To use plugins:**  
1. Browse or search plugins on [the site](https://abendrothj.github.io/lao-plugins).
2. Each plugin's `README.md` has install/use instructions.
3. Check `plugin.yaml` for compatibility/version info.

**To contribute a new plugin:**  
1. Fork this repo, add a new directory to `/plugins/`.
2. Include your `plugin.yaml`, `README.md`, and binaries (if distributing).
3. Submit a Pull Request (see [CONTRIBUTING.md](CONTRIBUTING.md))!

---

## 🧩 Plugin Requirements

- `plugin.yaml` manifest: required fields as above.
- Documentation (`README.md`): how to install/use, contact.
- All distributed binaries built for major OS targets, where needed.
- List dependencies and special requirements.

Best starting point: [`plugin-template`](https://github.com/abendrothj/lao/tree/main/plugins/plugin-template)

---

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for full details!

- Fork, branch, PR—just like any open source repo.
- We welcome all contributions that enhance LAO's local agentic workflows.

---

## 🆘 Support

- Plugin-specific issues: check their README or linked repo.
- General help/questions? Open an issue here.
- For engine/core issues: visit [LAO main repo](https://github.com/abendrothj/lao).

---

## 📄 License

Each community plugin: see its own license.  
This registry is MIT-licensed.

---

## 💡 About

Built for the LAO ecosystem with GitHub Pages & Jekyll.  
Want to help LAO grow? Build and contribute a plugin!