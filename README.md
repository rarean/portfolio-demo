# Bootstrap Portfolio Demo Project

A small **minimal Portfolio** with bootstrap based on [sivanesh-s.github.io](https://sivanesh-s.github.io/portfolio-minimal/)
with [GitHub Actions](https://github.com/features/actions) for continuous build/deployment to [github pages](https://pages.github.com/).

## Responsive
Like the original it is based on, this is responsive.

### Large Screen
<img src="./src/img/Lg.png" width="800px">

### Medium Screen
<img src="./src/img/Md.png" width="400px">

### Small Screen
<img src="./src/img/Sm.png" width="200px">

# Deploy your Bootstrap portfolio to GitHub Pages effortlessly
There are a few different ways of getting started with a website using bootstrap. You could start from scratch, you might have a website that you have put together based on a template, or you can fork an existing site and remake it as your own. However you obtain your site code, you want to publish the site somewhere and have heard about GitHub Pages, but you don’t know how to use GitHub to turn it into a free website.
This tutorial will create a basic one page portfolio and publish to GitHub Pages. If you already have a website ready to go, you can skip to the deployment section.

## Getting Started
Assuming you already have the necessary tools installed, and a GitHub account. If you do not have a GitHub account or need to install tools (npm, nodes, and git) please do so before continuing.
1. Fork the example repository https://github.com/rarean/portfolio-demo . It will take a few seconds to make a full copy of the example “portfolio-demo”.
2. Go to the Settings tab and rename the repository to `USERNAME.github.io`, be sure to use **your username** in place of **USERNAME**. This username should also match your account name in GitHub.
3. Clone the repo to your computer so that you have a local copy of the code to update with your changes
4. Open the index.html file and edit the appropriate sections
  * Your Name<br/>
    `<span id="name" class="d-block text-lg"> Your Name </span >`
  * Links
    ```
    <span id="links" class="text-md">
      <a href="https://github.com/"><i class="fa fa-github mx-2"></i></a>
      <a href="https://www.linkedin.com/"><i class="fa fa-linkedin-square mx-2"></i></a>
      <a href="mailto:your.mail@me.com?Subject=Hello%20again"><i class="fa fa-envelope-square mx-2"></i></a>
    </span>
    ```
  * Contact
    ```
    <div id="contact" class="col d-sm-block mx-auto my-auto text-center">
        <a href="https://github.com/" class="badge badge-light mt-5">Projects</a>
        <a href="mailto:your.mail@me.com?Subject=Hello%20again" class="badge badge-light">
          your.mail@me.com
        </a>
     </div>
    ```
5. Verify all your changes are correct and show up as expected
  * In the root folder of your project, run `npm install`
  * Once `node_modules` are installed, run `npm start`
  * Check your page for errors or changes

## Deploying Your Portfolio
Now that you have a portfolio site ready for GitHub Pages, you will only need to commit and push your changes to the master branch of your repository and ensure settings are pointing to the correct branch to display your site.

The magic that creates the site is found in the `.github/workflows/deploy.yml` file. This file tells GitHub Actions to install the project dependencies, run a build script that puts the required files in an output folder named “dist”, and then upload the contents of the “dist” folder to the gh-pages branch. If the branch does not exist, it will create the branch.

If you have an existing site or code that you want to publish to GitHub pages, you only need to add this file (and directory structure) to your project.

Once the gh-pages branch exists in your repository, go to the settings and ensure that the source for GitHub Pages is using this branch. Note that it may take a few minutes to populate DNS servers for it to show up in your browser.
