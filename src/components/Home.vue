<template>
  <div class="home">
    <div class="about">
      <div id="name"><span id="name-text">Will Li</span></div>
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
        <a href="https://drive.google.com/file/d/1RGFoJ43YIma4estjR4f6dk2g5nyS_1LS/view?usp=sharing"><i class="bi bi-file-earmark-text-fill"></i></a>
      </div>
      <div id="quote">
        <span id="quote-text">"Man's reach exceeds his imagination!" - Robert Angier, <em>The Prestige</em></span>
      </div>
    </div>
    <Projects/>
  </div>
</template>

<script>
import Projects from './Projects.vue'

export default {
  name: 'Home',
  components: {
    Projects
  },
  props: {
    msg: String
  },
  data: function() {
    return {
      Projects: 5
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.about {
  margin: 100px auto;
  width: 50%;

}
#name {
  font-size: 3em;
  margin: 0.33em 0;
}
#name-text {
  transition: 300ms ease-in-out;
}
#name-text:hover {
  color: #ED960B;
  font-size: 1.8em;
}
#bio {
  display: flex;
}
#history {
  margin: 1em 0;
}
a:visited, a:link {
  color: inherit;
}
i {
  font-size: 2em;
  margin-right: 0.5em;
  transition: 300ms ease-in-out;
}
i:hover {
  color: #ED960B;
}
#quote {
  width: fit-content;
  margin: 1em 0;
  padding: 9px;
  border: 1px solid #ED960B;
  border-radius: 5px;
}
</style>
