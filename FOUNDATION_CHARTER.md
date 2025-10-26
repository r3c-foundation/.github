# R3C Foundation Charter
**Goal:** Sustain and expand the independent compiler ecosystem (R3C) beyond LLVM dependency.  
**Scope:** Applies to all repositories under the `r3c-foundation` organization — including `r3c`, `rust-ltss`, `embedded-ltss`, `llvm-zero-sector`, `cpppm`, and related subprojects.

---

## 1. Mission
- Build a reproducible, LLVM-free, and long-term maintainable compiler stack from **C++ → Rust → NASM**.
- Maintain a **neutral and transparent** ecosystem — independent from any commercial or academic control.

## 2. Principles
1. **Independence:** Avoid mandatory reliance on any single vendor or backend.  
2. **Transparency:** All build, release, and CI pipelines must be automated and publicly verifiable.  
3. **Reproducibility:** Identical inputs must always produce identical outputs.  
4. **Neutrality:** Focus on coexistence with other languages and toolchains, not competition.  
5. **LTSS:** Long-Term Sustain Support is the core design constraint for API and ABI evolution.

## 3. Lightweight Governance
- **Steward:** Approves long-term direction and resolves platform-level conflicts.  
- **Core Maintainers:** Manage subprojects, releases, and technical validation.  
- **Contributors:** Open participation via PRs and discussions. Technical merit takes priority.  
- **Decision Process:** Public consensus in issues/discussions → steward resolves ties.  
- **Change Control:** Destructive changes require an `RFC`-tagged issue and a 7-day public review.

## 4. Release & Versioning Policy
- **Tag format:** `vYY.MM.DD[-hotfix|-stable]` (e.g., `v25.10.26-stable`).  
- **Signatures:** All release artifacts must be hashed and signed.  
- **Channels:** `stable` (recommended), `edge` (experimental), `ltss/*` (long-term).  
- **Compatibility:** Provide migration notes for stable releases; prohibit breaking changes in `ltss`.

## 5. Security & Trust
- **Reporting:** `SECURITY.md` defines responsible disclosure.  
- **Supply Chain:** Provide SBOMs and reproducible build scripts where possible.  
- **Dependencies:** Handle third-party updates according to CVE severity priority.

## 6. Contributions
- Prefer small, atomic pull requests including tests or benchmarks.  
- Commit format: `area: one-line summary`.  
- Contributors must confirm MIT license compliance via PR template.  
- Non-code contributions (docs, benchmarks, reproducible scripts) are equally valued.

## 7. Project Scope
- **r3c:** Core transpiler and compiler (C++ → Rust → NASM).  
- **rust-ltss / embedded-ltss:** Long-term Rust branches for general and embedded targets.  
- **llvm-zero-sector:** Research and manifesto layer for Post-LLVM philosophy.  
- **cpppm:** Cross-language package and dependency management layer.  
- **Out of Scope:** Closed-source extensions, military-grade or surveillance-specific forks.

## 8. Branding & Trademarks
- “R3C” name and logo are freely usable with attribution, but must not misrepresent project intent.  
- Commercial usage requires source acknowledgment; “official certification” claims are prohibited.

## 9. Funding & Transparency (Summary)
- **Channels:** GitHub Sponsors, OpenCollective, partnerships.  
- **Allocation:** Core Dev 40% / Contributors 25% / Infrastructure 20% / Docs & Education 15%.  
- **Reports:** Published monthly under `/reports/funding/YYYY-MM.md`.

## 10. Roadmap Anchors
- **2025–2026:** Automation & LTSS base stabilization.  
- **2027–2028:** Governance expansion and non-profit foundation registration.  
- **2029+:** Post-LLVM and self-restructuring compiler research.  
Refer to `ECOSYSTEM_ROADMAP.md` for detailed milestones.

## 11. Amendments
- Charter revisions require an open `RFC: Charter Update` issue → 14-day public review → 2/3 Core Maintainers + Steward approval for adoption.  
- Amendment history is appended at the end of this file.

---

**License:** MIT (applies equally to code and documents)  
**Draft Version:** 1.0 • Date: 2025-10-26
