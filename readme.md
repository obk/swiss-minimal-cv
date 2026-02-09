# Swiss Style Resume Template

A minimalist, typography-focused resume template inspired by **Swiss Design** . This template prioritizes legibility, clean grids, and geometric structure, making it ideal for developers, designers, and engineers who value clarity and precision.

## 🎨 Key Features

* **Swiss Design Principles:** Uses a clean, grid-based layout with the classic **Helvetica** font family.
* **High Legibility:** Generous whitespace and a strong hierarchy ensure your content is easily scannable.
* **Smart Commands:** Custom commands like `\cvsection` and `\jobtitle` make adding new entries fast and consistent.
* **Customizable Accent:** Comes with a signature "Swiss Red" accent color that can be easily changed to match your personal brand.

## 🚀 How to Use

1.  **Open in Overleaf:** Upload `main.tex` to your project.
2.  **Edit Personal Info:** Update the Header section in `main.tex` with your Name, Email, and Links.
3.  **Add Content:**
    * Use `\cvsection{Title}{Content}` to create new main sections.
    * Use `\jobtitle{Company}{Location | Date}` for work entries.
    * Use `\itemize` lists with the `[leftmargin=*]` option to keep bullet points aligned.

## ⚙️ Configuration

### Changing the Accent Color
Find the **Colors** section in the preamble and change the HTML hex code for `swissred`:

```latex
% Change FF3300 to your preferred HEX color
\definecolor{swissred}{HTML}{FF3300} 

```

### Changing Fonts

The template uses `helvet` (Helvetica) by default. To use a different sans-serif font, simply change the package:

```latex
\usepackage{helvet}   % Default
% \usepackage{lato}   % Alternative
% \usepackage{roboto} % Alternative

```

### Enabling Page Numbers

Page numbers are hidden by default. If your resume spans multiple pages and you want to show them, find and remove (or comment out) this line in the preamble:

```latex
\pagestyle{empty} % Comment this out to show page numbers

```

## 📄 License

This template is free to use for personal and commercial resumes. Attribution is appreciated but not required.
