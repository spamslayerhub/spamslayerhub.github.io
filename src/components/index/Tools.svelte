<script lang="ts">
    import Tab from '../../components/utils/Tab.svelte';
    import Tool from '../TitledLi.svelte';
</script>

<div id="tools">
    <h1>Project Tools</h1>
    <ol>
        <Tool
            title="HSpamSlayer Sub Config Helper"
            href="/tools/hss-sub-configs"
        >
            <Tab />A tool to help you manage and create a HSpamSlayer
            configuration files for specific subreddits that you moderate, with
            helpful descriptions, great defaults and filters that help your
            config file be processed without any errors.
        </Tool>
    </ol>
</div>

<style>
    #tools {
        padding-top: var(--default-top-padding);
    }
    #tools h1 {
        text-transform: capitalize;
        text-align: center;
    }

    #tools ol {
        list-style: decimal-leading-zero;
        margin-left: var(--default-text-block-margin-size);
        margin-right: var(--default-text-block-margin-size);
    }
</style>
