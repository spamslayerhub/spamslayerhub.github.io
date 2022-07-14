<script lang="ts">
    import Tab from '../../components/utils/Tab.svelte';
    import Project from '../TitledLi.svelte';
</script>

<div id="projects">
    <h1>Our Projects</h1>

    <ol>
        <Project
            title="HSpamSlayer"
            href="https://github.com/guiloj/HSpamSlayer"
            target="_blank"
        >
            <Tab />A bot made to keep away undesired cosspost spam from
            malicious subreddits hosted by bad actors trying to promote scam
            links. To get this service you just need to follow
            <a
                href="https://github.com/guiloj/HSpamSlayer#setup"
                target="_blank">these instructions</a
            >. Also if you know python feel free to
            <a
                href="https://github.com/guiloj/HSpamSlayer/blob/master/doc/contribute.md"
                target="_blank">contribute</a
            >!
        </Project>
        <Project
            title="AutoMod Anti-Spam Cheat Sheet"
            href="/projects/automod-sheet/"
        >
            <Tab />A big compilation of essential anti-spam rules for Auto Mod
            that will help you filter unwanted links and messages from your
            comments and posts. A page dedicated to this is coming soon!
        </Project>
    </ol>
</div>

<style>
    #projects {
        padding-top: var(--default-top-padding);
    }
    #projects h1 {
        text-transform: capitalize;
        text-align: center;
    }

    #projects ol {
        list-style: decimal-leading-zero;
        margin-left: var(--default-text-block-margin-size);
        margin-right: var(--default-text-block-margin-size);
    }
</style>
