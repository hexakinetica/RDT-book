# The RDT Book: Building a Real-World Robot Control System

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Book Status](https://img.shields.io/badge/status-public%20draft-orange)](https://github.com/hexakinetica/rdt-book)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/hexakinetica/rdt-book/pulls)
[![Zenodo DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15866825.svg)](https://doi.org/10.5281/zenodo.15866825)

**An open-source guide to the architecture and implementation of industrial robot controllers.**

This repository contains the full LaTeX source code for the book that documents the **[Robot Development Toolkit (RDT)](https://github.com/hexakinetica/rdt-core)**. This book and the code are two halves of the same whole.

---

### ⚠️ Book Status: Living Document (Public Draft)

**This is a public draft.** The primary goal of this book is to be a **living document** that evolves alongside the RDT codebase. It is designed to be read, criticized, and improved by the community.

**What this means for you:**

*   **There are typos and rough patches.** You will find grammatical errors, unfinished sections, and placeholders. The "final" version does not exist yet; we are building it together.
*   **Content is the main feature.** The core value here is in the honest explanation of engineering trade-offs and architectural decisions, not in perfect prose. We prioritize practical insights over literary elegance.
*   **This is the perfect place to contribute!** Found a typo? Is an explanation unclear? Do you have a better analogy? Can you translate a section? Your contributions to this text are as valuable as code contributions to the RDT project.

Think of this repository as the shared "lab notebook" for the RDT project. The fundamentals are here, and we invite you to help us fill in the details and polish the explanations.

---

### Philosophy: A Field Manual, Not a Textbook

This book is a "field manual," designed to bridge the gap between university-level robotics and the robust, deterministic, and maintainable systems required on a factory floor. We don't just show you the "what"; we obsess over the "why."

This book is architected to teach key principles of industrial automation software:

*   **From Why to How**: We start with high-level systems engineering principles and trace them all the way down to specific C++ implementations.
*   **Code-First Approach**: Every architectural pattern discussed is backed by a real, working implementation in the [RDT Core Repository](https://github.com/hexakinetica/rdt-core).
*   **Honest Engineering**: We openly discuss trade-offs, design mistakes, and the "ugly" parts of real-world development that are often omitted from textbooks.
*   **Open and Collaborative**: This book is written in the open. You can see its history, participate in discussions via Issues, and suggest improvements via Pull Requests.

### Table of Contents (Draft)

A high-level overview of the book's structure.

| Part | Chapter Title | Core Concepts |
| :--- | :--- | :--- |
| **I** | **Philosophy & Systems Engineering** | The "Why". From prototype to product, V-Model, requirements, common design mistakes. |
| **II** | **The Language of a Robot** | The "What". Kinematics, dynamics, coordinate transformations (frames, FK/IK, Jacobians). |
| **III** | **Core Controller Architecture** | The "How". RT/NRT separation, SSOT state bus, HAL, safety, the Command Conveyor. |
| **IV** | **Implementation in C++** | Translating architecture to modern C++. Design patterns, lock-free queues, RAII. |
| **V** | **Advanced & Future Topics** | Extending the core. Path correction, force control, advanced I/O, future of RDT. |

---

## How to Contribute (All Skills Welcome!)

We are thrilled you're interested in contributing! This project is driven by the community, and we believe that a good idea is more important than mastering a specific tool.

### The Easy Way: No LaTeX Required!

If you found a typo, have a suggestion, or think an explanation could be clearer, the easiest way to let us know is by:

1.  **Creating an Issue:** Go to the [Issues tab](https://github.com/hexakinetica/rdt-book/issues) and click "New Issue". Simply describe your finding or suggestion. You can even include a screenshot. This is the preferred method as it allows for public discussion.
2.  **Sending an Email:** If you prefer, you can send your feedback directly to `contact@hexakinetica.com`.

### The Pro Way: Submit a Pull Request

If you are comfortable with LaTeX:

1.  **Fork** this repository (`rdt-book`).
2.  **Create a new branch** for your fix (`fix/typo-in-chapter-3`) or suggestion (`feature/better-hal-analogy`).
3.  **Make your changes** to the `.tex` source files.
4.  **Submit a Pull Request!** Please check the `CONTRIBUTING.md` file for style guidelines.

### Looking for Code Contributions?

If your contribution is related to the C++ code of the robot controller itself, please head over to the core repository:
*   **[RDT Core Repository](https://github.com/hexakinetica/rdt-core)**

### Building the Book from Source

#### 1. Dependencies
You need a working LaTeX distribution that supports `lualatex`. We recommend [TeX Live](https://www.tug.org/texlive/). The book uses several specific packages, which are all listed in the preamble of the main `.tex` file.

#### 2. Building
The project is built using `lualatex` due to its excellent support for modern fonts and Unicode.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/YourUsername/rdt-book.git
    cd rdt-book
    ```
2.  **Compile the document:**
    ```bash
    lualatex main.tex
    ```
    You may need to run it a couple of times to resolve all cross-references and update the table of contents.

---

### License

This work is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

You are free to:
*   **Share** — copy and redistribute the material in any medium or format.
*   **Adapt** — remix, transform, and build upon the material for any purpose, even commercially.

Under the following terms:
*   **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.

For the full license text, see: [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
