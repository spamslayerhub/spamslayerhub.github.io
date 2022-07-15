<script lang="ts">
    import Css from '../components/utils/Css.svelte';

    import Footer from '../components/Footer.svelte';
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
    <Footer />
</main>
