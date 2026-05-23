# <span id="animated-name"></span>

Hi there! I'm Eskedar Nigussie

🎓 Computer Science Student | 💻 MERN Stack Developer  
💼 Open for Internship Opportunities (Frontend / Full Stack)

I am passionate about building clean, responsive, and user-friendly web applications using modern technologies. I enjoy learning by building real-world projects.

---

## 🌐 [Portfolio](https://personal-portfolio-web-sitee.netlify.app)

---

## 🚀 About Me
- 🔭 Currently mastering the MERN stack and building full-stack applications  
- 🌱 Learning advanced React patterns, Node.js, and database design  
- 🎯 Goal: Become a professional software engineer  
- 💡 I enjoy building real-world projects and solving problems  
- 📍 Based in Ethiopia  

---

## 🧠 Tech Stack

### 💻 Languages
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="50"/>
</p>

### ⚛️ Frontend
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" width="50"/>
</p>

### 🧩 Backend
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" width="50"/>
</p>

### 🛠 Tools & Deployment
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/render/render-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/netlify/netlify-original.svg" width="50"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vercel/vercel-original.svg" width="50"/>
</p>

---

## 📌 Featured Projects

### 🛒 E-Commerce Product Page
A responsive product listing website with a clean UI, showcasing items with images, pricing, and smooth user interaction.

**Features:**
- Product display grid
- Responsive design for all devices
- Simple and clean user interface

---

### 🧑‍💼 Personal Portfolio Website
A modern responsive portfolio built to showcase my skills, projects, and contact information in a professional and elegant way.

**Features:**
- About me section
- Project showcase
- Contact links and social media integration
- Fully responsive design

---

### 📅 Task Manager App
A simple and efficient task management web application that helps users organize daily tasks easily.

**Features:**
- Add and delete tasks
- Mark tasks as completed
- Clean and user-friendly interface
- Responsive layout

---

## 📫 Contact Me
- Email: nigussieeskedar@gmail.com 
- [Portfolio](https://personal-portfolio-web-sitee.netlify.app)

---

<!-- Animation Scripts -->
<script>
  // Animated name - letter by letter
  const name = "Eskedar Nigussie";
  const element = document.getElementById("animated-name");
  let i = 0;
  
  function typeWriter() {
    if (i < name.length) {
      element.innerHTML += name.charAt(i);
      i++;
      setTimeout(typeWriter, 100);
    }
  }
  
  typeWriter();

  // Sliding tech stack at the bottom
  const style = document.createElement('style');
  style.textContent = `
    @keyframes slide {
      0% { transform: translateX(100%); }
      100% { transform: translateX(-100%); }
    }
    
    .sliding-stack {
      position: fixed;
      bottom: 0;
      left: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.9);
      padding: 10px 0;
      overflow: hidden;
      white-space: nowrap;
      z-index: 1000;
      backdrop-filter: blur(10px);
      border-top: 1px solid rgba(255, 255, 255, 0.2);
    }
    
    .sliding-content {
      display: inline-block;
      animation: slide 20s linear infinite;
      color: white;
      font-family: monospace;
      font-size: 16px;
    }
    
    .sliding-content img {
      width: 30px;
      height: 30px;
      vertical-align: middle;
      margin: 0 10px;
    }
    
    .sliding-content span {
      margin: 0 20px;
    }
    
    .sliding-stack:hover .sliding-content {
      animation-play-state: paused;
    }
  `;
  document.head.appendChild(style);
  
  const tools = [
    "React", "Node.js", "Express", "MongoDB", "JavaScript", 
    "HTML5", "CSS3", "Git", "GitHub", "VS Code", 
    "Render", "Netlify", "Vercel"
  ];
  
  const slidingDiv = document.createElement('div');
  slidingDiv.className = 'sliding-stack';
  
  const contentDiv = document.createElement('div');
  contentDiv.className = 'sliding-content';
  
  // Duplicate content for seamless loop
  let content = '';
  for (let i = 0; i < 3; i++) {
    tools.forEach(tool => {
      content += `<span>⚡ ${tool}</span>`;
    });
  }
  
  contentDiv.innerHTML = content;
  slidingDiv.appendChild(contentDiv);
  document.body.appendChild(slidingDiv);
</script>
