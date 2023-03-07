# Hosting a resume with GitHub Pages

Guide on formatting and hosting your resume on GitHub Pages using static site generator (Jekyll in this case).

## Prerequisites
* Markdown editor like Visual Studio Code 
* A resume formatted in Markdown
* Jekyll 
* GitHub account
* Windows operating system

## Instructions

1. ### Setting up the GitHub repository

    1. Create a new repository on your GitHub account.

    2. Go to Settings > Pages page for your repository.

    3. Navigate to Build and deployment, select Deploy from branch as the source and the desired branch (main is the default branch) and click save. 

    After completing the above steps you should have a GitHub pages website up and running within a few minutes. You can navigate to your website by clicking Visit site button on Settings > Pages page. 

2. ### Configuring the static site generator

    1. Go to the Settings > Page on your repository.
    
    2. Select add a Jekyll theme on the page.

    3. Select your desired theme by editing the _config.yml file using the above guide.

At the end of this step, you should see the changes on your website.



## More resources

1. [Markdown Tutorial](https://www.markdowntutorial.com/): An easy-to-follow tutorial for learning markdown.

2. [Jekyll Installation](https://jekyllrb.com/docs/installation/): Website features Jekyll installation for a variety of operating systems like macOS, Ubuntu and Windows.

3. [Windows CMD Cheatsheet](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands/): Tutorial features common CMD commands useful for following along with this README.


## FAQs

1. What is the default address of the Jekyll site?

    Answer: You can access your jekyll site after the serve command at http://localhost:4000.

2. Why is my website not showing up on the GitHub Pages page?

    Answer: In case you cannot see your website, go to Actions page on your repo. It should show your website under All workflows wait until the build is complete (a green mark is displayed) and try again.

## Authors
Arshdep Singh