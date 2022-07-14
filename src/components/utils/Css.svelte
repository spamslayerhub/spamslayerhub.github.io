<style global>
    :global(:root) {
        --nav-color: #333;
        --nav-text-color: #fff;
        --background-color: white;
        --nav-hover-text-color: rgba(255, 255, 255, 0.7);
        --default-text-visited-color: rgb(82, 82, 82);
        --default-text-color: #3d3d3d;
        --default-font: 'Courier New', Courier, monospace;
        --default-p-font-size: 20px;
        --default-title-font-size: 50px;
        --default-h1-font-size: 32px;
        --default-h2-font-size: 24px;
        --default-text-block-margin-size: 20%;
        --default-color-transition: ease-in-out 0.3s;
        --default-top-padding: 60px;
    }
    @media only screen and (max-width: 800px) {
        :global(:root) {
            --default-p-font-size: 20px;
            --default-title-font-size: 40px;
            --default-h1-font-size: 28px;
            --default-h2-font-size: 16px;
            --default-text-block-margin-size: 2%;
            --default-top-padding: 60px;
        }
    }

    :global(body) {
        background-color: var(--background-color);
        transition: var(--default-color-transition);
    }

    :global(body.dark-mode) {
        --nav-color: rgb(218, 218, 218);
        --nav-text-color: rgb(0, 0, 0);
        --nav-hover-text-color: rgba(0, 0, 0, 0.7);
        --background-color: black;
        --default-text-color: #c2c2c2;
        --default-text-visited-color: rgb(182, 182, 182);
    }

    * {
        font-family: var(--default-font);
        /* DEBUG */
        /* outline: 1px solid limegreen !important; */
    }

    h1,
    h2,
    p,
    a {
        color: var(--default-text-color);
    }

    h1 {
        font-size: var(--default-h1-font-size);
    }

    a:visited {
        color: var(--default-text-visited-color);
    }
</style>
