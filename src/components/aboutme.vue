<script setup lang="ts">
</script>

<template>
  <div class="hero">
    <div class="left">
        <div class="whoIAm">Who I am?</div>
        <div class="about">
          My name is ABU SAID. I am a professional and enthusiastic programmer in my daily life. I am a quick learner with a self-learning attitude. I love to learn and explore new technologies and am passionate about problem-solving. I love almost all the stacks of web application development and love to make the web more open to the world. My core skill is based on JavaScript and I love to do most of the things using JavaScript. I am available for any kind of job opportunity that suits my skills and interests.
        </div>
    </div>

    <div class="center">
        <img src="../assets/passport.JPG" alt="About Me Image" />
            <div class="about-tag">ABOUT ME</div>
    </div>

  </div>
</template>

<style scoped>
.hero {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  color: #ffffff;
  gap: 15vw;
  margin-top: 8vh;
}

.left {
  flex: 1;
}

.center {
  display: flex;
  align-items: center;
  gap: 5vw;
  flex: 0 0 280px;
}

.center img {
  width: 10vw;
  height: 20vh;
  border-radius: 12px;
  object-fit: cover;
  object-position: center 5%;
  filter: grayscale(100%);
  transition: filter 0.5s ease, transform 0.5s ease; /* smooth transition */
}

.center img:hover {
  filter: grayscale(0%);
  transform: scale(1.1);
}


.whoIAm {
  font-size: 1.5rem;
  color: #16f2b3;
}

.about {
  margin-top: 1rem;
  font-size: 1.2rem;
  line-height: 1.6;
  text-align: justify;
}

.about-tag {
  padding: 0.75rem 1.5rem;
  border-radius: 8px;
  font-size: 1.2rem;
  background-color: #1a1443;
  transform: rotate(90deg);
  margin-top: -25%;
  white-space: nowrap;
}


.about-tag::after {
  content: "";
  position: absolute;
  left: 100%;
  top: 50%;
  transform: translateY(-50%);
  width: 70%;
  height: 2px;
  background-color: #1a1443;
  border-radius: 2px;
}


@media (max-width: 768px) {
  .hero {
    flex-direction: column;
    gap: 2rem;
    align-items: center;
    margin-top: 4vh;
  }

  .left {
    text-align: center;
  }

  .center {
    flex: none;
    gap: 1rem;
    flex-direction: column;
  }

  .about-tag {
    display: none;
  }

  .center img {
    width: 200px;
    height: 200px;
  }
}
@media (max-width: 1200px) {
  .about-tag {
    display: none; /* hide the rotated tag */
  }

  .whoIAm {
    font-size: 1.3rem; /* slightly smaller */
  }

  .about {
    font-size: 1rem; /* reduce font size to fit */
    line-height: 1.4;
  }

  .center img {
    width: 220px; /* slightly smaller image */
    height: 220px;
  }
}

/* For smaller screens */
@media (max-width: 992px) {
  .whoIAm {
    font-size: 1.2rem;
  }

  .about {
    font-size: 0.95rem;
  }

  .center img {
    width: 200px;
    height: 200px;
  }
}
</style>
