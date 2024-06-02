---
title: Documentation notes
teaching: 30
exercises: 30
questions:  
- References on documenting code
objectives:  
- Learn how do document procedures, python and C++
keypoints:
- This will be useful for a lot of projects
- It is also something almost all people who get paid to program are expected to know well
---

## useful links

<details>

<summary> General text formatting in Markdown

[Markdown Cheatsheet][Markdown Cheatsheet]

[Github markdown][Github markdown]

[Advanced github formatting][Advanced github formatting]

</details>

<details> 

<summary> Documenting complex python packages with sphinx and readthedocs

[sphinx][sphinx] is a documentation system for python code that can be used with [rst][rst] or with [Markdown][Markdown Cheatsheet]. You can set up github actions to build custom `<organization>.github.io` pages from repository `github.com/<organization>`.

Alternatively [readthedocs][readthedocs] is a semi-commercial system that uses sphinx/rst and provides the build infrastructure.  

</details>

### C++

[doxygen][doxygen]

{%include links.md%} 

[Markdown Guide]: https://www.markdownguide.org/

[Markdown Cheatsheet]: https://www.markdownguide.org/cheat-sheet/

[Github markdown]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/

[Github markdown spec]: https://github.github.com/gfm/

[Advanced github formatting]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/

[sphinx]: https://www.sphinx-doc.org/en/master/usage/index.html

[rst]: https://docutils.sourceforge.io/rst.html

[readthedocs]: https://about.readthedocs.com/?ref=readthedocs.com

[doxygen]: https://www.doxygen.nl