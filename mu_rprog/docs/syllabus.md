---
output: pdf_document
linkcolor: blue
urlcolor: blue
---

\textbf{ECON 6931} \hspace{30mm}
\textbf{Introduction to R Programming} \hspace{30mm}
\textbf{Spring 2017}

\hrulefill

\textbf{Instructor:} James Lamb - james.lamb@marquette.edu | [Twitter](https://twitter.com/_jameslamb) | [LinkedIn](https://www.linkedin.com/in/jameslamb1) | [GitHub](https://github.com/jameslamb)

\hrulefill

\section{I. Course Info}

Welcome to R Programming! In this course, we'll explore the basic building blocks of statistical programming in R. My hope is that by the end, you will be able to use R code to turn your ideas into scripts, packages, and applications.

\subsection{A. Course Resources}

**Your Professor:**

My contact information is given at the top of this syllabus. Email is my preferred mode of contact, and I will do my best to respond to all emails within 48 hours.

I will be on campus at least an hour before class on the days we meet, and will host "office hours" at a location TBD. I will clarify office hour details during our first session.

**Course Repo:**

All course resources (including this syllabus!) can be found at https://github.com/jameslamb/teaching/tree/master/mu_rprog.

**Required Texbooks:**

None :)

**Required Hardware:**

\textcolor{red}{You are required to bring your own laptop to class.} If you do not have a personal laptop, please tell me as soon as possible and we can make other arrangements.

The use of personal hardware is required because one of my objectives for this course is to help each of you set up a data science friendly environment on your own machines. While the course is called "Introduction to R Programming", my hope is that you'll also get some hands-on experience working with an open-source data science stack.

**Required Software:**

