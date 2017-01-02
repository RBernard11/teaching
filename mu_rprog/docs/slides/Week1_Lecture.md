---
title       : ECON 6931 - R Programming
subtitle    : Week 1
author      : James Lamb
job         : Data Scientist | Uptake
logo        : 
framework   : io2012  # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz}
mode        : selfcontained # {selfcontained, standalone, draft}
lib_cdn     : "https://cdn.rawgit.com/ramnathv/slidifyLibraries/master/inst/libraries"
knit        : slidify::knit2slides
---

<script src="assets/js/footer_bubbles.js"></script>

<footer>
  <hr></hr>
  <span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2 class="content_slide">Welcome to Class!</h2>

I'm pumped for this.

<center><img src="./assets/img/you_gon_learn_today.jpg"></center>

--- .toc_slide &twocol

<footer>
  <hr></hr>
  <span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Contents</h2>

*** =left

<b class="toc_header"> I. Introduction to R </b>
<ol class="toc" type="none">
    <li> Personal Introduction <span style="float:right"> 5 </span></li>
    <li> Syllabus Review       <span style="float:right"> 6 </span></li>
    <li> Course Objectives     <span style="float:right"> 7 </span></li>
</ol>

<b class="toc_header"> II. Setting Up Your Environment </b>
<ol class = "toc" type="none">
    <li> Installing R + RStudio             <span style="float:right"> 9  </span></li>
    <li> Authoring Scripts in RStudio       <span style="float:right"> 10 </span></li>
    <li> Installing Sublime Text            <span style="float:right"> 12 </span></li>
    <li> Authoring Scripts in a Text Editor <span style="float:right"> 11 </span></li>
    <li> R from the Command Line            <span style="float:right"> 12 </span></li>
</ol>

*** =right

<b class="toc_header"> III. Introduction to R </b>
<ol class = "toc" type="none">
    <li> R is an interpreted language      <span style="float:right"> 14 </span></li>
    <li> R is dynamically typed language   <span style="float:right"> 14 </span></li>
    <li> R has a few of its own file types <span style="float:right"> 14 </span></li>
</ol>

<b class="toc_header"> IV. Programming Fundamentals </b>
<ol class = "toc" type="none">
    <li> Variables and Namespaces    <span style="float:right"> 15    </span></li>
    <li> Introduction to Types       <span style="float:right"> 15    </span></li>
    <li> Dollarstore Calculator Math <span style="float:right"> 16-18 </span></li>
    <li> Controlling Program Flow    <span style="float:right"> 19-20 </span></li>
</ol>

--- .toc_slide &twocol

<footer>
  <hr></hr>
  <span style="float:right"> ECON 6931 - R Programming </span>
</footer>

<h2>Contents</h2>

*** =left

<b class="toc_header"> V. Functions in R </b>
<ol class="toc" type="none">
    <li> Intro to Functional Programming <span style="float:right"> 22 </span></li>
    <li> Required and Default Arguments  <span style="float:right"> 22 </span></li>
    <li> Lexical Scoping                 <span style="float:right"> 23 </span></li>
    <li> Lexical Scoping (pt. 2)         <span style="float:right"> 24 </span></li>
    <li> Handling Errors                 <span style="float:right"> 24 </span></li>
    <li> User-Defined Functions          <span style="float:right"> 24 </span></li>
</ol>

<b class="toc_header"> VI. Common R Data Structures </b>
<ol class = "toc" type="none">
    <li> Vectors pt. 1     <span style="float:right"> 29-30 </span></li>
    <li> Lists pt. 1       <span style="float:right"> 31-32 </span></li>
    <li> Data Frames pt. 1 <span style="float:right"> 33-35 </span></li>
</ol>

*** =right

<b class="toc_header"> VII. Introduction to Version Control </b>
<ol class = "toc" type="none">
    <li> What is Git?                <span style="float:right"> 29-30 </span></li>
    <li> Setting Up Your Repo        <span style="float:right"> 31-32 </span></li>
    <li> Local vs. Remote Repos      <span style="float:right"> 33-35 </span></li>
    <li> Getting Started with GitHub <span style="float:right"> 33-35 </span></li>
</ol>

--- .section_slide

<h2>Section I.</h2>
<hr></hr>
</br></br></br>
<h2>Introduction</h2>

--- .content_slide

<footer>
  <hr>
    <script>FooterBubbles(1,7)</script>I. Introduction<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Personal Introduction</h2>

>- <b>My Marquette Experience:</b>
    - B.S., Economics & Marketing (2013)
    - M.S.A.E., Marketing Research Specialization (2014)
    
