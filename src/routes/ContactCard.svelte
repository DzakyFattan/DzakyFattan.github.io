<script>
    export let name = "Name";
    export let text = "Text"
    export let link = "";
</script>

<a href={link} class="
w-full h-8 px-4 rounded-lg
flex flex-row gap-4
justify-left items-center
bg-black hover:bg-neutral-700
transition ease-in-out
hover:cursor-pointer
">
    <span class="font-bold text-sm">{name}</span>
    <span class="text-sm">{text}</span>
</a>