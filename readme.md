# minimalist latex cv template

a clean, professional, and ats-friendly cv/resume template based on swiss design principles. focused on typography, readability, and ease of editing.

![cv preview](cv.png)

## 🎨 features

* **clean design:** minimalist layout using helvetica/arial for maximum readability.
* **ats friendly:** single-column layout with standard fonts ensures applicant tracking systems parse it correctly.
* **easy customization:** centralized color definitions and custom commands for sections.
* **print ready:** professional margins and black/dark-gray color scheme for clear printing.

## 🚀 quick start

### option 1: overleaf (recommended for beginners)
1.  download this repository as a `.zip` file.
2.  go to [overleaf](https://www.overleaf.com/).
3.  click **new project** -> **upload project**.
4.  upload the zip file and hit **recompile**.

### option 2: local build
you need a latex distribution installed (tex live, mactex, or miktex).

1.  clone the repo:

2.  compile the pdf:
    ```bash
    pdflatex main.tex
    ```

## 🛠️ how to customize

open `cv.tex` in your favorite editor (vs code, texshop, overleaf).

### 1. changing personal info
navigate to the `% --- header ---` section in the document body.

```latex
\textbf{\MakeUppercase{your name}} \\[0.2cm]
{\color{darkgray}
title 1 $\cdot$ title 2 \\
+1 555 123 4567 $\cdot$ \href{mailto:email@example.com}{email@example.com}
}

```

### 2. adding experience

use the custom `\jobtitle` command followed by the description.

```latex
\jobtitle{company name}{date range}
\textit{job title} \\
description of your role...

```

### 3. changing colors

find the `% --- colors ---` section at the top of the file. you can use standard html hex codes.

```latex
\definecolor{mainblack}{HTML}{000000} % main text
\definecolor{darkgray}{HTML}{333333}  % subtitles & metadata
\definecolor{lightgray}{HTML}{555555} % lighter accents

```

### 4. adjusting margins

if you need more space, adjust the geometry package settings:

```latex
\usepackage[left=1.5cm,right=1.5cm,top=1.25cm,bottom=1.25cm]{geometry}

```

## 📄 license

this project is open source and available under the mit license.
feel free to use it for your own cv!
