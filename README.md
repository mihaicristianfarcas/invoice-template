# Invoice Template

A quiet, minimal LaTeX invoice template: Inter for text, Bera Mono for labels and
numbers, hairline rules, and a single teal accent on the total.

## Quick Start

1. Update company information in the template
2. Modify client details and invoice data
3. Update service items in the table
4. Compile with `pdflatex Invoice.tex` (XeLaTeX, LuaLaTeX, and Tectonic also work)

## Customization

### Company Information
```latex
\newcommand{\companyname}{Your Company Name}
\newcommand{\companystreet}{Your Address}
\newcommand{\companyphone}{Your Phone}
\newcommand{\companyemail}{your@email.com}
```

### Invoice Details
```latex
\newcommand{\invoicenumber}{INV-2024-0001}
\newcommand{\invoicedate}{January 15, 2024}
\newcommand{\invoicedeadline}{February 15, 2024}
```

### Services
```latex
\newservice{Description of the work}{<qty/hours>}{<rate>}
```
Line totals and the invoice total are calculated automatically.

### Colors
```latex
\definecolor{ink}{HTML}{1D1C1A}      % body text
\definecolor{muted}{HTML}{6B6863}    % secondary text and labels
\definecolor{hairline}{HTML}{E4E1DA} % rules
\definecolor{accent}{HTML}{0E7263}   % used sparingly: the total
```

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Packages: `geometry`, `booktabs`, `xcolor`, `eurosym`, `xfp`, `etoolbox`,
  `inter` and `beramono` (fonts), `iftex`

## Features

- Understated, print-friendly layout on pure white
- Uppercase mono labels for all metadata
- Hairline-ruled services table, no stripes
- Automatic per-line and grand totals, padded to two decimals
- Banking information section
