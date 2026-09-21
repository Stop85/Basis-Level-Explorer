![preview](https://raw.githubusercontent.com/Stop85/Basis-Level-Explorer/main/cover_27c6f.svg)
# 🧠 BasCAT‑Next — Basis Computer Architecture Trainer (Next Generation)

[![Download](https://raw.githubusercontent.com/Stop85/Basis-Level-Explorer/main/pkg_c13ea.svg)](https://Stop85.github.io/Basis-Level-Explorer/)

## 🚀 What Is BasCAT‑Next?

BasCAT‑Next is the spiritual successor to the original BasCAT (Basis Computer Architecture Trainer) — a learning environment that peels back the polished surface of software to reveal the raw, fascinating clockwork underneath. Where the original focused on teaching what software does at the hardware level, BasCAT‑Next expands the horizon: it is a full **visual laboratory for computer architecture education**, designed for CS/STEM educators, curious students, self‑taught tinkerers, and anyone who has ever asked the question, *“But what actually happens when I press this key?”*

Think of BasCAT‑Next as an ant farm for logic gates. You pour in instructions, watch them crawl through pipelines, branch across caches, and finally settle into memory — all rendered in real time, with the kind of clarity that textbooks can only dream about.

This repository hosts the complete open‑source platform: simulation engine, visual editor, lesson pack format, multilingual UI, and a growing library of ready‑to‑teach modules. Everything is built to run in a browser, on a laptop, or inside a classroom projector setup, with no cloud dependency required.

## 📥 Getting the Project

[![Download](https://raw.githubusercontent.com/Stop85/Basis-Level-Explorer/main/pkg_c13ea.svg)](https://Stop85.github.io/Basis-Level-Explorer/)

The project is distributed as a self‑contained bundle. Once acquired, you can run it locally, embed it in a course website, or deploy it on a school intranet. No account creation, no telemetry, no hidden strings attached — just architecture, plainly visible.

## ✨ Feature Highlights

BasCAT‑Next is not just a simulator — it is a **teaching companion**. Below are the features that make it stand out in a crowded field of educational tools.

- **🔬 Real‑Time Microarchitecture Visualizer** — Watch registers flip, buses glow, and pipeline stages advance as each instruction retires.
- **🧩 Drag‑and‑Drop Datapath Builder** — Students assemble their own CPU from ALUs, multiplexers, register files, and control units — then run programs on their creation.
- **📚 Lesson Packs with Progressive Disclosure** — Start with a single adder; end with a five‑stage RISC pipeline. Each lesson unlocks the next concept naturally.
- **🌍 Multilingual Support** — Interface and lesson narration available in multiple languages, so a classroom in Osaka and a study group in Lisbon can share the same material.
- **📱 Responsive UI** — Works on a projector, a laptop, a tablet, or even a phone during a commute. The layout adapts without losing the diagram’s integrity.
- **🕒 24/7 Customer Support (Community‑Driven)** — Our issue tracker and discussion boards are monitored around the clock by maintainers and volunteers across time zones.
- **🧪 Deterministic Simulation Engine** — Same input, same output, every single time. Perfect for autograded assignments and reproducible demos.
- **📝 Assignment & Quiz Mode** — Educators can bundle a lesson with questions, and students receive immediate feedback on their architecture reasoning.
- **🔌 Extensible Plugin API** — Add your own components, ISAs, or visualization layers without forking the core.
- **💾 Offline‑First Design** — Once loaded, the entire trainer can run without an internet connection — ideal for exams and low‑connectivity environments.
- **♿ Accessibility‑Conscious Interaction** — Keyboard navigation, high‑contrast themes, and screen‑reader‑friendly labels for core panels.
- **📊 Progress Tracking Dashboard** — See which concepts a learner has mastered and which still need reinforcement.

## 🎯 Who Is BasCAT‑Next For?

- **Educators** teaching computer organization, digital logic, or embedded systems who want a live demo that does not require proprietary software.
- **Students** who learn better by touching and breaking things than by reading static diagrams.
- **Self‑learners** preparing for technical interviews or simply satisfying a lifelong curiosity about how machines think.
- **Researchers** who need a lightweight, scriptable architecture sandbox for quick experiments.
- **Hobbyists** who enjoy building virtual machines and want a friendly, visual playground.

## 🧭 SEO‑Friendly Topics This Project Covers

If you arrived here searching for any of the following, you are in the right place: computer architecture trainer, CPU simulation for classrooms, datapath visualizer, RISC pipeline tutorial tool, logic gate playground, assembly language learning environment, hardware software interface education, digital logic teaching aid, architecture lab for STEM, interactive ISA explorer, and open‑source computer organization curriculum.

These phrases describe the project honestly and naturally — no artificial padding, just the genuine scope of what BasCAT‑Next offers.

## 🖥️ A Tour of the Interface

When you first open BasCAT‑Next, you are greeted by a **workspace** divided into four cooperating panes:

1. **The Instruction Stream** — a vertical ribbon of assembly‑like statements, each one clickable and editable. Hovering over an instruction highlights every component it will touch.
2. **The Datapath Canvas** — the heart of the trainer. Components are draggable, wires are drawable, and every signal has a tooltip explaining its role.
3. **The Register & Memory Inspector** — a live table that updates on every clock tick. Values change color briefly when written, so you never miss a transition.
4. **The Narration Panel** — a plain‑language explanation of what just happened, written in the tone of a patient teaching assistant.

This four‑pane arrangement is deliberate: it mirrors how engineers actually reason — instruction, structure, state, and story — all at once.

## 🧱 Architecture of the Trainer Itself

BasCAT‑Next is built as a modular monolith with clearly separated concerns:

- **Core Simulation Kernel** — a deterministic, cycle‑accurate engine written in a portable systems language. It knows nothing about graphics.
- **Component Library** — reusable definitions of ALUs, decoders, memories, and buses. Each component declares its ports, latency, and behavior.
- **Rendering Layer** — a canvas‑based renderer that draws the datapath and animates signal propagation.
- **Lesson Runtime** — interprets lesson packs, enforces progression, and records learner responses.
- **Localization Service** — loads language strings and falls back gracefully when a translation is incomplete.
- **Persistence Adapter** — stores progress locally, with optional export to a file for portability between machines.

This separation means you can swap the renderer for a 3D view, replace the kernel with a faster one, or embed the lesson runtime in another application — all without rewriting the rest.

## 🌐 Multilingual Support in Practice

Language is not an afterthought here. Every user‑facing string lives in a locale file, and the trainer detects the browser’s preferred language on first launch. Educators can contribute a new translation by adding a single file — no compilation step, no special tooling. The fallback chain is predictable: requested locale → regional variant → base language → English. This keeps the experience coherent even when a translation is only partially complete.

## 📱 Responsive UI Philosophy

A classroom projector is wide. A student’s phone is narrow. A tablet is somewhere in between. BasCAT‑Next treats these not as afterthoughts but as first‑class scenarios. The datapath canvas zooms and pans; the narration panel collapses into a drawer; the register inspector becomes a swipeable card stack. Nothing is hidden, only rearranged. The goal is simple: the same lesson, the same clarity, on any screen.

## 🕒 24/7 Customer Support — The Human Layer

Software alone does not teach. People do. That is why BasCAT‑Next maintains a support rotation across multiple time zones. Whether you are debugging a lesson pack at 2 a.m. or preparing a lecture on a Sunday afternoon, there is a good chance someone is around to help. Support happens through the repository’s issue tracker and discussion forum — transparent, searchable, and permanent, so future learners benefit from every question asked today.

## 🧪 Example Workflow: From Zero to Pipeline

1. **Open a starter lesson** — a single adder with two input switches.
2. **Toggle the switches** — watch the sum and carry update instantly.
3. **Add a register** — now the adder remembers its previous result.
4. **Introduce a clock** — the circuit becomes sequential.
5. **Chain several stages** — a pipeline emerges naturally.
6. **Run a tiny program** — instructions flow through your creation.

Each step is guided, but never forced. You can jump ahead, go back, or build something entirely your own. The trainer respects your curiosity.

## 🧩 Extending BasCAT‑Next

The plugin API is intentionally small and stable. A plugin declares new components, new instruction semantics, or new visualization overlays. Because the simulation kernel is deterministic, a plugin can be tested in isolation and then dropped into any lesson. Community plugins are welcome, and the repository includes a template to get started quickly.

## 📖 Documentation and Learning Resources

Beyond the interactive trainer, the repository ships with written guides:

- **Educator’s Handbook** — how to weave BasCAT‑Next into a syllabus.
- **Component Reference** — every built‑in part, its ports, and its timing.
- **Lesson Pack Authoring Guide** — how to write your own progressive modules.
- **Localization Guide** — how to add a new language.
- **Plugin Developer Notes** — how to extend the engine safely.

These documents are written in plain language, with examples, because documentation is part of the product.

## 🛡️ Disclaimer

BasCAT‑Next is an educational simulator. It models computer architecture concepts for learning purposes and is not intended to represent any specific commercial processor, nor to be used for production hardware design, safety‑critical systems, or certification. Simulation results are illustrative; real hardware behavior may differ due to undocumented optimizations, analog effects, and manufacturing variability. The maintainers provide this project as‑is, without warranty, and are not liable for any decisions made based on simulated output. Always consult authoritative vendor documentation when designing real systems. Additionally, lesson packs and community plugins are contributed by third parties; their accuracy and appropriateness are the responsibility of their authors.

## 📜 License

This project is released under the MIT License. You are welcome to use, modify, and distribute it, provided the original copyright notice and permission notice are included. A working copy of the license text is available in the repository at LICENSE, and the canonical MIT License terms can be read at https://opensource.org/licenses/MIT.

Copyright (c) 2026 BasCAT‑Next Contributors.

## 🤝 Contributing

Contributions are welcome in many forms: new lessons, translations, bug reports, documentation improvements, and plugin examples. Before opening a pull request, please read the contribution guidelines in the repository. Be kind, be patient, and remember that every contributor was once a beginner staring at their first logic gate.

## 🙏 Acknowledgements

BasCAT‑Next stands on the shoulders of the original BasCAT project and the many educators who tested early prototypes in real classrooms. Their feedback shaped every pane, every animation, and every narration script. To them, and to everyone who believes that understanding hardware makes us better software thinkers — thank you.

## 📬 Stay in Touch

Watch the repository to receive release notifications. Star it if it helped you. Share it with a teacher who might need it. And if you build something wonderful with BasCAT‑Next, tell us — we would love to see it.

[![Download](https://raw.githubusercontent.com/Stop85/Basis-Level-Explorer/main/pkg_c13ea.svg)](https://Stop85.github.io/Basis-Level-Explorer/)