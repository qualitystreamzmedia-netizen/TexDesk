# TexDesk 1.4.1

**Your ideas, beautifully typeset.**

TexDesk is a Windows LaTeX editor for writing mathematics, creating plots, and preparing teaching materials. Write source on the left and see your compiled PDF alongside it.

**Publisher: Eric Agyekum**  
**Development assistance: OpenAI Codex**

## Download and get started

Download **TexDesk-1.4.1-Setup-x64.exe** from the [TexDesk 1.4.1 release](https://github.com/qualitystreamzmedia-netizen/TexDesk/releases/tag/v1.4.1).

1. Run the installer. It includes the .NET runtime and offers installation of missing MiKTeX and Microsoft Edge WebView2 components.
2. Open TexDesk and choose **New**, or open an existing `.tex` file.
3. Enable **Compile as I type** to refresh the PDF after a short pause. Successful builds also save the PDF beside the main source file.
4. Press **F1** for the searchable help guide and examples. **Help → About TexDesk** shows your installed version and credits.

Save your work and close TexDesk before updating an existing installation. Updates are downloaded and installed separately.

## Linux preview

[Download TexDesk Linux Preview 0.9.1](https://github.com/qualitystreamzmedia-netizen/TexDesk/releases/tag/linux-v0.9.1). The archive contains the self-contained x64 app, installation script and help. Tested on Ubuntu 24.04 under WSL 2/WSLg. Install the native dependencies listed in the release help before running it. This preview includes plotting, assignments, mathematics tools and a table builder with individual line thicknesses; it does not yet include the full Windows feature set.

## New in this update

- Line numbers, clearer build diagnostics, cancellable compilation, and background MiKTeX package installation.
- Local recovery drafts, project-wide search, editor appearance preferences and setup checks.
- Two-way source/PDF navigation, reference and citation completion, and a collapsible document outline.
- Optional review before applying generated changes, with coordinated insertion/package Undo on Windows.
- Reusable teaching export presets and advisory accessibility checks.
- Updated help and examples, using **your LMS** and **your institution** throughout.

Windows includes a local linked PDF view alongside its original viewer. Linux preview supports source/PDF navigation in its image preview and retains a smaller feature set than Windows.

## Write and preview

- Edit in one or two source columns and restore your workspace layout.
- Use the embedded PDF preview or TexDesk's live external PDF window.
- Follow the source cursor in the preview, find text, and review replacements.
- Insert symbols, fractions, powers, subscripts, tables and boxes using guided controls.
- Set table outline, heading and inner-line thicknesses, with overrides for individual horizontal or vertical boundaries.
- Use command suggestions and review supported spelling, package and compilation corrections.
- Export PDFs or package the main document and supported local dependencies in a ZIP.

## Graph and calculate

- Plot explicit and implicit equations, including several curves on one set of axes.
- Add shaded regions with optional area labels.
- Plot common statistical distributions with optional shading and probability labels.
- Adjust plot sizes and edit saved settings; browse generated figures referenced by the active document.
- Solve supported elementary integrals with worked steps and simplify supported expressions.
- Use supported integration-by-parts and nonlinear-substitution methods, and evaluate supported convergent improper integrals with one-sided limits.
- Use optional local R tools for statistics and numerical integration.

## Prepare teaching materials

- Create separate student copies and instructor keys, with configurable answer visibility.
- Save reusable questions and generate 1–30 reproducible test versions using parameter rules or local R.
- Build assignments from an offline library of **72 topic families** covering selected calculus I–IV, introductory statistics, algebra, linear algebra and discrete mathematics topics.
- Select topics directly or use supported topic keywords, without an API key.
- Review and edit multiple-choice, matching and short-answer questions; preview versions before export.
- Export student PDFs, instructor keys and Brightspace-compatible CSV question pools for your LMS.
- Optionally use your own OpenAI API key to draft assignments from broader prompts.

The offline library is a starting collection of selected topics, not a complete course syllabus or a general language model. Supported mathematical tools have defined limits. Review generated questions, answers and plots before use.

LMS exports contain fixed variants, not native Brightspace arithmetic formulas. A single blank imports as short answer. Configure and test question pools, grading and availability in your LMS. TexDesk does not automatically publish to a course. Share the intended student PDFs rather than generation folders or source files containing answers.

## Requirements

- Windows x64.
- A working LaTeX installation for PDF compilation; the installer offers MiKTeX when missing.
- Microsoft Edge WebView2 for PDF previews; the installer offers it when missing.
- Internet access for prerequisite installation and any first-time LaTeX package downloads.
- R installed separately for optional R tools and numerical integration.
- Optional AI drafting requires internet access and separately billed OpenAI API access. The API key is held only while its builder window is open.

Ordinary editing, supported plotting and offline question generation do not require an AI service. The installer is not digitally signed.

## Acknowledgements

TexDesk uses .NET, Microsoft Edge WebView2, PDF.js and Math.NET Numerics. PDF compilation uses your LaTeX installation, and optional statistical tools use R.

One offline average-velocity family adapts Matthew Boelkins's *Active Calculus*, second edition, section 1.1, Preview Activity 1.1.1(c), under CC BY-SA 4.0. Attribution remains attached to exported questions. The installer includes the notice and editable educational template under **ThirdPartyNotices**. Other new offline templates are original TexDesk material.

## This repository

This public repository distributes installers and documentation. Application source code is not included.
