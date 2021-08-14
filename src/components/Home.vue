<template>
  <div class="home">
    <div class="sidebar">
      <div class="about">
        <h1>Will Li</h1>
        <div id="bio">
          Hello! I am a student at Stony Brook University with a passion for Computer Science. 
          I love building different websites and apps, 
          and I am also super interested in researching deep learning and computer vision.
          My hobbies include learning new languages & skills, making music, and reading books. 
        </div>
        <div id="history">
          <div class="history-item">Currently: Undergraduate Researcher @ Stony Brook University</div>
          <div class="history-item">Previously: Software Engineer Intern @ Optum</div>
        </div>
        <div id="icons">
          <a href="https://github.com/liwll"><i class="bi bi-github"></i></a>
          <a href="https://www.linkedin.com/in/liwll/"><i class="bi bi-linkedin"></i></a>
          <a href="mailto:will.li@stonybrook.edu"><i class="bi bi-envelope-fill"></i></a>
          <a href="#bio"><i class="bi bi-file-earmark-text-fill"></i></a>
        </div>
      </div>
    </div>

    <div class="content">
      <div class="projects">
        <div class="project-card">
          Project
        </div>
        <div class="project-card">
          Project
        </div>
        <div class="project-card">
          Project
        </div>
        <div class="project-card">
          Project
        </div>
        <div class="project-card">
          Project
        </div>
      </div>
      

    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sidebar {
  position: fixed;
  height: 100vh;
  width: 37vw;
  border-right: 1px solid black;
}
.about {
  margin: 33% 100px;
}
#bio {
  display: flex;
}
#history {
  margin: 1.34em 0;
}
a:visited, a:link {
  color: inherit;
}
i {
  font-size: 2em;
  margin-right: 0.5em;
  transition: ease-in-out 0.2s;
}
i:hover {
  color: black;
}
.content {
  position: fixed;
  right: 0;
  height: 100vh;
  width: 63vw;
}
.projects {
  width: 90%;
  margin: 12vh auto;
  display: flex;
  flex-wrap: wrap;
}
.project-card {
  flex: 0 0 calc(45% - 0px);
  height: 200px;
  border: 1px solid black;
  border-radius: 5px;
  padding: 10px;
  margin: 0.5%;
}
</style>
