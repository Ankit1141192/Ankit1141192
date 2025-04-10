<h1 align="center">Hi 👋, I'm Ankit Kumar</h1>
<h3 align="center">A passionate Full-Stack developer from India</h3>

<img align="right" alt="coding" width="400" src="https://user-images.githubusercontent.com/55389276/140866485-8fb1c876-9a8f-4d6a-98dc-08c4981eaf70.gif" />

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=ankit1141192&label=Profile%20views&color=0e75b6&style=flat" alt="ankit1141192" />
</p>

- 🔭 I’m currently working on [Shopnetic](https://github.com/Ankit1141192/ReactNativeProject/tree/main/Shopnetic)

- 🌱 I’m currently learning **Full-Stack Development at Masai School**

- 📫 How to reach me: **ankit2914978@gmail.com**

- 📄 Know about my experiences: [Resume](https://drive.google.com/file/d/1osrjwy_5oM4dqDILhARHewyvgcAIKKnP/view?usp=sharing)

---

<h3 align="left">Connect with me:</h3>
<p align="left">
  <a href="https://www.linkedin.com/in/ankit1141" target="blank">
    <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="ankit1141" height="30" width="40" />
  </a>
  <a href="https://leetcode.com/ankit1141192/" target="blank">
    <img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" alt="ankit1141192" height="30" width="40" />
  </a>
  <a href="https://github.com/Ankit1141192" target="blank">
    <img align="center" src="https://img.icons8.com/ios-filled/50/000000/github.png" alt="GitHub" height="30" width="30" />
  </a>
</p>

---

<h3 align="left">Languages and Tools:</h3>
<p align="left">
  <a href="https://www.w3.org/html/" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40" />
  </a>
  <a href="https://www.w3schools.com/css/" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40" />
  </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40" />
  </a>
  <a href="https://reactjs.org/" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40" />
  </a>
  <a href="https://reactnative.dev/" target="_blank">
    <img src="https://reactnative.dev/img/header_logo.svg" alt="reactnative" width="40" height="40" />
  </a>
  <a href="https://www.mongodb.com/" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40" />
  </a>
  <a href="https://firebase.google.com/" target="_blank">
    <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40" />
  </a>
  <a href="https://www.python.org" target="_blank">
    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40" />
  </a>
</p>

---

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=ankit1141192&show_icons=true&locale=en&layout=compact" alt="ankit1141192" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=ankit1141192&show_icons=true&locale=en" alt="ankit1141192" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=ankit1141192&" alt="ankit1141192" /></p>

---

## 🐍 Contribution Graph Snake Animation

```yaml
# .github/workflows/snake.yml

name: 🐍 Generate Snake

on:
  schedule:
    - cron: "0 0 * * *" # every day at midnight
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark
            dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
      - name: Push generated snake to the output branch
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
