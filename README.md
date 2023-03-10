# Hosting a resume with GitHub Pages

This guide aims to provide a quickstart in the field of technical writing for beginners. It employs various techniques mentioned in Andrew Etter's book Modern Technical writing. The content is split into two parts: first part of the guide focuses on explaining Etter's recommendations for technical writers. While the latter offers concrete implementation of Etter's principles by providing instructions on hosting a resume on GitHub Pages using Static site generators like Jekyll.

## Discussion of Etter's reccomendations

* ### 
* ### Hosting documents on a distributed version control system
    Etter's book highlights the importance of using a version control system like Git. It provides many benefits like providing a permanent storage space for your projects and documentation. It makes the process of tracking changes easy by allowing for mulitple restore points and also the ability to create branches for experimenting with new features. Most importantly it fosters colloboration among developers and stakeholders. Etter highlights the importance of communication between the stakeholders to deliver a better experience for the end user. Moreover, the colloboration ensures the documentation remains up to date and relevant for the end users and new errors and problems are added as they spring along the way. 

* ### Using static site generators.
    An important idea at the core of Etter's book is the simplification of process of technical writing to reduce the focus on building technologies to support the documentation and instead invest more time in perfecting the content. The idea is evident across the book as Etter recommends using simplified tools like markdown to further the idea. Similarly, instead of using complex hosting technologies and content management systems, Etter suggests the use of static site generator to build and host technical documentation. 

    Popular static site generators (SSG) like Jekyll is a popular choice for writing technical documentation. Jekyll is an open source static site generator based on Ruby and provides an excellent starting point for beginners. 

Github fits the bill of tools required for building technical documentation. It is based on the popular distributed version control system Git at the heart and has in built integration with Jekyll which highly simplifies the generation process. Moreover, it handles the whole site generation process without requiring users to have a deep knowledge of static site generators. At the same it offers experienced users the freedom to configure the site to their needs. Lastly, it also provides a free website to host the content on and is a perfect solution in itself. 

Therefore, the guide will focus on using GitHub as a solution to host a resume using the GitHub pages feature and demonstrate the principles at the heart of the Etter's book.




## Instructions on hosting the resume
---

### Prerequisites
* Windows operating system
* Markdown editor like Visual Studio Code 
* A resume formatted in Markdown
* Jekyll 
* GitHub account

### Steps

1. ### Setting up the GitHub repository

    1. Create a new repository on your GitHub account.
    
    2. Upload your resume as a markdown file and rename it to index.md.

    3. Go to Settings > Pages page for your repository.

    4. Navigate to Build and deployment.
    
    5. Select Deploy from branch as the source and the desired branch (main is the default branch) and click save. 

    After completing the above steps you should have a GitHub pages website up and running within a few minutes. You can navigate to your website by clicking Visit site button on Settings > Pages page. 

2. ### Configuring the static site generator

    1. Select a Jekyll theme you want to use for your resume. 
    
    2. Create a _config.yml file in your GitHub repository.

    3. Select your desired theme by editing the _config.yml file using the above guide.

GitHub's build tools work very well until they do not. Even in the best case the GitHub's site takes several minutes to show changes which may not be a big problem if you do not intend to make many changes in the website. However, the whole process starts to slow down the development time and in case GitHub's server are overwhelmed it can take siginificantly more time to complete the process. Therefore, setting up the process on a local machine makes the changes show up instantly and also offers a closer look at the processes which work inside the Jekyll website generation. 

3. ### Setting up Jekyll for local development
   
    1. Make sure your system has the latest version of Jekyll installed. Refer to this [guide](https://jekyllrb.com/docs/installation/windows/) for windows installation.

    2. Clone the GitHub repository to your local machine.

    3. Open a CMD on your machine and cd inside the directory where the repository is located.

    4. Execute the command below. 
        ``` console 
        jekyll serve
        ```
    5. The website will be available at  http://localhost:4000 on your machine.

At the end of this step, you should see the changes on your website. Here is a screenshot of a sample website generated using this guide.![Resume](resume.gif)



## More resources

1. [Markdown Tutorial](https://www.markdowntutorial.com/): An easy-to-follow tutorial for learning markdown.

2. [Jekyll Installation](https://jekyllrb.com/docs/installation/): Website features Jekyll installation for a variety of operating systems like macOS, Ubuntu and Windows.

3. [Windows CMD Cheatsheet](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands/): Tutorial features common CMD commands useful for following along with this README.


## FAQs

1. How to terminate the Jekyll site locally?

    Answer: You can terminate your jekyll site by pressing Ctrl + C.

2. Why is my website not showing up on the GitHub Pages page?

    Answer: In case you cannot see your website, go to Actions page on your repo. It should show your website under All workflows wait until the build is complete (a green mark is displayed) and try again.

## Authors and Acknoledgements
Author: Arshdep Singh

[Andrew Etter's Book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
