---
title: Scientific programming languages
subtitle: About scientific programming languages.

# Summary for listings and search engines
summary: What is “programming languages

# Link this post with a project
projects: []

# Date published
date: '2022-05-24T00:00:00Z'

# Date updated
lastmod: '2022-05-24T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin
 

tags:
  - Academic


categories:
  - Demo

---
## Scientific Programming Languages and Environments.
As computers become more ubiquitous in physics research (and scientific research in general), the issue of which programming languages to use becomes more important. Factors which especially influence the importance of this question are

    the increasing complexity of the tasks being programmed;
    the increasing complexity and diversity of the machines being programmed;
    the increasing use of graphical visualization and interfacing to scientific programs; and
    the increasing number of the programming languages available in which to program. 
    
    C and C++
C is an interesting choice as a scientific language. It is extremely flexible and available on about every machine known to man. Also, one of the best C compilers (gcc) is available for free. Almost all visualization and user-interface packages support the C language. C is frequently taught as a first or second language in university computer-science departments.

A long-standing gripe about C is that it produces slower code than does the equivalent Fortran. Nowadays, computer speeds are doubling every year or so, and C compilers don't seem to be doing that bad compared to Fortran anymore (typical C code runs between 50 and 100% as fast as the equivalent Fortran, depending on the application). In light of this, I think it's hard to discard C on the basis of the speed of the code it produces.

Nevertheless, I don't think it's a good scientific programming language. The C language is fairly close to the hardware, and it is quite easy to make big mistakes in coding an application. These mistakes often don't display themselves in small test cases, since they involve memory-management issues and the like. Also, programming large applications in C requires some degree of professionalism, meaning a fairly deep grasp of the language. As such, it is a bad language for mainstream scientific programming; typically only the creator of a program, or people with real expertise in computer programming, will be able to understand a large C application unless it is very carefully written.

I believe these comments also apply to C++ coding. The concerns about readability and professionalism apply perhaps even more strongly here than for "just C". C++ has the advantage of being the most-popular object-oriented language, but it is also recognized as being a fairly cryptic one. Again, a certain degree of professionalism is necessary to program a C++ application which is understandable to others. Packages which automatically generate C++ code from user-specified pseudocode help alleviate the problem, but then we are faced with asking all users to use the same C++ generator, which is another problem of the same magnitude.

The above two are the "traditional" choices. I now turn to newer languages which are less well known in the scientific community.
Python
Python is an object-oriented, extensible, interpreted language. It runs on essentially all Unix systems, as well as on DOS/Windows platforms and on the Mac. It is free and comes with complete source code. It is very easy to begin using Python --- at a simple level, it resembles Basic and can be used interactively in the same way as Basic. However, it supports object methods and "scales" nicely. Scaling indicates the relative difficulty of writing small vs. large applications. The object facilities help and encourage one to write an application in small pieces. These small pieces can be put together to make the big program, and the small pieces can also be used in other applications.

Another advantage of Python is its extensibility. One can write an object library in C, C++, or native Python, which can then either be dynamically or statically linked with the main Python system and used in Python programs. One can use this to make a programmable application, such as a data-plotting package. One would add a package to the interpreter which contained commands to set up your plots and to actually plot the data. This Python+graphics interpreter can be given a different name, such as "pygraph", and invoked as a command. The interpreter will process the graphics commands and perform them. However, at the same time you can use any other valid Python command as a command to this graphics program! Thus one graphics input file for this program could first compute the result and then manipulate and plot it.

The leap from this to having Python+package systems such as data-analysis programs, or experiment-control programs, is fairly obvious. This can also solve to some extent the above-mentioned dilemma about the use of C++. A professional programmer can produce a well-defined library package with a well-defined interface in C++, and this can be included into the Python programs for use. As Python is quite readable in much the same was as is Fortran, a "normal person" (i.e. someone who is not a professional programmer) can use this library in his programs. Both the professionals, who want the power and efficiency of C or C++, as well as the group who must use the result and be able to read and understand the program, can be happy. 
