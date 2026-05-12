<svg width="100%" height="600" viewBox="0 0 1200 600" xmlns="http://www.w3.org/2000/svg" style="position: absolute; top: 0; left: 0; z-index: -1;">
  <defs>
    <style>
      @keyframes moveStars {
        0% { transform: translateY(0px) translateX(0px); opacity: 0.3; }
        50% { opacity: 1; }
        100% { transform: translateY(-600px) translateX(20px); opacity: 0; }
      }
      @keyframes twinkle {
        0%, 100% { opacity: 0.3; }
        50% { opacity: 1; }
      }
      @keyframes float {
        0%, 100% { transform: translateY(0px); }
        50% { transform: translateY(-30px); }
      }
      @keyframes rotate3d {
        0% { transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg); }
        100% { transform: rotateX(360deg) rotateY(360deg) rotateZ(360deg); }
      }
      @keyframes glow {
        0%, 100% { filter: drop-shadow(0 0 5px rgba(102, 126, 234, 0.5)); }
        50% { filter: drop-shadow(0 0 20px rgba(102, 126, 234, 1)); }
      }
      .star {
        animation: moveStars linear infinite, twinkle 3s ease-in-out infinite;
      }
      .title-bg {
        animation: glow 2s ease-in-out infinite;
      }
    </style>
    <linearGradient id="starGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#667eea;stop-opacity:0.8" />
      <stop offset="100%" style="stop-color:#f093fb;stop-opacity:0.8" />
    </linearGradient>
    <filter id="blur">
      <feGaussianBlur in="SourceGraphic" stdDeviation="3" />
    </filter>
  </defs>
  
  <!-- Animated Gradient Background -->
  <rect width="1200" height="600" fill="url(#starGradient)" opacity="0.1"/>
  
  <!-- Moving Stars -->
  <circle cx="100" cy="50" r="2" fill="#667eea" class="star" style="animation-duration: 8s; animation-delay: 0s;"/>
  <circle cx="250" cy="80" r="1.5" fill="#f093fb" class="star" style="animation-duration: 10s; animation-delay: 1s;"/>
  <circle cx="400" cy="100" r="2" fill="#667eea" class="star" style="animation-duration: 12s; animation-delay: 2s;"/>
  <circle cx="550" cy="120" r="1.5" fill="#f5576c" class="star" style="animation-duration: 9s; animation-delay: 0.5s;"/>
  <circle cx="700" cy="60" r="2" fill="#764ba2" class="star" style="animation-duration: 11s; animation-delay: 1.5s;"/>
  <circle cx="850" cy="140" r="1.5" fill="#667eea" class="star" style="animation-duration: 10s; animation-delay: 0.8s;"/>
  <circle cx="1000" cy="90" r="2" fill="#f093fb" class="star" style="animation-duration: 13s; animation-delay: 2.5s;"/>
  <circle cx="150" cy="200" r="1.5" fill="#f5576c" class="star" style="animation-duration: 11s; animation-delay: 1.2s;"/>
  <circle cx="350" cy="250" r="2" fill="#764ba2" class="star" style="animation-duration: 9.5s; animation-delay: 0.3s;"/>
  <circle cx="600" cy="180" r="1.5" fill="#667eea" class="star" style="animation-duration: 12s; animation-delay: 1.8s;"/>
  <circle cx="900" cy="220" r="2" fill="#f093fb" class="star" style="animation-duration: 10.5s; animation-delay: 0.6s;"/>
  <circle cx="1100" cy="150" r="1.5" fill="#f5576c" class="star" style="animation-duration: 11.5s; animation-delay: 2s;"/>
  <circle cx="80" cy="350" r="2" fill="#764ba2" class="star" style="animation-duration: 9s; animation-delay: 1.1s;"/>
  <circle cx="300" cy="400" r="1.5" fill="#667eea" class="star" style="animation-duration: 12.5s; animation-delay: 0.4s;"/>
  <circle cx="500" cy="380" r="2" fill="#f093fb" class="star" style="animation-duration: 10s; animation-delay: 1.7s;"/>
