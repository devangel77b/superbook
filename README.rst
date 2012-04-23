2012/02/18

Shifted to Tufte-book.  Had to take out chapter bibliographies to do it.  This changes how the thing is compiled now - actually makes it easier.  

1.  Run pdfLaTeX on main.tex
2.  Run bibtex on main.tex
3.  Run pdfLaTeX twice. 
4.  Run make index on main.tex
5.  Run pdfLaTeX twice. 

***All references for a particular chapter must be added to the main bibliography file, now in references/main.bib. 

Still to-do: Make exercises be in a format that can easily be made into exams; add cute photos and quotes for each chapter? 




2012/02/10

Revision control and syncing using Mercurial
1. After making edits, commit your changes using:  hg commit -m "Enter a useful comment here."
2. To push your changes to the repository, use: hg push
3. To pull changes from the repository, use: hg pull, then hg update
4. To clone the repository using ssh, for example:
hg clone ssh:\\hg@bitbucket.org\devangel77b\superbook





Revision control block on top of tex file
Do not edit this.  After committing changes (hg commit -m "Made some changes"), update the block using the following:
1.  hg kwshrink
2.  hg kwexpand

Authors should have their usernames registered in main.tex



