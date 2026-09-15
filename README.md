# TexDesk for Windows

TexDesk 0.19.0 is a desktop LaTeX editor with automatic compilation and PDF previews.

[Download the Windows installer](https://github.com/qualitystreamzmedia-netizen/TexDesk/releases/latest)

## Installation

1. Download TexDesk-0.19.0-Setup-x64.exe from this repository's Releases page.
2. Run the installer. It installs for your Windows account and creates a TexDesk shortcut.
3. On Required components, leave missing components checked to install MiKTeX and WebView2. An internet connection is required; setup skips components already detected.
4. If you prefer to install a component yourself later, uncheck it. Compilation requires MiKTeX or TeX Live; PDF preview requires WebView2.

This installer includes the .NET runtime. It downloads MiKTeX (about 150 MB plus plotting packages) when missing and installs pgfplots for a new MiKTeX installation. The bundled Microsoft bootstrapper downloads WebView2 when missing. Existing LaTeX installations and their packages are left unchanged; documents may require additional packages. The installer is not digitally signed.

## New in 0.19.0

- **Calculus:** editable fields for definite and indefinite integrals, first-order derivatives, partial derivatives, and limits.
- **Command suggestions:** suggestions in both editor columns as you type. Arrow keys select; Tab accepts; Esc dismisses. Possible spelling corrections require your selection and can be undone.
- **Symbols:** 116 searchable mathematical symbols with automatic addition of required packages.
- **Implicit plots:** equations such as `x^2+y^2=25`, `x*y=1`, and `y^2=x^3-x` use the existing Plot equation window.
- **Smoother curves:** denser sampling and connected contour segments reduce artificial gaps while preserving genuine discontinuities.

Plot code remains in companion files, leaving short references in your document. Numerical plots may miss tiny features, isolated points, or repeated roots. Command suggestions use a curated catalog and macros declared in the current file; they are not a validator for every LaTeX package.

## Included features

- Automatic source saving, compilation, and PDF preview updates.
- Automatic PDF saving beside the main .tex file after successful compilation.
- Two editor columns, file closing, and source search with visible highlights.
- Statistical plots, probability shading, plot resizing, and readable plot references.
- Generated figure files hidden by default, with an option to show them.
- Live external PDF preview and cursor-to-PDF navigation.
- Guided corrections and optional AI prompts using your own API key.

Source files remain on your computer. Optional AI requests send the prompt and selected content to the configured service when you use that feature. No API key is supplied with this installer.

## Updating and recovery

Installing over an existing TexDesk installation updates the app. Documents are not included in the installer. Source backups are kept in each project's .texdesk/recovery folder. Compilation errors retain the last successful PDF. If another program locks the PDF, close that program and compile again to save the update.

This repository distributes Windows installers; it does not contain the application source code.