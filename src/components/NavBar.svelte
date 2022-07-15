<script lang="ts">
    export let home: string;
    export let about: string;
    export let projects: string;
    export let tools: string;

    let switchToTheme = 'dark';

    function toggleTheme() {
        window.document.body.classList.toggle('dark-mode');
        switchToTheme = window.document.body.classList.contains('dark-mode')
            ? 'light'
            : 'dark';
    }
</script>

<nav id="navbar">
    <ul>
        <a href={home}>
            <li>home</li>
        </a>
        <a href={about}>
            <li>about</li>
        </a>
        <a href={projects}>
            <li>projects</li>
        </a>
        <a href={tools}>
            <li>tools</li>
        </a>
        <!-- svelte-ignore a11y-invalid-attribute -->
        <a href="javascript:void(0);" on:click={toggleTheme}>
            <li id="theme-toggle">{switchToTheme} theme</li>
        </a>
    </ul>
</nav>
