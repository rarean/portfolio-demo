# bootstrapCi-demo

A small **minimal Portfolio** with bootstrap based on [sivanesh-s.github.io](https://sivanesh-s.github.io/portfolio-minimal/)
with circleCi for continuous build/deployment to github pages.

## Responsive
Like the original it is based on, this is responsive.

### Large Screen
<img src="./src/img/Lg.png" >

### Medium Screen
<img src="./src/img/Md.png" >

### Small Screen
<img src="./src/img/Sm.png" >

## Usage
* Clone the repo `git clone `
* [Create a repo][1] in GitHub with the format `yourUsername.github.io`
* Enable [GitHub pages][1] for the `master` branch
* Create a `develop` branch for your changes (files on master will be updated
  by CircleCi)
* Create Read/Write [deploy keys][2] for your repo
* [Link CircleCi][3] to your repo
* [Upload your private key][4] to CircleCi
* Copy the fingerprint of your private key and paste in the
  `.circleci/config.yml` file
* Push up your `develop` branch

[1](https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site)
[2]()
[3]()
[4]()
[5]()
