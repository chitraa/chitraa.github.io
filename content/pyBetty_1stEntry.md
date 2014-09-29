Title: The beginning of Alex
Date: 2014-09-30 00:15
Category: Alex
Tags: opensource, pelican, python, NLP
Slug: beginning-of-alex
Author: Me
Summary: A command line tool for natural language commands

As a part of a course _Architecture of Open Source Technologies_ offered by [Dr Ram P Rustagi](<mailto:user@example.com>), at PESIT, Bangalore, two of my batchmates, [Anushree Prasanna Kumar](<anushree.apk@gmail.com>), [Pratheek M S](<pratheekonline@gmail.com>) and [I](<chits.26@gmail.com>) are doing an open-source project which is named [__Alex__](https://github.com/pratheekms/alex) for now.


###What is open-source code ?

According to Wikipedia, [open-source software](http://en.wikipedia.org/wiki/Open-source_software) (OSS) is computer software with its source code made available with a license in which the copyright holder provides the rights to study, change and distribute the software to anyone and for any purpose. 


###Why open-source the code?

1. I believe if the community is active and maintains the code properly, the code itself gets __crowd tested__, eliminating the need for software testing (Companies spend quite a lot on hiring people who test the code at various stages).
2. While attending some talks in and around Bangalore, people threw some light on how __fast prototyping__ is, i.e. building upon things. Building from scratch moves the main focus from what you actually want to achieve. I'm using [Pelican](https://github.com/getpelican/pelican) myself, an open source static site generator, written in Python, for creating this blog. It was fast and simple, and I could directly focus on writing this blog, in markdown.
3. The entire world can read the code, understand, __gain inspiration__ from the architectures of various famous frameworks to create new content. [This book](http://aosabook.org/en/index.html) shows various examples of open source applications. As quoted in the aosabook -
> Architects look at thousands of buildings during their training, and study critiques of those buildings written by masters. In contrast, most software developers only ever get to know a handful of large programs well—usually programs they wrote themselves—and never study the great programs of history. As a result, they repeat one another's mistakes rather than building on one another's successes. 

###Inspiration
Our inspiration came from a famous open-source project [___Betty___](https://github.com/pickhardt/betty), a friendly English-like interface for your command line. We're being taught [Natural Language Processing](http://nlp-course.appspot.com/lectures.html#) by Prof Anantharaman Narayana, and have realized that there is a lot of potential in improvising the current product with our gained knowledge.

Betty is like [Siri](http://en.wikipedia.org/wiki/Siri) or [Google Now](http://en.wikipedia.org/wiki/Google_Now) for the [__command line__](http://en.wikipedia.org/wiki/Command-line_interface). The tool translates plain English into commands, and displays the command it runs and the command output, in the terminal. The current codebase of Betty is written in Ruby. 

###Now what is Natural Language Processing?
Again Wikipedia says, [Natural Language Processing](http://en.wikipedia.org/wiki/Natural_language_processing) (NLP) is a field of computer science, artificial intelligence, and linguistics concerned with the interactions between computers and human (natural) languages.

It deals with analyzing, understanding and generating the languages that humans use naturally in order to interface with computers in both written and spoken contexts using natural human languages instead of computer languages. 





###Roadmap

####We have decided to start with our own version in _Python_ mainly because:
 - All of us are more proficient in Python. But hey! We're engineering students, still learning, it's not hard for all of us to pick up another scripting language like Ruby. But we got more reasons to counter with. 
 - Python mostly comes preintalled in most of the linux/mac distros.
 - The [NLTK](http://en.wikipedia.org/wiki/Natural_Language_Toolkit) python libraries are used by a large number of people. It has very efficiently written modules, and has a lot of community support online. 
 - Building the pyBetty/Alex from scratch gives us a lot of flexibility, in twisting the code from our point of view, while taking a lot of inspiration from the actual Betty project. Some of the vulnerabilities where we think we can improve are : 
	- Preprocessing, tokenizing (stem and lemmatize) the sentences instead of directly mapping some group of sentences.
	- Try to infer the semantic meaning of sentences. (Intelligent information retrieval)
	- Initial task will be trying to think of all the different natural language command line statements people can make. We can then do some NLP techniques (such as Language Models, Wordnet look ups etc or even use some Machine learning techniques) to get a good implementation. All this starting with one example command.

####In software engineering terms, we plan to follow an [Agile](http://en.wikipedia.org/wiki/Agile_software_development) model, whereby there are
1. _Individuals and interactions_ over Processes and tools
2. _Working software_ over Comprehensive documentation
3. _Customer collaboration_ over Contract negotiation
4. _Responding to change_ over Following a plan



####Why will all cool geeks accustomed to using the terminal interface use this tool?
This can be used by beginners to command the computer in simple english words, instead of using man pages or googling for small-small things. I agree, lots of useful commands can be aliased and put into .bashrc, but natural language commands are always more intuitive. 
For example, long text processing commands(using sed/grep/tr) are always a pain. Simple english words will save time.

###Challenges?
A lot. Most of the problems in this domain are __open problems__, and don't have the exact solution. Lot of __ambiguities__ arise when we try to extract the semantic meaning from sentences. Moreover, some methods may require a lot of _computations_, which might slow down the process. With lesser computations, the _accuracy_ might reduce. We need to find a proper balance between them.



###List of open source tools used :
1. [Sublime Text](http://www.sublimetext.com/), an amazing text editor, with the [markdown](https://github.com/revolunet/sublimetext-markdown-preview) plugin.
2. Python Language (CPython, the reference implementation of Python is free and open-source software)
3. [Pelican](https://github.com/getpelican/pelican), a static site generator, written in Python.
4. [Bootstrap3](http://getbootstrap.com/), a framework for developing responsive, mobile first projects on the web.
5. [Git](http://git-scm.com/), version control system.
6. [Github pages](https://pages.github.com/) to host the blog free of cost :D