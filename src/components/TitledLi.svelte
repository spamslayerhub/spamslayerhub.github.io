<script lang="ts">
    export let title: string;
    export let href: string;
    export let target = '_self';
</script>

<li>
    <h2>
        <a class="title-link" {href} {target}>{title}</a>
    </h2>
    <p>
        <slot />
        <!-- This is what goes inside the component tag: <TitledLi title="" href=""> this </TitledLi> -->
    </p>
</li>

<style>
    h2 {
        text-transform: capitalize;
    }
    .title-link,
    .title-link:visited {
        color: var(--default-text-color);
    }
</style>
