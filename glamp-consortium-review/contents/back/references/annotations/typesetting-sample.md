---
description: Annotation Typesetting Sample for JBT
---

# Typesetting Sample

## Sample Information

### Citekey

For illustrative purposes, we have selected Maranhao2020.

### Source

Our bibliography is a `.bib` database.  
Each entry is structured data in `bibtex` format.  
An annotated entry's source is stored like so:

```text
@Article{Maranhao2020,
  author    = {Andre Maranhao and Sanchita Bhadra and Inyup Paik and David Walker and Andrew D. Ellington},
  title     = {An improved and readily available version of Bst {DNA} Polymerase for {LAMP}, and applications to {COVID}-19 diagnostics},
  year      = {2020},
  month     = {oct},
  doi       = {10.1101/2020.10.02.20203356},
  groups    = {04-target-amplification, has-annotation, 10.08-bst-polymerase-biology},
  publisher = {Cold Spring Harbor Laboratory},
  timestamp = {2020-12-17},
  annote    = {%
               \onestar\\
               Protein engineering fusion improves function of Bst DNA polymerase in  LAMP\\
               Modifying Bst DNA polymerase significantly improves reverse transcriptase activity\\
               Further improves LAMP-OSD detection in pre-heated saliva without RNA extraction\\
             %}
}
```

In this source, the `annote` field contains the annotations.

1. `\onestar` is priority 1 on the 1-3 scale, where 3 is highest.
2. `\\` is a line-separator.
3. Further lines are highlight bullets on the cited work.

## Usage

### Inline Use

We cite Maranhao2020 by its **citekey,** Maranhao2020**.**  
We do this using the `\cite` command, as in:

> Lorem ipsum dolor sit amet.\cite{Maranhao2020}



### In References

Once rendered, this turns into a numeric value in brackets.  
If Maranhao2020 is reference number 4, for instance, the output is:

> Lorem ipsum dolor sit amet.\[4\]

## Appearance

### Current Appearance

In our working draft's References section, Maranhao2020 renders like so:

\[4\]  Andre Maranho, Sanchita Bhadra, Inyup Paik, David Walker, and Andrew D. Ellington. 2020.  
      An improved and readily available version of Bst DNA Polymerase for LAMP, and applications  
      to COVID-19 diagnostics. \(oct 2020\). [https://doi.org/10.1101/2020.10.02.20203356](https://doi.org/10.1101/2020.10.02.20203356)  
  
**We can change this ourselves to achieve the desired appearance.  
Our understanding is that the publisher will not be retaining LaTeX-based styles, however.**

### Desired Appearance

We would like to see the priority \(● - ●●●\) prefixed prior to the reference's author\(s\) field.  
Additionally, we ask that the highlight bullets _not_ make use of a circular item label, for clarity.  
An alternative shape, such as a diamond or square, would assist in providing contrast:

\[4\]  ●  Andre Maranho, Sanchita Bhadra, Inyup Paik, David Walker, and Andrew D. Ellington. 2020.  
           An improved and readily available version of Bst DNA Polymerase for LAMP, and applications  
           to COVID-19 diagnostics. \(oct 2020\). [https://doi.org/10.1101/2020.10.02.20203356](https://doi.org/10.1101/2020.10.02.20203356)  
  
             ◇ Protein engineering fusion improves function of Bst DNA polymerase in  LAMP  
             ◇ Modifying Bst DNA polymerase significantly improves reverse transcriptase activity   
             ◇ Further improves LAMP-OSD detection in pre-heated saliva without RNA extraction

### Fallback Appearance

* If the [desired appearance](./#desired-appearance) is not possible:
  * Styles closer to the Current Opinions style are acceptable to us.
  * These styles are well-suited to flowing prose annotations.
  * They do not meld well with itemized, highlight-style annotations, however.
* What Changes
  * These styles place the priority marker inline with the first line of annotation text.

\[4\] Andre Maranho, Sanchita Bhadra, Inyup Paik, David Walker, and Andrew D. Ellington. 2020.  
     An improved and readily available version of Bst DNA Polymerase for LAMP, and applications  
     to COVID-19 diagnostics. \(oct 2020\). [https://doi.org/10.1101/2020.10.02.20203356](https://doi.org/10.1101/2020.10.02.20203356)  
  
             ● Protein engineering fusion improves function of Bst DNA polymerase in  LAMP  
                 Modifying Bst DNA polymerase significantly improves reverse transcriptase activity   
                 Further improves LAMP-OSD detection in pre-heated saliva without RNA extraction

