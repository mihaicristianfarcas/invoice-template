# Professional Invoice Template

A clean LaTeX invoice template with modern design and easy customization.

## Quick Start

1. Update company information in the template
2. Modify client details and invoice data
3. Update service items in the table
4. Compile with `pdflatex Invoice.tex`

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

### Colors
```latex
\definecolor{primaryblue}{RGB}{44, 82, 130}   % Main color
\definecolor{lightgray}{RGB}{128, 128, 128}   % Labels
```

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Standard packages: geometry, booktabs, colortbl, xcolor

## Features

- Professional layout with clear sections
- Alternating table rows for readability
- Customizable color scheme
- Banking information section
- Clean typography