<template>
  <h1>Typist<span class="blinking-caret">|</span></h1>
</template>

<script>
export default {
	name: "AppHeading"
}
</script>

<style scoped>
h1 {
	font-size: 5.0em;
}

.blinking-caret {
  font-weight: 100;
  font-size: 5rem;
  color: #2E3D48;
  -webkit-animation: 1s blink step-end infinite;
  -moz-animation: 1s blink step-end infinite;
  -ms-animation: 1s blink step-end infinite;
  -o-animation: 1s blink step-end infinite;
  animation: 1s blink step-end infinite;
}

@keyframes blink {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-moz-keyframes blink {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-webkit-keyframes blink {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-ms-keyframes blink {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}

@-o-keyframes blink {
  from, to {
    color: transparent;
  }
  50% {
    color: black;
  }
}
</style>
