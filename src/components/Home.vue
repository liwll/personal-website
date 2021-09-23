<template>
    
    <div id="bio">
      <div id="name">Hi, I'm <span style="color: #228b22; font-size: 1.8em;">Will Li</span></div>
      <img id="picture" src="../../public/me.jpg" alt="A picture of me">
      <div class="container">
        <div id="history">
          <div><span class="history-item">Currently: </span>Undergraduate Researcher @ Stony Brook University</div>
          <div><span class="history-item">Previously: </span>Software Engineer Intern @ Optum</div>
        </div>
        <div id="icons">
          <a href="https://github.com/liwll"><i class="bi bi-github"></i></a>
          <a href="https://www.linkedin.com/in/liwll/"><i class="bi bi-linkedin"></i></a>
          <a href="mailto:will.li@stonybrook.edu"><i class="bi bi-envelope-fill"></i></a>
          <a href="https://drive.google.com/file/d/1RGFoJ43YIma4estjR4f6dk2g5nyS_1LS/view?usp=sharing"><i class="bi bi-file-earmark-text-fill"></i></a>
        </div>
      </div>
      <div class="container">
        <span id="quote-text">"Man's reach exceeds his imagination!" - Robert Angier, <em>The Prestige</em></span>
      </div>
    </div>
    <div id="about-me">
      <h1>About Me</h1>
      <div id="intro-short">
        Hello! I am a student at Stony Brook University with a passion for Computer Science. 
        I love building different websites and apps, 
        but I'm also super interested in researching fields 
        outside of software engineering such as deep learning and computer vision.
        In my free time, I enjoy learning new languages & skills, making music, and reading books. 
        <br><br>
        My friends describe me as easy-going and friendly (although they may be a little biased!).
        It's a pleasure for me to meet and talk to new people, especially since everyone has unique stories about their lives. 
        In the future, I plan to travel the world in the hope of gaining more wisdom and learning about different cultures.
      </div>
    </div>
    <Projects/>
</template>

<script>
export default {
  name: 'Home',
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
h1 {
  border-bottom: 1px solid #228b22;
  padding-bottom: 0.25em;
}
#picture {
  display: block;
  width: 30%;
  margin: 1em 0;
  border-radius: 25px;
}
#bio {
  margin: 5em auto;
  width: 50%;
}
#name {
  display: block;
  font-size: 3em;
  margin: 0.5em auto;
}
.container {
  border: 1px solid #228b22;
  border-radius: 5px;
  width: fit-content;
  padding: 9px;
  margin: 1em 0;
}
#history {
  margin-bottom: 1em;
}
.history-item {
  color: #228b22;
  font-weight: bold;
}
a:visited, a:link {
  color: inherit;
}
i {
  font-size: 2em;
  margin-right: 0.5em;
  transition: 100ms ease-in-out;
}
i:hover {
  color: #228b22;
  /* color: #ED960B; */
}
#about-me {
  width: 50%;
  margin: 5em auto;
}
</style>
