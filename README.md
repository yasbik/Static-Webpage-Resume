# Readme

## `Purpose`
This readme is a description of how format a resume with Markdown and host it on GitHub with the help of Jekyll and GitHub Pages.
All of this also relates to the general principles of current Technical Writing, as explained in Andrew Etter's book Modern Technical Writing.
Given below is a sample of a resume formatted in Markdown.

## `Markdown Formatted Resume `

    # Abu Yasin Sabik
    90 Brotman Bay, Winnipeg, MB R2N 2P1  
    +1 (431) 996-6939 | yasin00sabik@gmail.com

    ---

    # Education

    ### **Bachelor of Science (B.Sc.) in Computer Science**  
    ***University of Manitoba***   
    January 2019 - Present (Ongoing)  
    Expected Date of Gratuation: May 2022

    Relevant Coursework:
    * Object Oriented Programming
    * Software Engineering
    * Database Management
    * Human Computer Interaction
    * Operating Systems

    ---

    # Technical Skills

    |  |  |
    | --- | --- |
    | Programming Languages | HTML/CSS, Javascript, Java, Python, C/C++, SQL, System Tap |
    | Database Management | MySQL, Sqlite3, Neo4J |
    | Tools/Technologies | Git/Github, MySQL, Sqlite3, Neo4J, Android Studio, Vim, VMware, VS Code, IntelliJ, MS Office Suite/Office365 |
    | Operating Systems | Windows, MacOS, Unix, Linux |

    ---

    # Projects

    ### **Ixalan** - *An Android Application for booking movie tickets*

    * A mobile application for booking movie tickets and purchasing movie merchandise. The project follows software engineering principles, agile development, and very thorough testing. A static website was also built for marketing and exposure of the product.  

    * Technology/Tools/Software used: Android Studio, Java, HTML/CSS, Junit, Mockito

    ### **Chowtown** - *A Website for ordering food*

    * A food ordering website which focuses heavily in UI/UX and implements innovative ideas to ensure better handling and navigation for all sorts of users.

    * Technology/Tools/Software used: HTML/CSS, Javascript, ReactJS

    ---

    # Work Experience 

    ### **STEM Tutor** - *Paper*  
    Montreal, QC  
    July 2021 - Present

    * Manage tutoring sessions with multiple students (simultaneously) in STEM subjects.
    * Conduct pedagogical assessments, and provide=ing feedback to teachers and students.

    ### **Fitness Motivator** - *GoodLife Fitness*  
    Winnipeg, MB  
    August 2019 - December 2020

    * Assisting club members with enquiries, complaints, and services.
    * Overseeing front desk operations.

    ### **General Crew** - *McDonald's Canada*  
    Winnipeg, MB  
    April 2018 - December 2019

    * Handling drive-thru and in-store sales.
    * Providing customer service.

    ### **Marketing Assistant** - *Qdoba Mexican Eats*  
    Winnipeg, MB  
    July 2018 - June 2019

    * Running local marketing campaigns and promotions.
    * Making cold calls and sample out products to create new business.
    * Carrying out market research and create reports/tracking sheets for future reference and opportunities.

    ### **Teaching Assistant** - *Edbridge*  
    Dhaka, Bangladesh  
    July 2014 - June 2017

    * Taking physics and higher-level math classes of grades 9-10.
    * Grading papers, evaluate coursework, create worksheets.

    ---
 
---
# Instructions on creating and hosting the resume

## `1. Creating the resume with a Lightweight Markup Language`

The first step is to create the actual resume and format it using a Lightweight Markup Language.
In his book Modern Technical Writing, Andrew Etter recommends using Markdown to do this. 
He states that it is the most widely used lightweight markup language in the world. 
This is beacause compared to other markup languages, Markdown is very simple, human-readable, and easy to learn. 

