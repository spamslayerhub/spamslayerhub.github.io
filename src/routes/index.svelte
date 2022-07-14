<script lang="ts">
    import Css from '../components/utils/Css.svelte';

    import About from '../components/index/About.svelte';
    import Home from '../components/index/Home.svelte';
    import Projects from '../components/index/Projects.svelte';
    import Tools from '../components/index/Tools.svelte';
    import NavBar from '../components/NavBar.svelte';
    // import Tab from '../components/utils/Tab.svelte';
</script>

<Css />

<title>SpamSlayerHub</title>
<main>
    <NavBar home="#home" about="#about" projects="#projects" tools="#tools" />
    <Home />
    <About />
    <Projects />
    <Tools />
    <footer>
        <p>
            Powered by <a href="https://pages.github.com/" target="_blank"
                >GitHub Pages</a
            >
            & <a href="https://svelte.dev/">Svelte</a>
        </p>
    </footer>
</main>

<style>
    footer {
        margin-top: var(--default-top-padding);
        position: absolute;
        height: fit-content;
        text-align: center;
        width: 100%;
        left: 0;
        background-color: var(--nav-color);
    }
    footer p {
        padding: 0;
        margin: 10px;
    }
    footer p,
    footer a {
        color: var(--nav-hover-text-color);
    }
</style>
