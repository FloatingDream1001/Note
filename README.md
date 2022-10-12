### Hi there 👋


**2011526487/2011526487** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...caozhiy 
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
### 技术栈


![C](https://img.shields.io/badge/-C-%232c3e50?style=for-the-badge&logo=C)
![C++](https://img.shields.io/badge/-C++-%23F7DF1C?style=for-the-badge&logo=c++&logoColor=000000&labelColor=%23F7DF1C&color=%23FFCE5A)
![Python](https://img.shields.io/badge/-Python-%23E44D27?style=for-the-badge&logo=Python&logoColor=ffffff)
![HTML5](https://img.shields.io/badge/-HTML5-%23E44D27?style=for-the-badge&logo=html5&logoColor=ffffff)
![CSS3](https://img.shields.io/badge/-CSS3-%231572B6?style=for-the-badge&logo=css3)
![JavaScript](https://img.shields.io/badge/-JavaScript-%23F7DF1C?style=for-the-badge&logo=javascript&logoColor=000000&labelColor=%23F7DF1C&color=%23FFCE5A)
![Vue.js](https://img.shields.io/badge/-Vue.js-%232c3e50?style=for-the-badge&logo=Vue.js)
![Git](https://img.shields.io/badge/-Git-%23F05032?style=for-the-badge&logo=git&logoColor=%23ffffff)
![VS Code](https://img.shields.io/badge/-VSCode-%23007ACC?style=for-the-badge&logo=visual-studio-code)
# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 6 hours.

on:
  schedule:
      # every 6 hours
    - cron: "0 */6 * * *"

# This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:
    
    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2
      
    # Generates the snake  
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: arpanaditya
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg
          
     # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status
          
      # Push the changes
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true
          
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
### 我的Github
ShannonMYang's github stats](https://github-readme-stats.vercel.app/api?username=shannonmyang&show_icons=true&theme=dracula&local=cn)
### 我的代码库(部分)

-->
<!--
要显示的仓库，都可以在这里逐一填写上
-->

[![ReadMe Card](https://github-readme-stats.vercel.app/api/pin/?username=shannonmyang&repo=CDemo)](https://github.com/anuraghazra/github-readme-stats)


<!--

### 我的编程语言使用排行榜

-->

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=shannonmyang)](https://github.com/anuraghazra/github-readme-stats)


### 我的联系方式

> `简书`: [简书](https://www.jianshu.com/u/2fd0c319f098)
> `个人博客`: [个人博客]()
