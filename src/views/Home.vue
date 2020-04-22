<template>
  <div>
    <div class="hero is-cover is-relative is-fullheight-with-navbar has-background-link">
        <div class="hero-body">
            <div class="container">
              <div class="typewriter">
                <h1 class="title is-1 something">Armaan Lala</h1>
                </div>
                <h1 class="subtitle is-2">Software Developer</h1>
                <h1 class="subtitle is-3">Mathmatics and Computer Science Student at Georgia Institute of Technology</h1>
            </div>
        </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "home",
};
</script>

<style  scoped>
* {
  color:white;
}
.something{
  width: min-content;
}
.typewriter h1 {
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: .15em solid orange; /* The typwriter cursor */
  white-space: nowrap; 
  /* margin: 0 auto; */
  animation: 
    typing 1s steps(11, end),
    blink-caret .75s step-end infinite;
}

/* The typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 280px }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}

</style>