We will be working with the [R programming language](https://www.r-project.org/). For script editing and exploratory analysis, we'll use [RStudio](https://www.rstudio.com/), a very popular integrated development environment (IDE) for R. For working with other text files, such as READMEs and JSON data downlaoded from the web, you can use any text editor. I personally prefer [Sublime Text](http://www.sublimetext.com/3). For managing source code and backing up coursework on the web, we'll use Git(https://git-scm.com/) and GitHub(https://github.com/).

Instructions for setting up all of these components can be found in the section below. Download and installation instructions are given in this syllabus, but we will also spend some time on the first day of class ensuring that everyone is set up.

**Slides and Assignment Rubrics:**

Slides and assignment rubrics will be available both in the "Content" section of the course page on D2L and on the course [GitHub repository](https://github.com/jameslamb/teaching/tree/master/mu_rprog).

\subsection{B. To-Do Before the First Session}

The course begins on 1/14/2017. Before class on that date, please do the following:

**1. Take the pre-course survey on [d2l](https://d2l.mu.edu/)**

The survey must be completed before the first day of class. This is just to help me understand the class's previous experience with programming and data science. This assignment does contribute to your grade; you will get a 100% for completing it.

**2. Try to set up your development environment (i.e. "install a bunch of stuff")**

I'll devote some time in the first class to ensuring everyone is set up and resolving any lingering issues, so don't stress if you can't figure these out. I'm including the links here just to give you a chance to get a head start.

- Try to [install RStudio v1.0](https://www.rstudio.com/products/rstudio/download/) or higher on your personal laptop
- Try to [install R v3.3.2](https://cloud.r-project.org/) or higher on your personal laptop
- Try to [install Sublime Text 3](http://www.sublimetext.com/3)
- Try to [install Git](https://git-scm.com/downloads)
- Set up a free account on [GitHub](https://github.com/)

I hope you'll be able to install these components using the information at those links and some moderate Googling. If you run into any issues, please email me and I'll help you out.

\subsection{C. Course Outline}

The (tentative) outline below describes my goals for each lecture. Assignment due dates and lecture dates are fixed but content may change as the class progresses.

\underline{Week 1: January 14, 2017}

Due before class: Pre-course survey

\begin{itemize}
    \item Introductions
    \item Brief syllabus review
    \item Environment setup
    \item What is R?
    \item Variables, namespaces, objects, and types
    \item What is functional programming?
    \item Basic math operations in R
    \item Controlling program flow: if-then, for, and while
    \item Introduction to data frames
    \item Introduction to version control: Git and GitHub
\end{itemize}

\underline{Week 2: January 21, 2017}

Due before class: Quiz 1

\begin{itemize}
    \item Using External Packages
    \item Fitting Regressions in R
    \item Subsetting
    \item Working with Files
    \item Introduction to data.table
    \item User-Defined Functions
    \item Debugging Strategies
\end{itemize}

\underline{Week 3: January 28, 2017}

Due before class: Quiz 2, Programming Assignment 1

\begin{itemize}
    \item Getting data from databases
    \item Working with web APIs
    \item Dealing with missing data
    \item Visualization with R's base plotting system
    \item Visualization with external packages (ggplot2, rbokeh)
    \item More data.table
    \item Final Project Discussion
\end{itemize}

\underline{Week 4: February 4, 2017}

Due before class: Programming Assignment 2, Final Project Proposal

\begin{itemize}
    \item Introduction to regular expressions
    \item Review of weeks 1-3
    \item Discussion of project proposals
\end{itemize}

\underline{Week 5: February 11, 2017}

Due before class: Final Project script + report

In class: Final Project code review

\begin{itemize}
    \item Final project presentations
    \item Intermediate R: functional programming
    \item Intermediate R: wrapping your code in a package
    \item Strategies for speeding up R code
\end{itemize}

\section{II. Grading and Assignments}

You will receive a letter grade for this course. Grades will be assigned using the following scheme (also available under the "Grades" section of the course D2L page).

|                                |Proportion of Final Grade |
|:------------------------------:|:------------------------:|
|Pre-Class Quiz                  |5\%                       |
|Quiz 1                          |10\%                      |
|Quiz 2                          |10\%                      |
|Programming Assignment 1        |15\%                      |
|Programming Assignment 2        |15\%                      |
|Final Project - Proposal        |10\%                      |
|Final Project - R script        |20\%                      |
|Final Project - Code Review     |10\%                      |
|Final Project - Written Report  |5\%                       |

And letter grades will be assigned using the following scale:

> \textbf{A}  - 92\% or higher \newline
> \textbf{AB} - 87\% $\leq$ grade < 92\% \newline
> \textbf{B}  - 82\% $\leq$ grade < 87\% \newline
> \textbf{BC} - 75\% $\leq$ grade < 82\% \newline
> \textbf{C}  - 70\% $\leq$ grade < 75\% \newline
> \textbf{F}  - Less than 70\%


\subsection{A. Quizzes (25\%)}

There will be two quizzes which will test your mastery of topics covered in class. These quizzes will test your knowledge of terminology and core concepts. In addition, quizzes may require you to interpret pseudo-code or to write a bit of R code yourself to solve questions.

Quizzes will be delivered online via D2L (see the "Quizzes" section of the course site) and you are expected to complete them outside of class. Quizzes have no time limit. You will be allowed two attempts for each quiz and your grade on each quiz will be the better of your two scores.

|Quiz                       |Opens                       |Due                           |
|:-------------------------:|:--------------------------:|:----------------------------:|
|Pre-class survey           | Immediately                | Prior to class on January 14 |
|Quiz 1                     | After class on January 14  | Prior to class on January 21 |
|Quiz 2                     | After class on January 21  | Prior to class on January 28 |


\subsection{B. Programming Assignments (30\%)}

After we've covered preliminary topics in the first two weeks of the course, I'll ask you to complete two programming assignments. In these assignments, you'll write moderate-sized R scripts to accomplish common tasks in data exploration and statistical analysis. 

Assignment rubrics can be found under the "Programming Assignments" module in the "Content" section of the course D2L page.

Your completed assignment must be uploaded to the appropriate folder in the "Dropbox" section on the course D2L page by the due date listed in the table below.

|Assignment                 |Description Available       |Due                           |
|:-------------------------:|:--------------------------:|:----------------------------:|
|Programming Assignment 1   | Immediately                | Prior to class on January 28 |
|Programming Assignment 2   | Immediately                | Prior to class on February 4 | 

\subsection{C. Final Project (45\%)}

Unlike the quizzes and programming assignments, the final project will be relatively unstructured. In this project, you will be asked to augment what you've learned about base R with other functionality available in external packages. You will be responsible for building an end-to-end analysis in R...a script that gets/cleans real world data, creates some exploratory plots, executes some statistical analysis, and stores the results to a file for later re-use.

The project comprises four parts:

\begin{enumerate}
    \item \emph{Final project proposoal}: A 1-2 page briefing on your planned project
    \item \emph{Final project script}: The R script/scripts supporting your project
    \item \emph{Final project report}: A 2-4 page report detailing the outcome of your analysis
    \item \emph{Final project code review}: You will give a 3-5 minute review of your project and code on the final day of class.
\end{enumerate}

Full details of the project and each of its components are available in the "Final Project" module in the "Content" section of the course D2L page.

|Assignment                      |Description Available       |Due                            |
|:------------------------------:|:--------------------------:|:-----------------------------:|
|Final Project proposal          | After class on January 14  | Prior to class on February 4  |
|Final Project (script + report) | After class on January 14  | Prior to class on February 11 |
|Final Project code review       | After class on January 14  | In class on February 11       |

\section{III. Administrative Information}

\subsection{A. Special Needs}

Please inform me during the first week of class if you have any conditions that may limit or affect your ability to participate in this course so that we can make necessary arrangements.  You may also contact the Office of Student Disability Services (OSES), in Marquette Hall 005 (8-1645) for more information (see also: http://www.marquette.edu/disability-services/).

\subsection{B. Emergency Plan}

Every Marquette University campus building has emergency shelter and evacuation plans. Please familiarize yourself with the plans of each building in which you take classes or attend meetings. Make sure to note the routes to the lowest level of the buildings for shelter during inclement weather, as well as exits from the buildings in the event of fire or other emergency.

\subsection{C. Attendance Statement}

The Marquette University Graduate School of Management considers regular class attendance an important component of the learning process. Students are expected to attend scheduled class meetings; excessive absences may have adverse consequences, ranging from a lowered course grade to forced withdrawal from the course. Excessive absence is generally defined as missing more than 10-15 percent of the regularly scheduled class time. Please consult \textbf{\emph{the instructor's course syllabus for additional details regarding a particular course}}.  

For this course, anything more than 1 class period is determined to be "excessive". Because this is a short (5-week) course, missing even one week will make it difficult to learn the material and satisfactorily complete the course requirements. If you miss more than one class, your grade will be reduced by a full letter grade for each absence after the first. All students are expected to complete all quizzes, assignments, and the final project.

\subsection{D. College of Business Administration Assessment Statement}

The fundamental mission of the College of Business Administration is to provide a quality education grounded in Catholic, Jesuit intellectual values.  Students are expected to learn how to function effectively in a diverse and global economy and develop into responsible members of the business community.  As one of many methods of assuring that the goals of our educational mission are successfully met, the college regularly and systematically engages in the assessment of these competencies.

Students in the Bachelor of Science in Business Administration program are assessed on their ability to reason ethically, communicate effectively, analyze critically, and understand local, national and global business and cultural issues.   Students in our MBA programs are also assessed on their competency to communicate effectively, reason ethically and apply critical thinking, as well as their capacity to comprehend the global strategic issues of firms and perform fundamental activities of business managers.  Students in our other graduate programs are assessed on specific competencies related to their disciplines.

Assessment takes place each semester in all programs and settings using quantifiable measures to gather and analyze information to help continuously improve the educational process.  The College of Business Administration is dedicated to successfully providing a quality education for all students.  Assessment is the continuous improvement process of evaluating our success.  More information on assessment can be found at http://www.marquette.edu/assessment/ or in the assurance of learning tabs under http://business.marquette.edu/academics/assurance-of-learning-undergrad or http://business.marquette.edu/academics/assurance-of-learning-graduate.

\subsection{E. Academic Integrity}

Don't cheat. For more see http://www.marquette.edu/provost/integrity-pledge.php.
