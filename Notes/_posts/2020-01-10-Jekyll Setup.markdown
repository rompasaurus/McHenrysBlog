---
layout: post
title:  "Jekyll Setup Notes"
date:   2020-01-10 20:15:22 +0000
---

Below is the running documentation and notes taken along the way to setting up Jekyll and hosting it via github pages. Disclaimer: this post is a copypasta of the documentation notepad and it edit additions made along the way no formal revision established on this site.

### Overview:
I decided that my documentation should be formalized and available for view online.
I would like the processes and documentation behind creating a website to be a testament to my abilities as much as the site itself.
As such in beginning my new project The Thought Encyclopedia I would like to establish a static site as the repository of the thoughts, planning and steps taken to translate and idea into action.
My hope with this site will be provide useful information to anyyone in puruit of advancedmment in the field of web development along with a showcase to any future employers.

01/10/2020

### Steps to create this blog:

Begin research on jekyll deployment find the proper reseource to go from start to finishi in deploying a jekyll site and presenting content within.
Locate Jekyll templates and use case and determine best route of configuration
Determine what it will take to host jekyl either on azure or in github.

https://jekyllrb.com/docs/step-by-step/01-setup/

### Example sites:

https://blog.codingmilitia.com/2019/02/24/aspnet-016-from-zero-to-overkill-authentication-with-identity-and-razor-pages

### YAML:

The principle way that jekyle works is by translating yaml created content into distinct static html pages.
Yaml is unique in that it is a simplistic markup language that is easy to read and takes advatage of the tabular structure of typing and establish a format in which can be quickly writing and subsequently parsed into an html format.

Yaml sysntax will be an important concept to understand in begining to contribute well formatied conted to the jekyll applcaition

### Thoughts:

I love the idea of jeckyll and the simplicity of static pages however I would to reamin in the .net ecosystem instead of ruby and as such decided a different framework would be more appealing

### Wyam:

Seems the better alternative to jekyll to allow me to stay within the scope of the dotnet framework contining forward I will be using this as the template for my simple blog.

### Steps Taken to setup whyam on mac:

### install the wyam package via command:
	dotnet tool install -g Wyam.Tool
I am going to be using the prebuilt docs recipe for simplicity
### terminal:
	wyam new -r Docs

### Basic concept behind wyam :

Posts are established via .md mardownfiles setup within the input folder the wyam project
Each subfolder acts as a separate page.
Metadate for each page is establish via yaml headers created in each post
you establish your input files is a yaml format with notated as "front matter"

After a few hours of tinkering with wyam I decided not to use it, the documention is just there I am unable to properly host this site with the given static site that it generates

Resources:

Adding search to static pages using azure search:
https://hutchcodes.net/2016/12/azure-search-for-jekyll/
https://www.hanselman.com/blog/ExploringWyamANETStaticSiteContentGenerator.aspx
wyam.io

### About details quick draft:

My name is michael mchenry and 
I am an aspiring software and web developer. With over 10 years experience in the IT industry I have had the unique opportunity to work with numerous enterprise software and hardware systems starting out as tech support for Verizon internet cable and voice services for 2 years I eventually made my way to JP Morgan Chase and worked as an IT analyst tasked with the continued support and maintenance of the enterprise hardware and software used firm wide by all of JP Morgans employees 3 years of experience eventually lead me to a Top Secret cleared position working as a red hat server/software admin contracted through the department of defense,here I tasked with the 24/7 maintenance and monitoring of several communications servers located throughout the US ,I ensured continuous up time of all services and in the event of outages and system issues ensuring service continuity of operations by implementing redundancy measures to guarantee minimal service interruptions.

Since 2016 I have pursued continued advancement and learning in the fields of software development and web design and over the years have amassed an extensive portfolio of projects each with the expressed intent to advance my knowledge and experience in critical, cutting edges technology frameworks and methodologies. In 2019 I started a position in Guantanamo Bay Cuba and am currently employed as a software developer for a mission critical ASP.net web application. Here I ensure that the applications functionality stays current to the ever changing mission requirements, tailoring web front end workflows with intuitive layouts allowing for quick analysis and modification of pertinent data. Further I have performed back-end system performance improvements in MS SQL ensuring that the data is efficiently modeled, indexed and queried.

Looking forward it is my goal to continue down the path of software development within the cleared spaces of US government. I intend to continue to work and live in exotic locations, to contribute meaningfully to mission critical projects and to gain real world experience and knowledge in cutting edge technologies. 


## Quick Steps to setup Jekyll example instance from scratch:
### Step 1:
Download Ruby sdk version 2.6 from ruby.io and install
### Step 2:
open the ruby cli from the start menu and type the following commands"
	gem install jekyll bundler
pulls in all the jekyll packages and dependecies and includes it inot ruby sdk file listing
	jekyll new myblog
pull template blog setup with default configuration established by jekyll
	### note:
	blog files and folders will be created in the current directory specified in cmd prompt
	cd myblog
change directory to where the blog was created
	bundle exec jekyll serve
pulls in any remain dependencies need to run the default jekyll build and begins hosting site on localhost:4000 addres	
	### note: 
	upon adding pages to jeckyll folder structure, jekyll will automatically injest and route the page properly, however any change to the config.yml file will require a reinitialiez of jekyll and the server via 
	ctr-c x2 > jekyll serve command

### steps 3:
from here the about,index and post can be created and modified to orient what kind of contect you would like to see on the site.
further the config.yml file can be editied to establish global variables for the site such as the theme, site title and footer details.

01/15/2020			
### Blog:
Need to establish intros and outlines to each page 
specifically the throught encylcopedia page 

### Blog Progress:
Still getting a full understanding of jekyll, right now I'm trying to figure out how categories set via yaml and folder structure also ruby sytax and libraries are going to take a bit to fully ingrained but it will just be a matter of learn exatcly what I need to get things done.
to do: 
add 2-3 more posts to the site and find a way to eloquetly display categories

01/16/2020
### Progress:
Added eloquest categories to the title section of each post to show the the context of each post 
Adding further the overview to TE website projects
need to also find a suitable host for this site

### Deploy to github:
Deploying this site to github is relatively staright forward the main thing to remember is that the config.yml needs edited to account for the github url path and starting directories
guide followed:https://idratherbewriting.com/documentation-theme-jekyll/mydoc_publishing_github_pages.html#customize-your-url

