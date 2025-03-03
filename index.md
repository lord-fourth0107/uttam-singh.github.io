---
layout: default
---

<!-- Theme Toggle -->
<button id="theme-toggle" style="position: fixed; top: 20px; right: 20px; z-index: 1000;">🌓</button>

<div class="header-container">
    <img src="{{ '/assets/profile.jpg' | relative_url }}" alt="Uttam Singh" class="profile-img">
    <div class="header-text">
        <h1>Uttam Singh</h1>
        <p>Master's Candidate in Computer Science @ NYU</p>
        <div class="contact-links">
            <a href="mailto:us2193@nyu.edu">📧 Email</a>
            <a href="https://www.linkedin.com/in/uttam-singh-nyu/">💼 LinkedIn</a>
            <a href="https://github.com/lord-fourth0107">👨💻 GitHub</a>
            <a href="https://scholar.google.com/citations?user=MxGGafQAAAAJ&hl=en">📚 Google Scholar</a>
        </div>
    </div>
</div>

<style>
:root {
  --bg-color: #ffffff;
  --text-color: #2d3748;
  --accent-color: #2E86C1;
  --card-bg: #f8f9fa;
}

[data-theme="dark"] {
  --bg-color: #1a202c;
  --text-color: #e2e8f0;
  --accent-color: #63b3ed;
  --card-bg: #2d3748;
}

body {
  background: var(--bg-color);
  color: var(--text-color);
  transition: background 0.3s ease;
}

.header-container {
  display: flex;
  align-items: center;
  margin: 1rem 0;
  gap: 2rem;
}

.profile-img {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid var(--accent-color);
}

.contact-links a {
  margin-right: 1.2rem;
  color: var(--accent-color);
  text-decoration: none;
}

/* Compact Education Section */
.education-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 1rem 0;
  padding: 1rem;
  background: var(--card-bg);
  border-radius: 8px;
}

.logo-circle {
  width: 50px;
  height: 50px;
  min-width: 50px;
}

/* Reduced Section Spacing */
section {
  margin: 1.5rem 0;
}

#theme-toggle {
  background: transparent;
  border: none;
  cursor: pointer;
  font-size: 1.5rem;
  color: var(--text-color);
}
</style>

<script>
const toggle = document.getElementById('theme-toggle');
const storedTheme = localStorage.getItem('theme');

const setTheme = (theme) => {
  document.documentElement.setAttribute('data-theme', theme);
  localStorage.setItem('theme', theme);
};

toggle.addEventListener('click', () => {
  const currentTheme = document.documentElement.getAttribute('data-theme');
  setTheme(currentTheme === 'dark' ? 'light' : 'dark');
});

