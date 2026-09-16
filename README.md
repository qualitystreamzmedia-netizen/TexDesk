# TexDesk

TexDesk is a Windows LaTeX editor for writing mathematics, building plots, and preparing teaching materials. Version **0.33.0**.

## Start writing

Open a `.tex` document or choose **New**. Type in the source editor and enable **Compile as I type** to update the PDF after a short pause. Successful builds also save the PDF beside the main source file. **F1** opens the searchable help guide, with copyable examples.

## What you can do

- Work in two source columns, move a document to the second column, and restore the previous workspace layout.
- Follow the source cursor in the PDF, use a live external PDF window, and search or preview replacements in source files.
- Insert symbols, fractions, calculus templates, tables and boxes; use command completion and review suggested spelling or package corrections.
- Plot explicit or implicit equations, including several curves together. Add shaded regions with optional area labels.
- Plot common statistical distributions with shading and optional probabilities. Edit saved plot settings and browse figures referenced by the active file.
- Solve supported elementary integrals with worked steps; simplify supported mathematical expressions. These are limited local mathematics tools, not a general computer algebra system.
- Prepare student and instructor copies, store reusable questions, and generate 1–30 randomized versions using parameter rules or local R calculations.
- Preview inserted items, adjust formatting styles and table borders, inspect compiler errors, and recover earlier saved document versions.
- Export a PDF or package the main source and supported local dependencies in a ZIP.

## Randomized teaching materials

Use **Teaching → Randomize** for multi-question tests. Load one of the three-question examples, adjust the questions and matching solutions, choose a seed and version count, and validate all versions before generation. The help guide explains placeholders, parameter rules, R scripts, marks, answer spaces and student/instructor views in detail.

Review the generated answers and student PDFs before distributing them. Ordinary student-mode source documents can still contain hidden solutions; share the intended student PDFs rather than the full project or generation folder.

## Requirements

Windows x64. The installer includes the .NET runtime and offers installation of missing MiKTeX and WebView2 components; prerequisite downloads require internet access. R is optional and must be installed separately for R statistics and numerical integration. LaTeX may download packages on first use. Optional AI features require separate configuration; the ordinary editor, plots and supported mathematics run locally.

The installer is not digitally signed.

## Changes in 0.33.0

Build assignments without an API key from 72 topic families: calculus I–IV, introductory statistics, algebra, linear algebra and discrete mathematics. In **Teaching → Assignment from a prompt**, browse and select topics or enter supported topic keywords, then choose **Create offline assignment**. This is an initial library of selected topics, not a complete course syllabus or a general language model. Review the reported topic matches and generated questions.

Numerical templates generate reproducible values, with optional multiple-choice conversion. Existing conceptual families provide matching, multiple-choice and short-answer questions. Source attribution is preserved in editable assignments, student/instructor PDFs and VIU Learn CSV. One average-velocity family adapts Active Calculus under CC BY-SA 4.0; its notice and editable educational template are included with the installer.

## Changes in 0.32.0

Teaching → Assignment from a prompt prepares editable multiple-choice, matching and single-blank question banks. Use the built-in Math 161 example without a key, or your own OpenAI API key to draft new questions. Review and edit alternatives and arithmetic rules, generate reproducible tests, preview student/instructor views, and export PDFs or VIU Learn CSV pools. CSV contains fixed variants; one blank imports as short answer. Live course import and grading must be checked in VIU Learn.

## Changes in 0.31.1

- Project export follows nested `.TEX`, `.STY` and `.CLS` files regardless of extension case.
- Comments after LaTeX table row endings no longer cause false missing-file errors during export.
- Export checks the source/dependency snapshot and reports conflicts between an included figure and the output PDF filename.
- Oversized dependencies are checked before their contents are loaded.
- Updated documentation and export regression checks.

Project export supports literal dependency paths inside the main document folder. It does not automatically package every possible LaTeX dependency mechanism. If export reports an unsupported path or command, resolve that message before sharing the archive.

## Download

Get the installer from [GitHub Releases](https://github.com/qualitystreamzmedia-netizen/TexDesk/releases/latest). The public repository contains installers and documentation only; it does not contain application source or personal teaching documents.
