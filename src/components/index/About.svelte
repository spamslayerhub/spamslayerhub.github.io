<script lang="ts">
    import Tab from '../../components/utils/Tab.svelte';
</script>

<div id="about">
    <h1>About Us</h1>
    <p>
        <Tab />We are a group of reddit moderators that decided to come
        toghether to adress problems we all had with the plataform, notably,
        <b>spam</b>. By adding up our expertise in different fields we were able
        to create different tools and projects to make your life as a moderator
        easier.
    </p>
    <p>
        <Tab />All of the services that we pubicly provide are free and open
        source (<a
            target="_blank"
            href="https://github.com/spamslayerhub/spamslayerhub.github.io"
            ><i>even this very website</i></a
        >), so feel free to experiemnt with your own versions and
        configurations, if you need anything feel free to join our
        development/help
        <a href="https://discord.gg/RkUF87GZWD" target="_blank"
            >discord server</a
        >!
    </p>
    <p style="color: gray; font-style: italic;">
        // team members here probably
    </p>
</div>

<style>
    #about {
        padding-top: var(--default-top-padding);
    }
    #about h1 {
        text-align: center;
        text-transform: capitalize;
    }
    #about p {
        margin-left: var(--default-text-block-margin-size);
        margin-right: var(--default-text-block-margin-size);
    }
</style>
