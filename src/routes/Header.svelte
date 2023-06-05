<script>
	export let y = 0;

	let currentY = 0;
	function scrollToTargetAdjusted(id = 'top') {
		if (y == currentY) return;
	    var element = document.getElementById(id);
	    if (element != null) {
	    	var headerOffset = 48;
	    	var elementPosition = element.getBoundingClientRect().top;
	    	var offsetPosition = elementPosition + y - headerOffset;
			currentY = y;
	    	window.scrollTo({
	    		top: offsetPosition,
	    		behavior: "smooth"
	    	});
	    }
	}
</script>

<header class="fixed w-screen flex flex-row bg-black text-white items-center justify-between px-16 md:justify-between">
	<h1 class="text-lg my-2 font-black md:text-2xl">DzakyFattan</h1>
	<nav class="hidden md:inline-block">
		<ul class="flex flex-row gap-8 text-lg">
			<li><button on:click={() => scrollToTargetAdjusted('top')}>Home</button></li>
			<li><button on:click={() => scrollToTargetAdjusted('educations')}>Educations</button></li>
			<li><button on:click={() => scrollToTargetAdjusted('projects')}>Projects</button></li>
			<li><button on:click={() => scrollToTargetAdjusted('contacts')}>Contacts</button></li>
		</ul>
	</nav>
	<span class="md:hidden">
		<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M4 18h16c.55 0 1-.45 1-1s-.45-1-1-1H4c-.55 0-1 .45-1 1s.45 1 1 1zm0-5h16c.55 0 1-.45 1-1s-.45-1-1-1H4c-.55 0-1 .45-1 1s.45 1 1 1zM3 7c0 .55.45 1 1 1h16c.55 0 1-.45 1-1s-.45-1-1-1H4c-.55 0-1 .45-1 1z"/></svg>
	</span>
</header>