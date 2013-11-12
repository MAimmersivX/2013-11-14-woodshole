% Software Carpentry - Overview
  Woods Hole Scientific Community
% Software Carpentry Team
% November, 2013

## Copy This Lecture!
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<a rel="license" href="http://creativecommons.org/licenses/by/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/InteractiveResource" property="dct:title" rel="dct:type">Software Carpentry Overview</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://software-carpentry.net" property="cc:attributionName" rel="cc:attributionURL">Software Carpentry</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/3.0/deed.en_US">Creative Commons Attribution 3.0 Unported License</a>.

# More About Software Carpentry

## History

* Founded by Greg Wilson in 1998, teaching scientists how to use supercomputers at LANL.
* Open sourced materials 2004-present
* Currently funded by the Sloan Foundation and the Mozilla Foundation

## What We Teach

* Unix Command Line Interface (Shell)
* Version Control
* Python
* Testing

## What We *Actually* Teach

* A program is just another piece of lab equipment
* Programming is a human activity
* Little pieces loosely joined
* Let the computer repeat it
* Paranoia makes us productive
* Better algorithms beat better hardware

*How to THINK like a programmer*

## Who We Teach

<div align="center">
<table>
<tr>
<td><img src="swc-demographics/thumb-age.png" /></td>
<td><img src="swc-demographics/thumb-role.png" /></td>
</tr>
<tr>
<td><img src="swc-demographics/thumb-gender.png" /></td>
<td><img src="swc-demographics/thumb-platform.png" /></td>
</tr>
</table>
</div>

## Who We Are

* Will Trimble (Argonne)
* Ross Dickson (Dalhousie University) 
* Woods Hole Python Users Group
* volunteers
 
## Our Goals for You

### We will take you on a tour of:
>
* Managing and sharing Software, Data, and Manuscripts with Git
* Automating things with the shell
* Principles of Practical Programming with Python
* Scientific Computing with Python
* Gallery of plotting and mapping in Python (matplotlib and basemap)

# Some High-Level Advice

## Be fluent in multiple languages
<comment>
You speak multiple languages when interacting with a computer.
Choosing to use a new tool, library, or language can be similar to
learning a new language:
</comment>

>
+ There is a high initial startup cost as you learn vocabulary, grammar, and
idioms
<font color=blue>`sum(x*y for x,y in itertools.izip(x_vector, y_vector))`
</font color>
+ You will learn faster by observing and working with others who are more
skilled than you
+ But once you have gained some fluency, you will find yourself capable of
new things!

## Use domain specific languages and libraries to increase your expressivity

* Aim for languages and tools that allow you to express your models and
manage your data simply. 

## Make it work right first, make it fast later.

## Use REPL Environments for Development

**REPL (read-eval-print-loop)** environments tighten the coupling between
the code you write and the results you see, increasing productivity.

REPL                                        non-REPL
-------------------          -----------------------
Visual Basic                 Supercomputers
Command Line                 C
IPython and Python           C++
MATLAB                       Java
Mathematica                  Fortran
LISP



# Don't Repeat Yourself (or Others)

## Automate common actions by saving simple blocks of code into **scripts**


* A script is a set of commands organized into a single file
* The script is the basest unit of scientific programming, you should be
comfortable writing these whenever you want to save or otherwise document or
repeat your actions
* Use scripts to explore new ideas, they are easy to write and throw away
* **Don't repeat commands into your REPL, save them to a script**

## Refactor commonly used blocks of code into **functions**

* Eventually, you will find that your scripts have a lot of repeated code,
or that you are spending a lot of time adjusting parameters at the top of
the file
* Refactor out repeated code into **function calls** in your scripts and
implement the **function** either in the same file or a separate one
* Be comfortable with the calling and return syntax of your programming language
environment, whether it is bash or Python
* **Don't repeat code in scripts, refactor them to functions**

## Group commonly used functions into **libraries**

* If you have to write a lot of software functions,
consider designing and releasing a library so that
others do not have to share your misfortune
* Check that nobody else has implemented the functionality you need
* If something close exists, it may be worth adapting to your needs if the
project is of high quality and suitably licensed
* *Openly licensed non-commercial libraries tend to have a much longer effective
lifespan than unreleased codes*
* **Share your code with others, and use their code**

# Reduce Complexity

## Basic strategies

