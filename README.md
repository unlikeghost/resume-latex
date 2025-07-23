# Professional Resume - LaTeX

A modular LaTeX resume template with clean structure and easy customization.

## 📁 Structure

```
.
├── Eng/                          # English version
│   ├── main.tex                  # Main document file
│   ├── main.pdf                  # Compiled resume (generated)
│   └── sections/                 # Modular content sections
│       ├── 1.- personal_information.tex
│       ├── 2.- summary.tex
│       ├── 3.- education.tex
│       ├── 4.- publications.tex
│       ├── 5.- research_experience.tex
│       ├── 6.- professional_experience.tex
│       ├── 7.- technical_skills.tex
│       ├── 8.- languages.tex
│       └── 9.- extra.tex
└── README.md                     # This file
```

## 🚀 Quick Start

### Prerequisites
- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Text editor (VS Code with LaTeX Workshop extension recommended)

**Ubuntu/Debian:**
```bash
sudo apt install texlive-full latexmk
```

### Compilation
```bash
cd Eng/
latexmk -pdf main.tex
```

Or use your LaTeX editor's build function.

## ✏️ Customization

### Personal Information
Edit `sections/1.- personal_information.tex` with your contact details.

### Adding/Removing Sections
1. Create new `.tex` file in `sections/`
2. Add `\input{sections/filename.tex}` to `main.tex`
3. Recompile

### Language Variants
To create Spanish version:
1. Copy `Eng/` folder to `Esp/`
2. Change `\usepackage[english]{babel}` to `\usepackage[spanish]{babel}` in main.tex
3. Translate content in sections

## 📝 Section Guide

- **Personal Information**: Contact details, links
- **Summary**: Brief professional overview  
- **Education**: Degrees, institutions, dates
- **Publications**: Academic papers, conferences
- **Research Experience**: Academic/research positions
- **Professional Experience**: Industry work experience
- **Technical Skills**: Programming, tools, technologies
- **Languages**: Language proficiency levels
- **Extra**: Awards, certifications, interests
