<script>
  import Intro from "../components/Intro.svelte";
</script>

<style>
.content {
  clip-path: polygon(0 35%, 100% 0, 100% 100%, 0% 100%);
  background-color: #31384A;
}
</style>

<svelte:head>
	<title>
    Hom sweet home
  </title>
</svelte:head>

<!-- Landing view -->
<Intro />

<div class="content bg-blue-600 py-20">
</div>