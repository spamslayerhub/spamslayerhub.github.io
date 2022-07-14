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

<style>
    #navbar {
        position: fixed;
        background-color: var(--nav-color);
        color: var(--nav-text-color);
        top: 0;
        left: 0;
        overflow: auto;
        width: 100%;
        z-index: 100;
        transition: var(--default-color-transition);
    }

    #navbar a {
        color: var(--nav-text-color);
        display: contents;
    }

    #navbar ul {
        list-style: none;
        padding: 0;
        margin: 0;
    }

    #navbar ul li {
        display: inline-block;
        padding: 5px;
        top: 0;
        letter-spacing: normal;
        text-transform: uppercase;
        line-height: 60px;
        margin-left: 30px;
    }

    #navbar ul li:hover {
        color: var(--nav-hover-text-color);
    }

    #navbar ul li#theme-toggle {
        right: 0;
        position: absolute;
        margin-right: 30px;
        margin-left: 0;
    }
    #navbar ul a li {
        font-weight: 600;
        font-size: large;
    }

    @media only screen and (max-width: 800px) {
        #navbar ul li {
            padding: 0;
            line-height: 50px;
            margin-left: 4px;
            font-size: 15px !important;
        }
        #navbar ul li#theme-toggle {
            right: 0;
            position: absolute;
            margin-right: 4px;
            font-size: 15px;
            margin-left: 0;
        }
    }
</style>