* Use languages and libraries that reduce the complexity of
your work
* It is worth installing a complicated or expensive software tool if your
computations or model are naturally expressed with it
* Always look for opportunities to write **less** code
    + you will have to do less initial work (sometimes)
    + you will introduce less bugs
    + your code will be easier to understand and maintain
* When writing software, try to keep individual functions short, single-purpose,
and avoid excessive nesting

## Back up your data!

## Use version control for checkpointing and collaboration

* use local version control software to checkpoint personal code development
  + checkpointing your work encourages wild ideas and late-night coding sessions
  + you can easily restore back in the morning if it was a bad idea
* use **distributed version control** to collaborate with others
* We advocate *Git*, but you may be stuck with whatever your group uses
  + though check out git-svn for using Git to collaborate with an svn repository,
  it's awesome!

*We will learn more about working with git and GitHub today*

# Verify and Validate your Code

## Principles of verification and validation
* **verification** - is your code correctly written?
* **validation** - do your computations accurately model the physical phenomena
in question?
* test frameworks help you verify your code, but validation is usually a manual
process
* Be paranoid and test small things!  

# Document your Computational Work

## Principles of documentation
* Save every bit of code you use for generating publishable results
* Document and comment your code for yourself as if you will need to understand
it in 6 months
  + use README files liberally
  + as well as file-level, function-level, and inline documentation
* If any piece of code is too complex to easily describe, consider refactoring
it


## Schedule 

### Today

* **9:00-12:00** Managing and Collaborating with your Software, Data,
and Manuscripts with Git
* **1:00-4:30** Debugging, testing, and numpy/pandas


# Closing Thoughts

## Aim for reproducibility
* The goals of non-review scientific publications are to:
    + Describe a new result or approach
    + Convince others of its usefulness
* The **reproducibility** of your publication will greatly benefit both of
these goals
* See <http://figshare.com> for an easy way to store and share your data in
an easily-cited way

# References and Further Reading

# Books

## Pragmatic Programmer, The: From Journeyman to Master
Andrew Hunt and David Thomas

ISBN 978-0132119177

*Describes the important principles and practices of being an effective
programmer, instead of teaching a specific language or technique*

## Code Complete Second Edition
Steve McConnell

ISBN 978-0735619678

*Focuses on principles of software construction, with attention to skills,
testing, and design.*

## Verification and Validation in Scientific Computing
William L. Oberkampf and Christopher J. Roy

ISBN 978-0521113601

*Focuses on verification and validation of numerical solutions to models
described by systems of partial differential and integral equations.*

# Research Literature

## Programming Languages for Scientiﬁc Computing
Matthew G. Knepley

Preprint: http://arxiv.org/pdf/1209.1711.pdf

*Gives an overview of modern programming languages and techniques such as code
generation, templates, and mixed-language designs. This is a preprint,
so expect some rough spots.*

## Two Solitudes
Greg Wilson

Slides: http://www.slideshare.net/gvwilson/two-solitudes

*Describes Greg's journey as a scientist and leader for the Software Carpentry
project, provides some insight into the differences between industry and
academics.*

## Best Practices for Scientific Computing
D. A. Aruliah, C. Titus Brown, Neil P. Chue Hong, Matt Davis, Richard T. Guy,
Steven H. D. Haddock, Katy Huff, Ian Mitchell, Mark Plumbley, Ben Waugh,
Ethan P. White, Greg Wilson, Paul Wilson

Preprint: http://arxiv.org/abs/1210.0530

*Good summary paper of many fundamental practices for working with and
developing scientific software. This is a preprint, so expect some rough spots.*

# Web References

## What Every Computer Scientist Should Know About Floating-Point Arithmetic
David Golberg

Web article: http://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html

*Introduction to the IEEE floating-point standard, its implications, and many of
the common pitfalls when using floating-point numbers in scientific computing*

## The Research Software Engineer
Rob Baxter, Neil Chue Hong, Dirk Gorissen, James Hetherington, and Ilian Todorov

Web article: http://dirkgorissen.com/2012/09/13/the-research-software-engineer

*Discussion of the current challenges to scientific software engineering as
a profession.*

## Science Code Manifesto

http://sciencecodemanifesto.org

*Publicly signed commitment to clear licensing and curation of software
associated with research publications.*

## You sometimes need geeks.  You never need dorks.
<div align="center">
<table>
<tr>
<td><img src="swc-demographics/careful.png" /></td>
</tr>
</table>
</div>
