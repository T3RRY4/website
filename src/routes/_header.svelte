<script>
	import { scrollto } from "svelte-scrollto";
</script>

<header>
	<a class="logo" href="/">terry.dev</a>
	<nav>
		<a use:scrollto={".greeting"} href="/">#home</a>
		<a use:scrollto={".about"} href="/">#about</a>
		<a use:scrollto={".work"} href="/">#work</a>
		<a use:scrollto={"footer"} href="/">#contacts</a>
	</nav>
</header>