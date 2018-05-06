---
title: Q-Step Essay submission
---

In Hilary Term 2018, I wrote an essay as part of my studies at university. This
essay is 

> expected to provide an empirical
answer to one of the three questions listed below that deal with Lijphart’s regime type
classification and its consequences:

> 1. Does consensus democracy reduce social inequality?
  2. Does consensus democracy improve economic outcomes?
  3. Does consensus democracy improve the quality of government?

I chose the first question, "Does consensus democracy reduce social inequality?"
I used an R notebook to do my scratch work and preliminary data exploration,
then wrote the essay in Markdown and used pandoc to compile it into
[essay.pdf](/essay.pdf).

I also knit the notebook into [HTML](/qstep_data_analysis.nb.html) and exported
it to [pdf](/qstep_data_analysis.pdf). The reason why I couldn't export it
directly to PDF is because that process gets rid of the code highlighting and I
couldn't find a way to fix that.

Lastly, I stapled the two PDFs together into the [final
essay](/qstep_essay_final.pdf).

# Things to take note
I commented out the first line `install-packages` but you may have to uncomment
it to install the requisite packages.

The command I used for pandoc was something like

```bash
pandoc --filter pandoc-citeproc -V papersize:a4 essay.md -o essay.pdf
```

which runs the Markdown file through the `pandoc-citeproc` filter and replaces
my references smartly.

# Things I learned

I learned about R. At my level, R isn't really programming, you just Google for
the right library or function that does exactly what you want to do. It is the
epitome of "library whacking". I would like to learn how to write custom
functions in R.

I learned a bit of statistical knowledge: what is Cronbach's alpha, what is
R-squared, and so on. But only on a very surface level; I didn't bother going
into the maths, I merely Googled them perfunctorily and agak-agak read enough to
reference it in my essays.

More importantly, I learned a lot about workflow:

- I learned about how bibliographies work in \TeX documents.
- I now have a better understanding of how `pandoc` works and I don't think I will
be going back to Google Docs or writing \LaTeX by hand ever again.




