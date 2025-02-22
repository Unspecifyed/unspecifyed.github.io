---
layout: default
title: "Resume"
description: "View my professional resume and experiences."
---

<style>
  body {
    background-color: #1a1a1a; /* Dark black background */
    color: #e63946; /* Vibrant red for text */
    font-family: Arial, sans-serif;
  }

  .resume-header {
    text-align: center;
    margin-top: 50px;
    margin-bottom: 30px;
  }

  .resume-header h1 {
    font-size: 2.5em;
    color: #e63946; /* Red for the title */
  }

  .resume-section {
    margin: 30px auto;
    max-width: 800px;
  }

  .resume-section h2 {
    color: #e63946; /* Red for section headers */
    border-bottom: 2px solid #e63946;
    padding-bottom: 5px;
    margin-bottom: 15px;
  }

  .resume-item {
    margin-bottom: 20px;
  }

  .resume-item h3 {
    color: #ffffff; /* White for job titles and project names */
  }

  .resume-item p {
    color: #f5f5f5; /* Light gray for descriptions */
  }
</style>

<div class="resume-header">
  <h1>Resume</h1>
</div>

<div class="resume-section">
  <h2>Education</h2>
  <div class="resume-item">
    <h3>Bachelor of Science in Computer Science</h3>
    <p>University of [Your University] | [Graduation Year]</p>
  </div>
</div>

<div class="resume-section">
  <h2>Professional Experience</h2>
  <div class="resume-item">
    <h3>Software Developer Intern</h3>
    <p>[Company Name] | [MM/YYYY - MM/YYYY]</p>
    <ul>
      <li>Developed a feature to [describe key achievement].</li>
      <li>Collaborated with cross-functional teams to [describe team contributions].</li>
    </ul>
  </div>
</div>

<div class="resume-section">
  <h2>Projects</h2>
  {% for project in site.data.projects %}
  <div class="resume-item">
    <h3>{{ project.name }}</h3>
    <p>{{ project.description }}</p>
    <a href="{{ project.url }}" target="_blank">View on GitHub</a>
  </div>
  {% endfor %}
</div>

<div class="resume-section">
  <h2>Skills</h2>
  <ul>
    <li>Programming Languages: C++, Python, Java</li>
    <li>Tools: Jekyll, Octave, Radare2</li>
    <li>Platforms: Linux (Garuda, Mint), Android</li>
  </ul>
</div>
