<script>
    export let name = "Name";
    export let year = 2020;
    export let description = "Description";
    export let techStack = ["",];
    export let link = "";
</script>

<a href={link} class="
w-full h-48 p-4 rounded-lg shadow-lg 
flex flex-col
justify-center items-center
bg-gradient-to-br from-rose-600 to-orange-400
transition ease-in-out duration-300
hover:outline hover:outline-offset-4 hover:outline-white
">
    <span class="font-bold text-lg">{name}</span>
    <span class="text-sm">{year} · {description}</span>
    <span class="text-sm">{techStack.join(", ")}</span>
</a>