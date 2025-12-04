# 🤝 Contribution Guidelines for OmniPub Content Syndication Platform

As an Apex-level project, the `OmniPub-Content-Syndication-Platform-Web-App` adheres to rigorous standards of quality, architecture, and velocity. We welcome contributions that align with our commitment to **Zero-Defect, High-Velocity, Future-Proof** engineering.

## 1. Core Philosophy Alignment

Before contributing, internalize the core mandates outlined in **AGENTS.md**:

*   **Architectural Adherence:** All new code must respect SOLID principles, promote DRYness, and adhere to the established Modular Monolith structure.
*   **Toolchain Mandate:** Contributions must leverage the prescribed Apex Toolchain (e.g., TypeScript/Vite/Tauri or Python/uv/Ruff/Pytest, depending on the module being updated).
*   **Verification First:** Local testing must pass **all** existing suite checks before submitting a Pull Request.

## 2. Workflow: The 5 Stages of Apex Contribution

We follow a strict, high-velocity contribution workflow:

### Stage 1: Research & Setup
1.  **Fork:** Fork this repository under your own namespace.
2.  **Clone:** Clone your fork locally:
    bash
    git clone https://github.com/chirag127/OmniPub-Content-Syndication-Platform-Web-App.git
    cd OmniPub-Content-Syndication-Platform-Web-App
    
3.  **Branch:** Create a feature branch from `main` following the conventional commit standard (e.g., `feat/new-analytics-endpoint` or `fix/api-auth-bug`).

### Stage 2: Development & Internal Verification
1.  **Install Dependencies:** Based on the primary technology stack of the component you are modifying (Refer to `AGENTS.md` for the definitive list).
2.  **Local Testing:** Run the full verification suite for the relevant module:
    bash
    # Example for a Python module
    uv run test
    # Example for a TypeScript module
    npm run test:unit
    
3.  **Linting/Formatting:** Ensure code style is perfect using the mandated formatter (Ruff for Python, Biome for TS):
    bash
    # Example: Run formatter check
    npm run format:check  # or ruff check .
    

### Stage 3: Documentation Update (Mandatory)
Any functional change **must** be accompanied by corresponding documentation updates. This includes:
*   Updating inline code documentation (docstrings/JSDoc).
*   Updating the primary `README.md` if the feature is significant.
*   Updating **AGENTS.md** if architectural patterns have been introduced or modified.

### Stage 4: Pull Request Submission
1.  **Commit:** Push your branch and open a Pull Request against the `main` branch of the **original** repository (`chirag127/OmniPub-Content-Syndication-Platform-Web-App`).
2.  **Template Adherence:** Use the provided **PULL_REQUEST_TEMPLATE.md** fully. Ensure your description clearly explains *What*, *Why*, and *How* the change impacts the architecture.
3.  **Linking:** Reference relevant Issues using keywords (e.g., `Closes #123`).

### Stage 5: Review & Merge
*   PRs will be reviewed against the **Apex Architectural Checklist**.
*   Expect rigorous feedback focused on performance, scalability, and adherence to the 2026 standard architecture.
*   Only code that passes automated CI checks (see `.github/workflows/ci.yml`) and peer review will be merged.

## 3. Reporting Issues & Security Vulnerabilities

### Bug Reports
Use the dedicated template: `.github/ISSUE_TEMPLATE/bug_report.md`. Be precise. Provide minimal, reproducible examples.

### Security
For potential security vulnerabilities, **DO NOT** use standard Issues. Follow the guidelines in **.github/SECURITY.md** to ensure responsible disclosure.

## 4. Code of Conduct

We maintain a professional and inclusive environment. Refer to the overarching principles enforced by the **APEX TECHNICAL AUTHORITY**. Disrespectful or non-constructive criticism will result in immediate closure of contributions and potential blocking.

--- 

*Thank you for contributing to the **OmniPub Content Syndication Platform**.*