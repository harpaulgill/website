<template>
  
  <div id="main">
    <head>
    <link href="https://fonts.googleapis.com/css?family=Crimson+Pro:200|Montserrat&display=swap" rel="stylesheet">
    <link rel="shortcut icon" type="image/png" href="/static/hg_logo.png"/>
    </head>
    <div id="nav">
      <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item href="https://github.com/harpaulgill" target="_blank" title="Github"><font-awesome-icon :icon="['fab', 'github']" size="2x" /></b-nav-item>
            <b-nav-item href="https://www.linkedin.com/in/harpaulgill/" target="_blank" title="LinkedIn"><font-awesome-icon :icon="['fab', 'linkedin']" size="2x" /></b-nav-item>
            <b-nav-item href="https://drive.google.com/file/d/1yhK_Jlmu3wUlUmFQppwT37NHe_bmqtps/view" target="_blank" title="Resume"><font-awesome-icon :icon="['far', 'file']" size="2x" /></b-nav-item>
          </b-navbar-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="#about" style="font-size: 20px">About</b-nav-item>
            <b-nav-item href="#skills" style="font-size: 20px">Skills</b-nav-item>
            <b-nav-item href="#experience" style="font-size: 20px">Experience</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
      <div id="title">
        <h1>Harpaul Gill</h1>
        <h4> Softare Developer - University of British Columbia </h4>
        <img  class="pic" src="./assets/headshot.jpg" style="border-radius: 50%" height="400px" width="400px" >
        <img  class="mobile-pic" src="./assets/headshot.jpg" style="border-radius: 50%" height="160px" width="160px" >
      </div>
      <div id="about">
        <h2 class="headers">About Me</h2>
        <P class="intro">Hi, I’m in my last year studying Computer Engineering at the University of British Columbia.
          I am primarily interested in back-end and full-stack software development and have been focussing
          on that for the majority of my degree. Most of my experience comes from working with server side languages,
          but I am also comfortable doing front end development. I was born and raised around Vancouver and enjoy
          the variety of outdoor activities this city offers. In my spare time I enjoy hiking,
          lifting weights, playing sports and reading. When I'm not doing one of those things I’m usually
          tinkering with different frameworks and languages or learning something new.
        </p>
      </div>
      <div id="skills" class="headers">
        <h2 class="headers">Skills</h2>
        <div class="column">
          <h3>Back-end</h3>
          <ul class="skill-list">
            <li>Java</li>
            <li>Python</li>
            <li>C++</li>
            <li>Node.js</li>
            <li>SQL</li>
          </ul>
        </div>
        <div class="column">
          <h3>Front-end</h3>
          <ul class="skill-list">
            <li>JavaScript</li>
            <li>HTML</li>
            <li>CSS</li>
            <li>Vue</li>
            <li>React</li>
          </ul>
        </div>
        <div class="column">
          <h3>General</h3>
          <ul class="skill-list">
            <li>Docker</li>
            <li>AWS</li>
            <li>GCP</li>
            <li>Git</li>
            <li>Agile</li>
          </ul>
        </div>
      </div>
      <div id="experience"  style="padding-top: 150px">
        <h2 >Experience</h2>
        <div class="exp-icons">
          <img class="exp-img" src="./assets/dialpad_logo.jpg" height="250" width="250">
          <img class="exp-img" src="./assets/ca_logo.jpg" height="250" width="250"> 
          <img class="exp-img" src="./assets/ge_logo.jpg" height="250" width="250">
          <img class="exp-img-mobile" src="./assets/dialpad_logo.jpg" height="160" width="160">
          <img class="exp-img-mobile" src="./assets/ca_logo.jpg" height="160" width="160"> 
          <img class="exp-img-mobile" src="./assets/ge_logo.jpg" height="160" width="160">
        </div>
      </div>
      <div id="signatures">
        <h6>Harpaul Gill © 2019</h6>
      </div>
  </div>
</template>

<style>
#main {
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.pic {
  margin-top: 8%;
}

#title {
  margin: 8% 25% 6%;
}

#about {
  margin: -16% 25%;
  padding: 16% 0 10%;
}

#skills {
  margin: -16% 25%;
  padding: 14% 0;
}

#experience {
  margin: 10% 25% 4%;
}

#signatures {
  margin: 6% 25%;
}

.b-navbar-brand {
  font-size: 100px !important;
}

.headers {
  margin-bottom: 4%;
}

.intro {
  text-align: justify;
  margin: 0 8%;
}

h2 {
  text-align: center;
  margin-left: auto;
  margin-right: auto;

}

.skill-list {
  width: 70%;
  margin: auto;
  list-style-type: none;
  padding: 10px;

}

.column {
  float: left;
  width: 33.33%;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

.exp-icons{
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}

.exp-img {
  padding: 0 20px;
}

.mobile-pic, .exp-img-mobile {
  display: none;
}

@media screen and (max-width: 600px) {
  .column {
    width: 100%;
  }

  .skill-list {
    text-align: justify;
    list-style-position: outside;
    margin-left: 30%
  }

  #main {
    margin-left: 0%;
    margin-right: 0%;
  }

  .mobile-pic, .exp-img-mobile {
    display: block;
    margin:0 auto;
  }

  #title {
    margin-top: 20%;
  }

  .exp-img {
    margin:0 auto;
  }

  .pic, .exp-img{
    display: none;
  }
}
</style>