>- <b>Since Marquette:</b>
    - Data Scientist @ [Uptake](https://uptake.com/) in Chicago, IL 2016-Present
    - Analyst/Economist @ [Abbott Laboratories](http://www.abbott.com/) in North Chicago, IL 2015-2016
    - Analyst @ [IHS Economics](https://www.ihs.com/industry/economics-country-risk.html) in Lexington, MA 2014-2015
    - Completed 2 Coursera specializations: [JHU Data Science](https://www.coursera.org/specializations/jhu-data-science) | [UMich Python/Web](https://www.coursera.org/specializations/python)
    - Completed 20+ data science and computer science MOOCs
    - Co-wrote an EViews add-in to perform time-series cross validation. [GitHub repo](https://github.com/jameslamb/ML4EVIEWS) | [EV Blog](http://blog.eviews.com/2016/04/add-in-round-up-for-2016-q1.html)

--- .content_slide

<footer>
  <hr>
  <span>&#x25cf; &#x25cf; &#x25cf;&nbsp;I. Introduction</span><span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Economics in the Age of Big Data</h2>

**From [Einav & Levin (2014)](http://www.sciencemag.org/content/346/6210/1243089.full.pdf?keytype=ref&siteid=sci&ijkey=Jj7wCy7hhth4M):**

>- Economists increasingly using large data sets (private & administrative)
    > "Economic models bring a simplifying conceptual framework to to help make sense of large data sets"
    
>- A major challenge:
    > "...developing appropriate data management and programming capabilities, as well as designing creative 
    > and scalable approaches to summarize, describe, and analyze...data sets"

</br></br></br></br>
>- Other Commentary: [Einav (2013)](http://www.stanford.edu/~leinav/pubs/IPE2014.pdf) | [Varian (2013)](http://people.ischool.berkeley.edu/~hal/Papers/2013/BeyondBigDataPaperFINAL.pdf) | [Varian (2014)](http://people.ischool.berkeley.edu/~hal/Papers/2013/ml.pdf) | [Cagle (2014)](http://blogs.avalonconsult.com/blog/generic/ontology-for-fun-and-profit/)

--- .section_slide

<h2>Section II.</h2>
<hr></hr>
</br></br></br>
<h2>Setting Up Your Environment</h2>

--- .content_slide

<footer>
  <hr>
  <script>FooterBubbles(1,5)</script>II. Setting Up Your Environment<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Installing R + RStudio</h2>

text tbd

--- .content_slide 

<footer>
  <hr>
  <script>FooterBubbles(2,5)</script>II. Setting Up Your Environment<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Authoring Scripts in RStudio</h2>

text tbd

--- .content_slide 

<footer>
  <hr>
  <script>FooterBubbles(3,5)</script>II. Setting Up Your Environment<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Installing Sublime Text</h2>

text tbd

--- .content_slide 

<footer>
  <hr>
  <script>FooterBubbles(4,5)</script>II. Setting Up Your Environment<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>Authoring Scripts in a Text Editor</h2>

text tbd

--- .content_slide 

<footer>
  <hr>
  <script>FooterBubbles(5,5)</script>II. Setting Up Your Environment<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>R from the Command Line</h2>

text tbd

--- .section_slide

<h2>Section III.</h2>
<hr></hr>
</br></br></br>
<h2>Introduction to R</h2>

--- .content_slide

<footer>
  <hr>
  <script>FooterBubbles(1,3)</script>III. Introduction to R<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>R is an Interpreted Language</h2>

text tbd

--- .content_slide

<footer>
  <hr>
  <script>FooterBubbles(2,3)</script>III. Introduction to R<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>R is a Dynamically Typed Language</h2>

text tbd

--- .content_slide

<footer>
  <hr>
  <script>FooterBubbles(3,3)</script>III. Introduction to R<span style="float:right">ECON 6931 - R Programming</span>
</footer>

<h2>R has its own File Types</h2>

text tbd

--- .section_slide

<h2>Section IV.</h2>
<hr></hr>
</br></br></br>
<h2>Programming Fundamentals</h2>

text tbd

--- .section_slide

<h2>Section V.</h2>
<hr></hr>
</br></br></br>
<h2>Functions in R</h2>

text tbd

--- .section_slide

<h2>Section VI.</h2>
<hr></hr>
</br></br></br>
<h2>Common R Data Structures</h2>

text tbd

--- .section_slide

<h2>Section VII.</h2>
<hr></hr>
</br></br></br>
<h2>Introduction to Version Control</h2>

text tbd
