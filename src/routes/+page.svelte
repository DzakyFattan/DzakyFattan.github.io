<script>
	import src from "/src/lib/images/profile-img.jpeg";
	import Education from "./Education.svelte";
	import ProjectCard from "./ProjectCard.svelte";
	import ContactCard from "./ContactCard.svelte";

	const educations = [
		{color: "start", title: "Institut Teknologi Bandung", description: "Bachelor of Informatics", date: "2020"},
		{color: "def", title: "SMA Negeri 1 Medan", description: "Senior High School", date: "2017"},
		{color: "def", title: "SMP Negeri 1 Medan", description: "Junior High School", date: "2014"},
		{color: "def", title: "SD Harapan 2 Medan", description: "Elementary School", date: "2008"},
		{color: "end", title: "TK Harapan 1 Medan", description: "Kindergarten", date: "2006"},
	]

	const projects = [
	  	{
	    	name: "Image Compressor",
	    	year: 2021,
	    	description: "Image Compression Web App using EigenVector Technique in Python",
	    	techStack: ["Python", "Vue", "Flask"],
			link: "https://github.com/DzakyFattan/EigenVector-SimpleImageCompressor"
	  	},
	  	{
	  		name: "Usada Carbon Tracker",
	  	  	year: 2021,
	  	  	description: "Carbon Tracking Desktop App with GUI",
	  	  	techStack: ["Python", "PyQt5"],
			link: "https://github.com/DzakyFattan/Usada-Carbon-Tracker"
	  	},
	  	{
	  	  	name: "RockPaperScissors++",
	  	  	year: 2022,
	  	  	description: "Turn-based card fighting game",
	  	  	techStack: ["Java"],
			link: "https://github.com/DzakyFattan/RockPaperScissorPlusPlus"
	  	},
	  	{
	  	  	name: "DNATrain",
	  	  	year: 2022,
	  	  	description: "DNA Pattern Matching Web App for diagnosing sickness using KMP and Boyer-Moore Algorithms in Golang",
	  	  	techStack: ["Golang", "Node", "SQL"],
			link: "https://github.com/DzakyFattan/dnatrain_patternmatch"
	  	},
	  	{
	  	  	name: "MayanOS",
	  	  	year: 2022,
	  	  	description: "A Very Basic Operating System with very limited functions",
	  	  	techStack: ["C", "Assembly"],
			link: "https://github.com/DzakyFattan/mayanos"
	  	},
	  	{
	  	  	name: "Folder Crawler",
	  	  	year: 2022,
	  	  	description: "Files and Folders Search using BFS and DFS",
	  	  	techStack: ["C#", "Visual Studio"],
			link: "https://github.com/DzakyFattan/BFS-DFS-FolderCrawler"
	  	},
	  	{
	  	  	name: "Adoribu",
	  	  	year: 2022,
	  	  	description: "Basic Music Player Web App with various Web Tech Stacks",
	  	  	techStack: ["PHP", "HTML", "CSS", "JS", "React", "Node", "Express", "Java", "SQL"],
			link: "https://github.com/DzakyFattan/Binotify-AdoRibu"
	  	},
	  	{
	  	  	name: "Majika Unbound",
	  	  	year: 2023,
	  	  	description: "Android Application with Twibbon, purchases, and QR Scan Features",
	  	  	techStack: ["Android", "Kotlin"],
			link: "https://github.com/DzakyFattan/Majika-Unbound"
	  	},
	  	{
	  	  	name: "SakuGwej",
	  	  	year: 2023,
	  	  	description: "Money Management Progressive Web App",
	  	  	techStack: ["VueTS", "TailwindCS"],
			link: "https://github.com/DzakyFattan/SakuGwej-Frontend"
	  	}
	];

	const contacts = [
		{ name: "Email", text: "dzaky.fattan@gmail.com", link: "mailto:dzaky.fattan@gmail.com"},
		{ name: "WhatsApp", text: "+628116012019", link: "https://wa.me/628116012019"},
		{ name: "GitHub", text: "dzakyfattan", link: "https://github.com/DzakyFattan" },
		{ name: "Instagram", text: "dzakfr1006", link: "https://www.instagram.com/dzakfr1006/"},
		{ name: "Twitter", text: "TheEnderDuck", link: "https://twitter.com/TheEnderDuck"},
	]
</script>

<section id="top" class="
h-screen 
my-0 px-8 sm:px-16 
flex flex-col-reverse md:flex-row
justify-center items-center 
gap-8 md:gap-16
bg-gradient-to-br from-rose-600 to-orange-400 
">
	<div class="flex flex-col text-white">
		<h1 class="font-normal text-start text-3xl sm:text-5xl">Hi, I'm <strong>Dzaky Fattan Rizqullah</strong></h1>
		<p class="text-lg sm:text-2xl">
			A passionate Software Engineer, lowkey Graphic Designer, 
			and always motivated to improve towards near-perfections.
			and An Audio Engineer who always keeping up with trends 
		</p>
	</div>
	<img {src} alt="Dzaky Fattan Rizqullah" class="
	shadow-md 
	w-48 sm:w-64
	rounded-xl sm:rounded-3xl 
	"/>
	<span class="h-8 block sm:hidden"></span>
</section>

<section id="educations" class="text-center">
	<h1 class="mb-0 sm:text-4xl">Educations</h1>
	<p class="text-neutral-400 text-sm sm:text-base">My lifetime learning journey</p>
	<br>
	{#each educations as education}
		<Education {...education}/>
	{/each}
</section>

<section id="projects" class="m-4 p-4 bg-stone-800 rounded-lg text-center sm:text-lg md:text-2xl">
	<h1 class="mb-0 sm:text-4xl">Projects</h1>
	<p class="text-neutral-400 text-sm sm:text-base">Programming, programming, programming</p>
	<br>
	<div class="grid auto-cols-min gap-4 justify-center justify-items-center" 
	style="grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));">
		{#each projects as project}
			<ProjectCard {...project}/>
		{/each}
	</div>
</section>

<section id="contacts" class="
h-fit p-4 my-0 
text-white text-center sm:text-lg md:text-2xl
bg-gradient-to-br from-orange-400 to-rose-600">
	<h1 class="mb-0 sm:text-4xl">Contacts</h1>
    <p class="text-white text-sm sm:text-base">Get in touch with me!<br></p>
	<br>
	<div class="grid auto-cols-min gap-4 justify-center justify-items-center" 
	style="grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));">
		{#each contacts as contact}
			<ContactCard {...contact}/>
		{/each}
	</div>
</section>