<h1 align="center">Hi 👋, I'm Swarnava Ghosh</h1>
<h3 align="center">Backend-Focused Software Engineer | Java & MERN Stack Developer | DSA Enthusiast</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/swarnavaghosh51/" target="_blank">LinkedIn</a> •
  <a href="mailto:swarnaava.ghosh58@gmail.com">Email</a> •
  <a href="https://github.com/swarnaavaghosh58-codder">GitHub</a>
</p>

---

## 🚀 About Me

🎓 Computer Science Student passionate about building scalable and efficient software systems.  
💻 Strong foundation in **Java, Data Structures & Algorithms, and Full Stack Development**.  
🔥 Focused on backend architecture and writing clean, production-ready code.

### 🌱 Currently Learning
- Backend System Design
- Cloud & DevOps Fundamentals
- Scalable Architecture Patterns

---

## 🛠 Tech Stack

### 💻 Languages
Java • C++ • JavaScript • Python  

### ⚙ Backend
Spring Boot • Node.js • REST APIs  

### 🎨 Frontend
React.js • HTML • CSS  

### 🗄 Database
MySQL • MongoDB  

### 🚀 DevOps & Tools
Docker • Git • GitHub • Linux  

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=swarnaavaghosh58-codder&show_icons=true&theme=tokyonight&hide_border=true&cache_seconds=1800" height="180"/>
  
  <img src="https://streak-stats.demolab.com?user=swarnaavaghosh58-codder&theme=tokyonight&hide_border=true&cache_seconds=1800" height="180"/>
</p>

---

## 🚀 Top Languages

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=swarnaavaghosh58-codder&layout=compact&theme=tokyonight&hide_border=true&cache_seconds=1800" height="180"/>
</p>



name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: swarnaavaghosh58-codder
          outputs: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
