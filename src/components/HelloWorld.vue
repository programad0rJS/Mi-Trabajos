<template>
  <div class="hello">
    <header class="Header">
    <h1>#ProgramadorFitness</h1>

    <p>
      Bienvenid@s a #ProgramadorFitness, serie de videos, donde te daré consejos para llevar una vida saludable y evitar el sedentarismo.
      Recuerda... mente sana en cuerpo sano :)
    </p>
    <nav>
      <a href="https://www.youtube.com/playlist?list=PLvq-jIkSeTUbJFWQx8gcy1MK0lTLrdLR9" target="_blank" title="YouTube">
        <i class="fab fa-youtube"></i>
      </a>
      <a href="https://facebook.com/programadorfitness" target="_blank" title="Facebook">
        <i class="fab fa-facebook"></i>
      </a>
      <a href="https://www.instagram.com/explore/tags/ProgramadorFitness/" target="_blank" title="Instagram">
        <i class="fab fa-instagram"></i>
      </a>
    </nav>
  </header>
  <main class="Main">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/9oQIylJ-JpU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </main>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
/* Custom Properties */
:root {
  --main-color: #F0DB4F;
  --main-modal-color: rgba(240, 219, 79, .5);
  --second-color: #2B2B2B;
  --second-modal-color: rgba(43, 43, 43, .5);
}

html {
  box-sizing: border-box;
  font-family: 'Raleway', sans-serif;
  font-size: 16px;
  line-height: 1.6;
  color: var(--second-color);
  background-color: var(--main-modal-color);
}

*,
*:after,
*:before {
  box-sizing: inherit;
  padding: 0;
  margin: 0;
}

body {
  margin: 2rem auto;
  overflow-x: hidden;
  max-width: 800px;
}

a {
  font-weight: bold;
  color: var(--second-color);
  transition: all .3s ease-out;
}

a:hover {
  color: var(--second-modal-color);
}

p {
  padding: 1rem;
  font-size: 1.25rem;
}

::selection {
  background-color: var(--second-color);
  color: var(--main-color);
}

.Header {
  display: flex;
  flex-direction: column;
  text-align: center;
}

.Header h1 { word-wrap: break-word; }

.Header img {
  margin: 0 auto;
  display: block;
  max-width: 150px;
  border-radius: 50%;
}

.Header nav {
  padding: 2rem 0;
  display: flex;
  justify-content: space-evenly;
  font-size: 3rem;
}

.Main {
  position: relative;
  margin: 0 auto;
  padding-bottom: 56.25%; /* 16:9 */
}

.Main iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
</style>