// Initialize theme
setTheme(storedTheme || (window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light'));
</script>
---
## 👨About Me

Hi ! I'm Uttam Singh, a Master's candidate in Computer Science at New York University. I'm passionate about building AI solutions, currently focusing on foundational  models. I have experience in building cloud-native solutions. My interest lies in implementing cutting-edge technologies integrating the system for enabling real-time inferencing. I get excited about the fundamental principles and algorithms that underpin the modern machine learning landscape. The most interesting part of my journey is the continuous learning process, where I stay updated with the latest advancements in the field. I also enjoy project management, learning about new products and startups. When I'm not coding or learning, I can be found reading books, running around the beach and watching movies or Onepiece.

---

## 🔍 Professional Summary
Software Engineer (SDE-2) with 4+ years of experience in building cloud-native systems and AI solutions.  
**Key Expertise**: AI/ML Researcher • Distributed Systems • GenAI Integration • Real-time Streaming • Medical Imaging • Open Source Contribution  
**Awards**: GEHC EmerGE 23 Runner-Up • 11 Impact Awards • Published Researcher

---


## 💻 Technical Experience

### 🏥 GE Healthcare | Software Engineer (SDE-2)
**Oct 2020 - Aug 2024**  
- Architected cloud-native streaming platform handling 25 Mbps data with <300ms latency  
- Reduced batch latency by 60% through Kafka-TCP integration template  
- Led LLM adoption for GenAI integration across enterprise verticals  
- Developed U-Net ML algorithm for tumor detection (Computer Vision/TensorFlow)  
- Built Azure IoT microservice for Kafka-to-IoTHub message transformation  
- Introduced open-source tools to improve developer experience cutting down operational time by 10 times 

### 🌐 Open Source Contributions
**Unoplat | Nov 2023 - Sept 2024**  
- Implemented Docusaurus-based documentation portal  
- Deployed production website using Vercel  

---

## 🎓 Education
<!-- Education Section -->
<div class="education-container">
  <!-- NYU -->
  <div class="education-item">
    <div class="logo-circle">
      <img src="{{ '/assets/nyu.jpg' | relative_url }}" alt="NYU Logo" class="institution-logo">
    </div>
    <div class="education-details">
      <h3>New York University</h3>
      <p>M.S. Computer Science | 2024-2026 | GPA: 4.0/4.0</p>
    </div>
  </div>

  <!-- NIT Rourkela -->
  <div class="education-item">
    <div class="logo-circle">
      <img src="{{ '/assets/nitrkl.jpeg' | relative_url }}" alt="NIT Rourkela Logo" class="institution-logo">
    </div>
    <div class="education-details">
      <h3>National Institute of Technology Rourkela</h3>
      <p>B.Tech Computer Science | 2016-2020 | GPA: 9.13/10</p>
    </div>
  </div>
</div>

<style>
.education-container {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.education-item {
  display: flex;
  align-items: center;
  gap: 1.5rem;
}

.logo-circle {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: #f0f0f0;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 2px solid #2E86C1; /* NYU purple/NIT blue */
}

.institution-logo {
  width: 80%;
  height: 80%;
  object-fit: contain;
}

.education-details {
  flex: 1;
}
</style>

---

## 🚀 Key Projects

### Distributed Data Platform (GE Healthcare)
`Java`, `Kafka`, `AWS`, `MSK`,`Helm`,`Quarkus`,`Strmzi`,`Grafana`,`Prometheus`,`Tilt`,`Datadog`,`OpenTelemetry`
- Poineered on template based microservice architecture to allow maximum code reuse across modalities
- Built a real-time streaming architecture on the principles of Data Mesh 
- Implemented multiple POC's for components of Data Platform including Redpanda, ArgoCD, Strmzi, k8s Operators, mulitple AWS and Azure offerings
- Introduced opensource tilt to streamline the workflow pre-commit CI/CD
- Worked towards GenAI integration on the platform

### Notification Middleware on Cloud(GE Healthcare)
`Java`, `Kafka`, `Azure IoT Hub`, `Service Account`,`Helm`,`Quarkus`
- Implemented Kafka-Azure IoT Hub message transformation pipeline to transfer data from public Cloud to private datacenters
- Built the monitoring and alerting framework across the workflow for reliablity of system
- Co-introduced Quarkus, a JIT based Java framework for building cloud-native applications providing efficient memory and cpu performance


### GenAI for ROS2 Robotics(NYU)
`LLM` `RAG` `Qdrant` `Docker`  
- Built real-time RAG system for robotic context-aware QA  
- Optimized vector search latency by 40% using Qdrant  
- Implemented web scraping pipeline for dynamic knowledge updates  



### Grid Artifact Correction in Mamogram Images(GE Healthcare)
`C++`,`Image Processing`
- Implemented a robust artifact correction algorithm for mamogram images

### EEG-based Emotion Classification(NIT Rourkela)
`Deep Learning` `PyTorch` `EEG Dataset`
- Developed a deep learning model for emotion classification with a heuristic approach for optimatal channel selection
- Implemented a signal processing based data reduction technique for faster processing

### Multimodal Sentiment Detection(NYU)
`Transformers` `PyTorch` `MVSA Dataset`  
- Developed fusion model with 89% accuracy on multimodal sentiment classification  
- Implemented attention-based feature alignment for text-image pairs  

### Predicting CoVID 19 using Google Trends(NIT Rourkela)
`Machine Learning` `Python` `Google Trends Dataset`
- Developed a machine learning model for predicting CoVID 19 cases using Google Trends data
- Combined the power of heuristic approach with RNN-based network to predict CoVID 19 cases


---

## 🛠️ Technical Arsenal
**Languages**: Java • Python • C++ • SQL • JavaScript  
**Cloud**: Azure IoT • AWS • GCP • Kubernetes • Helm  
**AI/ML**: PyTorch • TensorFlow • Computer Vision • NLP  
**Systems**: Kafka • Flink • Spark • Docker • Quarkus  

---

## 📜 Publications & Achievements
- 3 research papers in peer-reviewed journals  
- First Runner Up: GEHC EmerGE 2023 (Health-tech Innovation)  
- Patent-pending: Real-time Medical Data Streaming Architecture  

---
