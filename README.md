# TexDesk for Windows

TexDesk 0.15.8 is a desktop LaTeX editor with automatic compilation and PDF previews.

[Download the Windows installer](https://github.com/qualitystreamzmedia-netizen/TexDesk/releases/latest)

## Installation

1. Download TexDesk-0.15.8-Setup-x64.exe from this repository's Releases page.
2. Run the installer. It installs for your Windows account and creates a TexDesk shortcut.
3. Install MiKTeX or TeX Live if you do not already have a LaTeX distribution. Install any packages required by your documents, including pgfplots for statistical plots.
4. Microsoft Edge WebView2 Runtime is required for the embedded PDF preview.

This installer includes the .NET runtime. It does not bundle a LaTeX distribution or automatically install LaTeX packages. The installer is not digitally signed.

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