Markdown is also available in several variants/flavours and for the purpose of this task, we will use a [GitHub Flavoured Markdown](https://github.github.com/gfm/) 
to ensure that is gets properly rendered in Github Pages.

Some Markdown features/syntaxes are demonstrated below as an example:

- A "#" followed by a space can be added to the beginning of a line to indicate that it is a heading. 
Using a single "#" formats the sentence as the biggest heading (called heading1). 
Adding more "#"s create smaller headings ("##" formats it as heading2, "###" formats it as heading 3, and so on until heading6).
Given below is an example:

    >"## Resume of Abu Yasin Sabik" produces
    > ## Resume of Abu Yasin Sabik

- Text can be formatted by wrapping them with special characters. Wrapping a text with a single "\*"  formats it in *italics*. 
Wrapping it with "\*\*" formats the text in **bold**.
Given below are two examples:

    >"\*Relevant Skills\*" formats the text as *Relevant Skills*.  
    >"\*Relevant Skills\*" formats the text as **Relevant Skills**.

- Bullet points can be created using "-". For example:
    >"- Providing customer service" produces
    >- Providing customer service

Although there are many specialized text editors for markdown, Etter suggests the following three, based on the operating system:

- [MarkdownPad](http://www.markdownpad.com/) (Windows)
- [iAWriter](https://ia.net/writer) (macOS)
- [ReText](https://sourceforge.net/directory/development/wordprocessors/os:windows/) (Linux)


## `2. Uploading the resume to GitHub`

The next step is to upload the markdown formatted resume to a distributed version control system (DVCS) such as Git or Mercurial. Etter highly emphasizes using DVCS over centralized systems because they have better performance, allow for offline work, and are superior for concurrent work on the same file. Etter quotes, "For technical writers, the most important reason to use DVCS is that develops prefer them.

For the purpose of this task, we will be using [GitHub](https://github.com/). It is an open-source software and its version control system allows for seamless collaboration without compromising the integrity of the original progect.

To use Github, we would first need to create an account. The steps to do this is given below, along with other steps to complete uploading the resume:

1. Download and install [Git](https://git-scm.com/) using this [link](https://github.com/git-guides/install-git#:~:text=To%20install%20Git%2C%20run%20the,installation%20by%20typing%3A%20git%20version%20.) and following the steps outlined.
2. Create a GitHub account but following this [link](https://github.com/) and clicking on the "Sign up" button on the top right corner. Follow the instructions to then create an account for yourself.
3. [Create a new repository](https://guides.github.com/activities/hello-world/) by loggin in and clicking the green "New" button  on the"Repositories" section. Name your repository using "\<YourUsername>.github.io". Finally, click the "Create Repository" button to create the repository.
4. Push your resume to the newly created repository by going to the repository and clicking the "Add file" button and then selecting your markdown formatted resume from your local computer. Make sure that your resume is named as "index.md" before uploading. Finally, commit the changes to push your resume to the repository.

The resume should now be successfully uploaded to the online repository. The last two steps can also be done using the command line. Steps to do this can be found [here](https://guides.github.com/activities/hello-world/).

## `3. Hosting the resume on Github Pages`

The final step to this task is to use a static website to host the resume that we created. In his book, Etter deeply encourages making static websites due to their speed, simplicity, portability, and security. Additionally, they have no server-side application dependencies, no databases, and nothing to install. Although Etter prefers using Sphinx, we will be using Jekyll since it is the most popular and is readily availabe for use in GitHub Pages.

The steps to host the resume with a theme on GitHub pages using Jekyll are given below:

1. Go to the repository and click on "Settings".
2. Navigate to the "Pages" section to go to the GitHub Pages webpage. 
3. Make sure that the main branch is selected under the "Source" section.
4. Click on the "Choose Theme" button to be redirected to a page showing the available themes for the static website. Click on "Select Theme" once you pick a theme to use. This will bring you back to the settings window.
5. Click on "Commit Changes" to finalize everything and create the static website.

We will now be able to see the resume on out static website. To do this, we can open a browser tab/window and type in "\<YourUsername>.github.io". This should display our resume on our static website.
