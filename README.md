## 👋 Hi! I'm Jhonata! 

-- 
## 👨‍💻 About Me
-- 
- 💻 I am currently studying Systems Analysis and Development at Eniac College (2026 - 2028)
- 🐍 I’m currently learning Python
- 📈 I am looking for collaboration opportunities in the field of systems development. ...
- 🤔 Studying and improving myself so that one day I can work in the IT field.
- 💬 I have other platforms to connect with you, like LinkedIn.
- ⚡ I've liked computers and video games since I was a child.


<div style="display: inline_block"><br>
  <img align="center" alt="Rafa-Python" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
</div>
  
  ##
 
<div> 
  <a href="https://www.youtube.com/channel/UC_-uuuZbY0AAt9CViNzvc-Q" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" target="_blank"></a>
 	<a href="https://www.twitch.tv/jonas241220" target="_blank"><img src="https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white" target="_blank"></a>
 <a href="https://discord.gg/E63JtECf" target="_blank"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" target="_blank"></a> 
 <a href="mailto:jhonatap386@gmail.com">
  <img src="https://img.shields.io/badge/-Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" target="_blank">
</a>

  <a href="https://www.linkedin.com/in/jhonata-pereira-345aa42a9/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  
</div>



name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

-uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
