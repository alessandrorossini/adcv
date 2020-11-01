# Adaptive CV (adcv) LaTeX class and template

Adaptive CV allows to compile different variants of a CV (e.g., a résumé and an extended CV) from a single LaTeX source. It is particularly suitable for academic CVs but flexible enough to be used with any CVs.

![Alessandro Rossini's CV](https://alessandrorossini.org/wp-content/cv_alessandro_rossini_en.png)

## Requirements

Adaptive CV requires [XeTeX](http://xetex.sourceforge.net/) along with the [array](https://www.ctan.org/pkg/array), [biblatex](https://www.ctan.org/pkg/biblatex), [csquotes](https://www.ctan.org/pkg/csquotes), [enumitem](https://www.ctan.org/pkg/enumitem), [fancyhdr](https://www.ctan.org/pkg/fancyhdr), [fontspec](https://www.ctan.org/pkg/fontspec), [geometry](https://www.ctan.org/pkg/geometry), [hyperref](https://www.ctan.org/pkg/hyperref), [longtable](https://www.ctan.org/pkg/longtable), [parskip](https://www.ctan.org/pkg/parskip), [tikz](https://www.ctan.org/pkg/pgf), [totpages](https://www.ctan.org/pkg/totpages), and [xcolor](https://www.ctan.org/pkg/xcolor) LaTeX classes.

## Class options

The `extended` class option prints the content within the `\ifextended`…`\fi` blocks.  
The `online` class option prints the email address with a bitmap `@` and `.` symbols to prevent email spam, and does not print the street address, the postal code, and the telephone number to preserve privacy.  
The `print` class option prints the CV in grayscale.  
The [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language code (e.g., `en`, default) class option prints the CV using the corresponding language definition file (e.g., `adcv_en.def`, default). Currently, only the [official languages of the European Union](https://europa.eu/european-union/about-eu/eu-languages_en) plus Norwegian are supported.

## Environments and commands

The `\adcvname{`*\<first name\>*`}{`*\<last name\>*`}{`*\<academic degree\>*`}` command defines the first and last names, and the academic degree (e.g., PhD).  
The `\adcvtitle{`*\<title\>*`}` command defines the title.  
The `\adcvaddress{`*\<street address\>*`}{`*\<postal code\>*`}{`*\<locality name\>*`}{`*\<country name\>*`}` command defines the visiting address.  
The `\adcvphone{`*\<phone number\>*`}` command defines the phone number.  
The `\adcvemail{`*\<local name\>*`}{`*\<second-level domain\>*`}{`*\<top-level domain\>*`}` command defines the email address.  
The `\adcvwebsite{`*\<URL\>*`}{`*\<link name\>*`}` command defines the website URL.  
The `\adcvdate{`*\<date\>*`}` command defines the date of the last update. The [day-month-year date format](https://alessandrorossini.org/we-can-put-an-end-to-month-day-year-dates/) is recommended outside the USA.

The `adcvtabletwo` environment provides a generic table with a wide left column and a narrow right column.  
The `\adcvrowtwo{`*\<left column text\>*`}{`*\<right column text\>*`}` command prints a row of the generic table with text in the left column and text in the right column.  
The `\adcvrowmulti{`*\<text\>*`}` command prints a row of the generic table with text spanning across the left and right columns.  
The `\adcvrowskip` command skips a row.

The `adcvlanguages` environment provides a language proficiency table based on the [Common European Framework of Reference for Languages (CEFR)](https://www.coe.int/en/web/common-european-framework-reference-languages).  
The `\adcvmothertongue{`*\<language name\>*`}` command prints the mother tongue.  
The `\adcvlanguagesheader` command prints the header of the language proficiency table.  
The `\adcvlanguage{`*\<footnote number\> (optional)*`}{`*\<language name\>*`}{`*\<listening level\>*`}{`*\<reading level\>*`}{`*\<interaction level\>*`}{`*\<production level\>*`}{`*\<writing level\>*`}` command prints a row in the language proficiency table.  
The `\adcvAOne`…`\adcvCTwo` commands print the A1…C2 proficiency levels, respectively.  
The `\adcvlanguagesfooter` command prints the footer of the language proficiency table.  
The `\adcvlanguagesfootnote{`*\<footnote number\>*`}{`*\<footnote text\>*`}` prints a footnote under the language proficiency table.

The `adcvpresentations` environment provides a presentation enumeration.  
The `\adcvpresentation{`*\<title\>*`}{`*\<conference\>*`}` prints an item in the presentation enumeration with the title in the first row and the conference in the second row.

## License

Copyright 2016-2020 [Alessandro Rossini](https://alessandrorossini.org).  
This work may be distributed and/or modified under the conditions of the [LaTeX Project Public License (LPPL)](https://www.latex-project.org/lppl.txt) version 1.3 or later.  
This work consists of the files `adcv.cls`, `adcv_en.def`, `bib_alessandro_rossini.bib`, and `cv_alessandro_rossini_en.tex`.

## Acknowledgements

Adaptive CV is inspired by [Friggeri CV](https://www.overleaf.com/latex/templates/friggeri-cv-template/hmnchbfmjgqh) and [Europe CV](https://www.ctan.org/pkg/europecv). It uses the [Roboto fonts](https://fonts.google.com/specimen/Roboto) and the [Multimedia Collection icons](https://www.flaticon.com/packs/multimedia-collection).
