<script>
  export let segment;
</script>

<style>
nav {
  background-color: #31384A;
  z-index: 9999;
  display: flex;
  flex-grow: inherit;
  justify-content: space-between;
  align-items: center;
}

.resume-btn {
  border: 2px solid #C6FFC5;
  color: #C6FFC5;
  padding: 0.4em 0.8em;
  font-size: 1.2em;
  cursor: pointer;
  border-radius: .3em;
  transition: 0.25s ease-out;
}

.resume-btn:hover {
  background-color: #C6FFC5;
  color: #3E465B;
}

a {
  text-decoration: none;
  margin-left: 1em;
  margin-right: 1em;
  font-size: 1.2em;
}

@media only screen and (max-width: 600px) {
  .sig {
    visibility: hidden;
    display: none;
  }

  nav {
    padding-top: 1.5em;
    padding-bottom: 1.5em;
    font-size: .85em;
    align-content: center;
    justify-content: center;
  }
}
</style>

<nav class="px-2 md:px-12 fixed w-full shadow-xl">
  <div class="sig">
    <a href=".">
    <svg height="40" viewBox="0 0 107 76" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M11.1235 36.536C19.9092 28.1594 38.4942 12.4319 42.5491 16.5348C47.6177 21.6633 19.7402 53.973 22.7814 60.1273C25.8226 66.2815 64.3442 34.4846 56.7413 29.8689C49.1383 25.2533 42.0422 36.1935 45.0834 40.6389C48.1246 45.0842 56.2344 52.9473 61.303 44.7417C65.3579 38.1772 62.9926 17.0476 61.303 7.3034L81.0707 75C79.5501 54.6568 74.9883 11.8165 68.906 3.20058C73.8057 11.5772 83.8078 29.9715 84.6187 36.536C85.6325 44.7417 77.5227 9.86767 86.6462 14.9962C95.7697 20.1247 95.2629 38.0746 99.3178 27.3047C103.373 16.5348 107.428 7.3034 99.3178 3.20058C92.8299 -0.0816815 31.736 37.7327 2 57.0501" stroke="white" stroke-width="5"/>
    </svg>
    </a>
  </div>

  <div class="block">
    <a href="about" class:font-bold='{segment === "about"}' >About</a>
    <a href="#!">Skills</a>
    <a href="#!">Projects</a>

    <a href='{segment === "contact" ? "." : "contact"}' class="resume-btn pt-12"
    >{segment === "contact" ? "Home" : "Contact"}</a>
  </div>
</nav>