</svg>

<div align="center" style="
  position: relative;
  z-index: 1;
  padding: 40px 20px;
  background: radial-gradient(ellipse at center, rgba(255,255,255,0.1) 0%, rgba(255,255,255,0) 70%);
">

<!-- ANIMATED 3D TITLE WITH MOVING STARS BACKGROUND -->
<div style="
  position: relative;
  margin-bottom: 30px;
  perspective: 1000px;
  height: 200px;
  display: flex;
  align-items: center;
  justify-content: center;
">
  
  <!-- 3D Background Cards Behind Title -->
  <div style="
    position: absolute;
    width: 500px;
    height: 180px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
    border-radius: 20px;
    opacity: 0.1;
    filter: blur(30px);
    animation: float 4s ease-in-out infinite;
    top: 10px;
    z-index: 0;
  "></div>

  <div style="
    position: absolute;
    width: 450px;
    height: 150px;
    background: linear-gradient(135deg, #f5576c 0%, #f093fb 100%);
    border-radius: 20px;
    opacity: 0.08;
    filter: blur(25px);
    animation: float 5s ease-in-out infinite;
    animation-delay: 0.5s;
    top: 25px;
    z-index: 0;
  "></div>

  <!-- Main 3D Text -->
  <h1 style="
    position: relative;
    z-index: 10;
    margin: 0;
    font-size: 4.5em;
    font-weight: 900;
    letter-spacing: 3px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #f5576c 75%, #667eea 100%);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: glow 2s ease-in-out infinite, moveText 3s ease-in-out infinite;
    text-shadow: 0 0 80px rgba(102, 126, 234, 0.3);
    filter: drop-shadow(0 10px 30px rgba(102, 126, 234, 0.3));
  ">
    👋 RAHUL RANA
  </h1>

  <style>
    @keyframes moveText {
      0%, 100% { transform: translateY(0px) scale(1); }
      50% { transform: translateY(-15px) scale(1.02); }
    }
    @keyframes glow {
      0%, 100% { 
        text-shadow: 0 0 20px rgba(102, 126, 234, 0.4),
                     0 0 40px rgba(102, 126, 234, 0.2);
        filter: drop-shadow(0 10px 30px rgba(102, 126, 234, 0.3));
      }
      50% { 
        text-shadow: 0 0 40px rgba(102, 126, 234, 0.8),
                     0 0 80px rgba(240, 147, 251, 0.4);
        filter: drop-shadow(0 10px 50px rgba(102, 126, 234, 0.6));
      }
    }
  </style>

</div>

<!-- Animated Subtitle -->
<h3 style="
  font-size: 1.6em;
  background: linear-gradient(90deg, #667eea, #764ba2, #f093fb, #f5576c);
  background-size: 200% 200%;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  animation: shimmer 3s ease-in-out infinite, slideDown 0.8s ease-out;
  margin: 20px 0;
  font-weight: 700;
  letter-spacing: 1px;
">
  Backend Developer | Open Source | GenAI Enthusiast 🚀
</h3>

<style>
  @keyframes shimmer {
    0%, 100% { background-position: 0% center; }
    50% { background-position: 100% center; }
  }
  @keyframes slideDown {
    from {
      opacity: 0;
      transform: translateY(-30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>

<!-- Glowing Info Section -->
<div style="
  margin: 30px 0;
  padding: 25px 30px;
  background: linear-gradient(135deg, rgba(102, 126, 234, 0.1) 0%, rgba(240, 147, 251, 0.1) 100%);
  border: 2px solid;
  border-image: linear-gradient(135deg, #667eea, #f093fb) 1;
  border-radius: 15px;
  backdrop-filter: blur(10px);
  box-shadow: 0 8px 32px rgba(102, 126, 234, 0.2),
              0 0 20px rgba(240, 147, 251, 0.1);
  animation: pulseBorder 3s ease-in-out infinite;
">
  <p style="
    font-size: 1.2em;
    color: #333;
    margin: 0;
    font-weight: 600;
  ">
    💡 Building Scalable Backend Systems & Real-World Solutions
  </p>
</div>

<style>
  @keyframes pulseBorder {
    0%, 100% { 
      box-shadow: 0 8px 32px rgba(102, 126, 234, 0.2),
                  0 0 20px rgba(240, 147, 251, 0.1);
    }
    50% { 
      box-shadow: 0 8px 32px rgba(102, 126, 234, 0.5),
                  0 0 40px rgba(240, 147, 251, 0.3);
    }
  }
</style>

</div>

---

## 🎯 About Me

<div style="
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 15px;
  margin: 30px auto;
  max-width: 700px;
">

<div style="
  padding: 20px;
  background: linear-gradient(135deg, rgba(102, 126, 234, 0.15) 0%, rgba(102, 126, 234, 0.05) 100%);
  border-left: 4px solid #667eea;
  border-radius: 10px;
  transition: all 0.3s ease;
  animation: cardFloat 3s ease-in-out infinite;
" onmouseover="this.style.transform='translateY(-8px)'; this.style.boxShadow='0 15px 35px rgba(102, 126, 234, 0.3)';"
   onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='none';">
  <strong style="color: #667eea; font-size: 1.1em;">🔭 Currently</strong><br/>
  <span style="color: #555;">GenAI Chatbot Development</span>
</div>

<div style="
  padding: 20px;
  background: linear-gradient(135deg, rgba(240, 147, 251, 0.15) 0%, rgba(240, 147, 251, 0.05) 100%);
  border-left: 4px solid #f093fb;
  border-radius: 10px;
  transition: all 0.3s ease;
  animation: cardFloat 3s ease-in-out infinite;
  animation-delay: 0.2s;
" onmouseover="this.style.transform='translateY(-8px)'; this.style.boxShadow='0 15px 35px rgba(240, 147, 251, 0.3)';"
   onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='none';">
  <strong style="color: #f093fb; font-size: 1.1em;">🌱 Learning</strong><br/>
  <span style="color: #555;">React, Node.js, DSA</span>
</div>

<div style="
  padding: 20px;
  background: linear-gradient(135deg, rgba(245, 87, 108, 0.15) 0%, rgba(245, 87, 108, 0.05) 100%);
  border-left: 4px solid #f5576c;
  border-radius: 10px;
  transition: all 0.3s ease;
  animation: cardFloat 3s ease-in-out infinite;
  animation-delay: 0.4s;
" onmouseover="this.style.transform='translateY(-8px)'; this.style.boxShadow='0 15px 35px rgba(245, 87, 108, 0.3)';"
   onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='none';">
  <strong style="color: #f5576c; font-size: 1.1em;">👯 Collaborate</strong><br/>
  <span style="color: #555;">Cloud-based Projects</span>
</div>

<div style="
  padding: 20px;
  background: linear-gradient(135deg, rgba(118, 75, 162, 0.15) 0%, rgba(118, 75, 162, 0.05) 100%);
  border-left: 4px solid #764ba2;
  border-radius: 10px;
  transition: all 0.3s ease;
  animation: cardFloat 3s ease-in-out infinite;
  animation-delay: 0.6s;
" onmouseover="this.style.transform='translateY(-8px)'; this.style.boxShadow='0 15px 35px rgba(118, 75, 162, 0.3)';"
   onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='none';">
  <strong style="color: #764ba2; font-size: 1.1em;">🤝 Help With</strong><br/>
  <span style="color: #555;">Cloud Deployment</span>
</div>

</div>

<style>
  @keyframes cardFloat {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-8px); }
  }
</style>

---

## 🌐 Connect With Me

<div style="
  display: flex;
  gap: 25px;
  justify-content: center;
  flex-wrap: wrap;
  margin: 40px 0;
  animation: fadeIn 1s ease-out;
">

<a href="https://www.linkedin.com/in/rahul-rana-61252a321/" target="_blank" style="
  position: relative;
  text-decoration: none;
  perspective: 1000px;
">
  <div style="
    padding: 15px 25px;
    background: linear-gradient(135deg, #0077B5 0%, #00A0D2 100%);
    color: white;
    border-radius: 15px;
    font-weight: 700;
    font-size: 1em;
    display: flex;
    align-items: center;
    gap: 10px;
    box-shadow: 0 8px 25px rgba(0, 119, 181, 0.3);
    transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
    cursor: pointer;
    animation: iconPop 2s ease-in-out infinite;
  "
  onmouseover="this.style.transform='translateY(-8px) scale(1.08) rotateY(5deg)'; this.style.boxShadow='0 15px 40px rgba(0, 119, 181, 0.6)';"
  onmouseout="this.style.transform='translateY(0) scale(1) rotateY(0deg)'; this.style.boxShadow='0 8px 25px rgba(0, 119, 181, 0.3)';">
    🔗 LinkedIn
  </div>
</a>

<a href="https://instagram.com/rahulrana4671" target="_blank" style="
  position: relative;
  text-decoration: none;
">
  <div style="
    padding: 15px 25px;
    background: linear-gradient(135deg, #E4405F 0%, #F77737 100%);
    color: white;
    border-radius: 15px;
    font-weight: 700;
    font-size: 1em;
    display: flex;
    align-items: center;
    gap: 10px;
    box-shadow: 0 8px 25px rgba(228, 64, 95, 0.3);
    transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
    cursor: pointer;
    animation: iconPop 2s ease-in-out infinite;
    animation-delay: 0.3s;
  "
  onmouseover="this.style.transform='translateY(-8px) scale(1.08) rotateY(5deg)'; this.style.boxShadow='0 15px 40px rgba(228, 64, 95, 0.6)';"
  onmouseout="this.style.transform='translateY(0) scale(1) rotateY(0deg)'; this.style.boxShadow='0 8px 25px rgba(228, 64, 95, 0.3)';">
    📸 Instagram
  </div>
</a>

<a href="https://leetcode.com/rahul9520" target="_blank" style="
  position: relative;
  text-decoration: none;
">
  <div style="
    padding: 15px 25px;
    background: linear-gradient(135deg, #FFA116 0%, #FFD700 100%);
    color: #000;
    border-radius: 15px;
    font-weight: 700;
    font-size: 1em;
    display: flex;
    align-items: center;
    gap: 10px;
    box-shadow: 0 8px 25px rgba(255, 161, 22, 0.3);
    transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
    cursor: pointer;
    animation: iconPop 2s ease-in-out infinite;
    animation-delay: 0.6s;
  "
  onmouseover="this.style.transform='translateY(-8px) scale(1.08) rotateY(5deg)'; this.style.boxShadow='0 15px 40px rgba(255, 161, 22, 0.6)';"
  onmouseout="this.style.transform='translateY(0) scale(1) rotateY(0deg)'; this.style.boxShadow='0 8px 25px rgba(255, 161, 22, 0.3)';">
    🏆 LeetCode
  </div>
</a>

<a href="https://github.com/rahulrana9520" target="_blank" style="
  position: relative;
  text-decoration: none;
">
  <div style="
    padding: 15px 25px;
    background: linear-gradient(135deg, #333333 0%, #555555 100%);
    color: white;
    border-radius: 15px;
    font-weight: 700;
    font-size: 1em;
    display: flex;
    align-items: center;
    gap: 10px;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
    transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
    cursor: pointer;
    animation: iconPop 2s ease-in-out infinite;
    animation-delay: 0.9s;
  "
  onmouseover="this.style.transform='translateY(-8px) scale(1.08) rotateY(5deg)'; this.style.boxShadow='0 15px 40px rgba(0, 0, 0, 0.6)';"
  onmouseout="this.style.transform='translateY(0) scale(1) rotateY(0deg)'; this.style.boxShadow='0 8px 25px rgba(0, 0, 0, 0.3)';">
    💻 GitHub
  </div>
</a>

</div>

<style>
  @keyframes iconPop {
    0%, 100% { transform: translateY(0px) scale(1); }
    50% { transform: translateY(-12px) scale(1.02); }
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
</style>

---

## ⚡ Tech Stack

<div style="margin: 40px 0;">

### 💻 Languages
![Languages](https://skillicons.dev/icons?i=cpp,c,java,js,python&perline=5)

### 🚀 Backend & Databases
![Backend](https://skillicons.dev/icons?i=nodejs,express,mysql,mongodb,firebase&perline=5)

### 🎨 Frontend & Styling
![Frontend](https://skillicons.dev/icons?i=react,html,css,tailwind,bootstrap&perline=5)

### 🛠️ Tools & Platforms
![Tools](https://skillicons.dev/icons?i=git,github,vscode,postman,docker&perline=5)

</div>

---

## 📊 GitHub Stats

<div align="center" style="
  margin: 50px 0;
  animation: statsAppear 1.5s ease-out;
">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=rahulrana9520&theme=tokyonight&hide_border=true&stroke=667eea&background=0d1117)

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=rahulrana9520&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&text_color=fff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=rahulrana9520&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117)

</div>

<style>
  @keyframes statsAppear {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>

---

## 🔥 Open Source Contributions

<div style="
  position: relative;
  margin: 40px auto;
  max-width: 800px;
  padding: 30px;
  background: linear-gradient(135deg, rgba(102, 126, 234, 0.1) 0%, rgba(240, 147, 251, 0.1) 100%);
  border: 2px solid rgba(102, 126, 234, 0.3);
  border-radius: 15px;
  backdrop-filter: blur(10px);
  animation: slideIn 0.8s ease-out;
">

<div style="
  position: absolute;
  top: -15px;
  left: 20px;
  padding: 5px 15px;
  background: linear-gradient(135deg, #667eea, #f093fb);
  color: white;
  border-radius: 20px;
  font-weight: 700;
  font-size: 0.9em;
">
  ✨ Open Source ✨
</div>

<div style="margin-top: 20px;">
  ✅ Contributed to real-world repositories  
  ✅ Implemented backend features and APIs  
  ✅ Optimized performance & debugging solutions

  ### Notable Contributions:
  
  <div style="
    display: flex;
    flex-direction: column;
    gap: 15px;
    margin-top: 20px;
  ">
    <a href="https://github.com/Trying-Two-Code/Tryingtocode.com/pull/15" target="_blank" style="
      padding: 15px 20px;
      background: white;
      border-left: 4px solid #667eea;
      border-radius: 8px;
      text-decoration: none;
      color: #667eea;
      font-weight: 600;
      transition: all 0.3s ease;
      display: block;
      cursor: pointer;
    "
    onmouseover="this.style.transform='translateX(10px)'; this.style.boxShadow='0 10px 25px rgba(102, 126, 234, 0.2)';"
    onmouseout="this.style.transform='translateX(0)'; this.style.boxShadow='none';">
      📌 Tryingtocode.com - PR #15
    </a>
    
    <a href="https://github.com/bhavyakashmira/AIcruiter/pull/21" target="_blank" style="
      padding: 15px 20px;
      background: white;
      border-left: 4px solid #f093fb;
      border-radius: 8px;
      text-decoration: none;
      color: #f093fb;
      font-weight: 600;
      transition: all 0.3s ease;
      display: block;
      cursor: pointer;
    "
    onmouseover="this.style.transform='translateX(10px)'; this.style.boxShadow='0 10px 25px rgba(240, 147, 251, 0.2)';"
    onmouseout="this.style.transform='translateX(0)'; this.style.boxShadow='none';">
      🤖 AIcruiter - PR #21
    </a>
    
    <a href="https://github.com/ayushbarthwal/bonfire" target="_blank" style="
      padding: 15px 20px;
      background: white;
      border-left: 4px solid #f5576c;
      border-radius: 8px;
      text-decoration: none;
      color: #f5576c;
      font-weight: 600;
      transition: all 0.3s ease;
      display: block;
      cursor: pointer;
    "
    onmouseover="this.style.transform='translateX(10px)'; this.style.boxShadow='0 10px 25px rgba(245, 87, 108, 0.2)';"
    onmouseout="this.style.transform='translateX(0)'; this.style.boxShadow='none';">
      🔥 Bonfire Project
    </a>
  </div>
</div>

</div>

<style>
  @keyframes slideIn {
    from {
      opacity: 0;
      transform: translateX(-30px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }
</style>

---

## 📌 Featured Projects

<div style="
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  margin: 50px auto;
  max-width: 1200px;
">

<!-- Project 1 -->
<div style="
  position: relative;
  height: 300px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 15px 40px rgba(102, 126, 234, 0.3);
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  cursor: pointer;
  animation: projectAppear 0.8s ease-out;
"
onmouseover="this.style.transform='translateY(-15px) scale(1.05) rotateX(-5deg)'; this.style.boxShadow='0 25px 60px rgba(102, 126, 234, 0.5)';"
onmouseout="this.style.transform='translateY(0) scale(1) rotateX(0deg)'; this.style.boxShadow='0 15px 40px rgba(102, 126, 234, 0.3)';">
  
  <div style="
    position: absolute;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgba(255,255,255,0.2) 0%, transparent 100%);
    animation: shine 3s ease-in-out infinite;
  "></div>
  
  <div style="
    padding: 30px;
    color: white;
    position: relative;
    z-index: 2;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  ">
    <div>
      <h3 style="margin: 0 0 15px 0; font-size: 1.8em;">🚀 TransPyC</h3>
      <p style="margin: 0; font-size: 1em; line-height: 1.6;">Python → C/C++ Converter (PWA)</p>
    </div>
    <p style="margin: 0; font-size: 0.9em; opacity: 0.9;">Advanced code transpilation with optimization</p>
  </div>
</div>

<!-- Project 2 -->
<div style="
  position: relative;
  height: 300px;
  background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 15px 40px rgba(240, 147, 251, 0.3);
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  cursor: pointer;
  animation: projectAppear 0.8s ease-out;
  animation-delay: 0.2s;
"
onmouseover="this.style.transform='translateY(-15px) scale(1.05) rotateX(-5deg)'; this.style.boxShadow='0 25px 60px rgba(240, 147, 251, 0.5)';"
onmouseout="this.style.transform='translateY(0) scale(1) rotateX(0deg)'; this.style.boxShadow='0 15px 40px rgba(240, 147, 251, 0.3)';">
  
  <div style="
    position: absolute;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgba(255,255,255,0.2) 0%, transparent 100%);
    animation: shine 3s ease-in-out infinite;
  "></div>
  
  <div style="
    padding: 30px;
    color: white;
    position: relative;
    z-index: 2;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  ">
    <div>
      <h3 style="margin: 0 0 15px 0; font-size: 1.8em;">🤖 AI Recruiter</h3>
      <p style="margin: 0; font-size: 1em; line-height: 1.6;">Candidate Pipeline & APIs</p>
    </div>
    <p style="margin: 0; font-size: 0.9em; opacity: 0.9;">Intelligent recruitment automation</p>
  </div>
</div>

<!-- Project 3 -->
<div style="
  position: relative;
  height: 300px;
  background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 15px 40px rgba(79, 172, 254, 0.3);
  transition: all 0.4s cubic-bezier(0.34, 1.56, 0.64, 1);
  cursor: pointer;
  animation: projectAppear 0.8s ease-out;
  animation-delay: 0.4s;
"
onmouseover="this.style.transform='translateY(-15px) scale(1.05) rotateX(-5deg)'; this.style.boxShadow='0 25px 60px rgba(79, 172, 254, 0.5)';"
onmouseout="this.style.transform='translateY(0) scale(1) rotateX(0deg)'; this.style.boxShadow='0 15px 40px rgba(79, 172, 254, 0.3)';">
  
  <div style="
    position: absolute;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgba(255,255,255,0.2) 0%, transparent 100%);
    animation: shine 3s ease-in-out infinite;
  "></div>
  
  <div style="
    padding: 30px;
    color: white;
    position: relative;
    z-index: 2;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  ">
    <div>
      <h3 style="margin: 0 0 15px 0; font-size: 1.8em;">📦 Warehouse</h3>
      <p style="margin: 0; font-size: 1em; line-height: 1.6;">Dijkstra + Knapsack Optimization</p>
    </div>
    <p style="margin: 0; font-size: 0.9em; opacity: 0.9;">Efficient logistics & inventory</p>
  </div>
</div>

</div>

<style>
  @keyframes shine {
    0%, 100% { transform: translateX(-100%); }
    100% { transform: translateX(100%); }
  }
  @keyframes projectAppear {
    from {
      opacity: 0;
      transform: translateY(30px) scale(0.9);
    }
    to {
      opacity: 1;
      transform: translateY(0) scale(1);
    }
  }
</style>

---

## 🎯 Skills & Interests

<div style="
  display: flex;
  gap: 12px;
  justify-content: center;
  flex-wrap: wrap;
  margin: 40px 0;
">
  <span style="
    padding: 10px 20px;
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
    border-radius: 25px;
    font-weight: 600;
    font-size: 0.95em;
    box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
    animation: badgeFloat 2s ease-in-out infinite;
  ">🔐 Backend Architecture</span>
  
  <span style="
    padding: 10px 20px;
    background: linear-gradient(135deg, #f093fb, #f5576c);
    color: white;
    border-radius: 25px;
    font-weight: 600;
    font-size: 0.95em;
    box-shadow: 0 5px 15px rgba(240, 147, 251, 0.3);
    animation: badgeFloat 2s ease-in-out infinite;
    animation-delay: 0.2s;
  ">🤖 GenAI & ML</span>
  
  <span style="
    padding: 10px 20px;
    background: linear-gradient(135deg, #4facfe, #00f2fe);
    color: white;
    border-radius: 25px;
    font-weight: 600;
    font-size: 0.95em;
    box-shadow: 0 5px 15px rgba(79, 172, 254, 0.3);
    animation: badgeFloat 2s ease-in-out infinite;
    animation-delay: 0.4s;
  ">☁️ Cloud Services</span>
  
  <span style="
    padding: 10px 20px;
    background: linear-gradient(135deg, #FA8231, #F7DC6F);
    color: white;
    border-radius: 25px;
    font-weight: 600;
    font-size: 0.95em;
    box-shadow: 0 5px 15px rgba(250, 130, 49, 0.3);
    animation: badgeFloat 2s ease-in-out infinite;
    animation-delay: 0.6s;
  ">⚙️ System Design</span>
  
  <span style="
    padding: 10px 20px;
    background: linear-gradient(135deg, #E74C3C, #C0392B);
    color: white;
    border-radius: 25px;
    font-weight: 600;
    font-size: 0.95em;
    box-shadow: 0 5px 15px rgba(231, 76, 60, 0.3);
    animation: badgeFloat 2s ease-in-out infinite;
    animation-delay: 0.8s;
  ">🏆 Competitive Programming</span>
</div>

<style>
  @keyframes badgeFloat {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-8px); }
  }
</style>

---

<div align="center" style="
  margin-top: 60px;
  padding: 40px;
  background: linear-gradient(135deg, rgba(102, 126, 234, 0.1) 0%, rgba(240, 147, 251, 0.1) 100%);
  border: 2px solid rgba(102, 126, 234, 0.3);
  border-radius: 20px;
  animation: fadeInUp 1s ease-out;
">

<h2 style="
  background: linear-gradient(135deg, #667eea, #764ba2, #f093fb, #f5576c);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin: 0 0 15px 0;
  font-size: 2em;
  animation: glow 2s ease-in-out infinite;
">
  ✨ Let's Build Something Amazing! ✨
</h2>

<p style="
  color: #555;
  font-size: 1.1em;
  margin: 0;
">
  Feel free to reach out for collaborations or just to connect! 👉 
  <strong style="color: #667eea;">rahul015january@gmail.com</strong>
</p>

</div>

<style>
  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>

<div align="center" style="margin-top: 30px;">
  ![Profile Views](https://komarev.com/ghpvc/?username=rahulrana9520&label=Profile%20Views&color=667eea&style=flat-square&up_color=blueviolet)
</div>
