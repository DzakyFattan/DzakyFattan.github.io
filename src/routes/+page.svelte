<script>
	import src from "/src/lib/images/profile-img.jpeg";
	import Education from "./Education.svelte";
</script>

<section id="top" class="flex flex-col-reverse justify-center items-center h-screen gap-16 my-0 bg-gradient-to-br from-rose-600 to-orange-400 px-16 md:flex-row px-16">
	<div class="flex flex-col text-white">
		<h1 class="font-normal text-start text-4xl md:text-5xl">Hi, I'm <strong>Dzaky Fattan Rizqullah</strong></h1>
		<p class="text-xl md:text-2xl">
			A passionate Software Engineer, lowkey Graphic Designer, 
			and An Audio Engineer who always keeping up with trends 
			and always motivated to improve towards near-perfections.
		</p>
	</div>
	<img {src} alt="Dzaky Fattan Rizqullah" class="shadow-md rounded-3xl w-64"/>
</section>

<section id="educations" class="text-center">
	<h1 class="mb-0">Educations</h1>
	<p class="text-base text-neutral-400">My lifetime learning journey</p>
	<br>
	<Education color = "start" title="Institut Teknologi Bandung" description="Bachelor of Informatics" date="2020 - Now"/>
	<Education title="SMA Negeri 1 Medan" description="Senior High School" date="2017 - 2020"/>
	<Education title="SMP Negeri 1 Medan" description="Junior High School" date="2014 - 2017"/>
	<Education title="SD Harapan 2 Medan" description="Elementary School" date="2008 - 2014"/>
	<Education color = "end" title="TK Harapan 1 Medan" description="Kindergarten" date="2006 - 2008"/>
</section>

<section id="projects" class="text-lg m-4 py-4 px-8 bg-stone-800 rounded-lg text-center md:text-2xl">
	<h1 class="mb-0">Projects</h1>
	<p class="text-base text-neutral-400">Programming, programming, programming</p>
	<br>
	<p>Image Compressor (2021) - Image Compression Web App using EigenVector Technique in Python - Python, Vue, Flask</p>
	<p>Usada Carbon Tracker (2021) - Carbon Tracking Desktop App with GUI - Python, PyQt5</p>
	<p>RockPaperScissors++ (2022) - Turn-based card fighting game - Java</p>
	<p>DNATrain (2022) - DNA Pattern Matching Web App for diagnosing sickness using KMP and Boyer-Moore Algorithms in Golang - Golang, Node, SQL</p>
	<p>MayanOS (2022) - A Very Basic Operating System with very limited functions - C, Assembly</p>
	<p>Folder Crawler (2022) - Files and Folders Search using BFS and DFS - C#, Visual Studio</p>
	<p>Adoribu (2022) - Basic Music Player Web App with various Web Tech Stacks - PHP, HTML, CSS, JS, React, Node, Express, Java, SQL</p>
	<p>Majika Unbound (2023) - Android Application with Twibbon, purchases, and QR Scan Features - Android, Kotlin</p>
	<p>SakuGwej (2023) - Money Management Progressive Web App - VueTS, TailwindCS</p>
</section>

<section id="contacts" class="h-fit py-4 mb-0 text-white bg-gradient-to-br from-orange-400 to-rose-600">
	<h1 class="text-2xl">Contacts</h1>
    <p class="text-xl text-center">In Progress... <br></p>
</section>