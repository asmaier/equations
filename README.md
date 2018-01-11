# Equations of fluid dynamics
 An experiment in the conversion of LaTeX to HTML. The HTML output can be seen at

 - http(s)://asmaier.github.io/equations


## Usage
To convert the LaTeX source you need to install [LaTeXML](http://dlmf.nist.gov/LaTeXML/). On Mac OS X do

    brew install latexml

To convert the latex source file `equations.tex` to the `index.html` output file do

    latexml equations.tex --dest=equations.xml
    latexmlpost --format=html5 --javascript='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=MML_CHTML' --dest=index.html equations.xml

If you have github pages (https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/) enabled for the master branch 
the `index.html` file will be automatically served at `http(s)://<username>.github.io/<projectname>`. 
    
