# naletter

This is a [Quarto](https://quarto.org/) extension to provide a PDF letter template. 

## Installation

If you want to start with a template do:
```bash
quarto use template nareal/naletter
```

You just want to install the extension use:
```bash
quarto add nareal/naletter
```

This command installs the extensions under the `_extension` subdirectory.

If you want you can specify the version number:
```bash
quarto add nareal/naletter@v1.0
```

To update the extension use:
```bash
quarto update extension nareal/naletter
```

and to remove it:
```bash
quarto remove extension nareal/naletter
```

## Usage

You can use the following metadata fields:

```yaml
title: "Notes title"
subtitle: "Notes subtitle"
author: "Author name"
date: "2022-10-06"
format:
  nanotes-pdf: 
    fromname: Nelson Areal
    fromaddress: |
                 | School of Economics and Management
                 | University of Minho
                 | Campus de Gualtar
                 | 4710-057 Braga - Portugal
    fromtitle: Associate Professor
    fromWWW: nelsonareal.net
    fromemail: nareal@eeg.uminho.pt
    fromphone: +351 253 601 923
    toname: Helen of Troy
    toaddress: University of Greece\newline Athens
    opening: Dear Helen,
    closing: Best regards,
    spacing: 1.4
    sansfont: NewsGotT
    lang: en-GB # pt-PT
    babel-lang: british # portuguese
    #date: Thursday, 18 October 2022
    #logofilepath:  um-eeg
    #keep-tex: true
```

## Example 

Here is the source code of the template: [template.qmd](template.qmd) and the [rendered PDF file](https://nareal.github.io/naletter/example.pdf).
