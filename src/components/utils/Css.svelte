<style global>
    @import url('https://fonts.googleapis.com/css2?family=Cousine:ital,wght@0,400;0,700;1,400;1,700&display=swap');

    :global(:root) {
        --brightest-r: 242;
        --brightest-g: 242;
        --brightest-b: 242;
        --darkest-r: 59;
        --darkest-g: 60;
        --darkest-b: 64;
        --brightest: var(--brightest-r),var(--brightest-g),var(--brightest-b);
        --darkest: var(--darkest-r),var(--darkest-g),var(--darkest-b);

        --brighter-value: 0.875;
        --bright-value: 0.75;
        --semi-bright-value: 0.625;
        --medium-value: 0.5;
        --semi-dark-value: 0.375;
        --dark-value: 0.25;
        --darker-value: 0.125;

        --brighter-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--brighter-value));
        --brighter-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--brighter-value));
        --brighter-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--brighter-value));
        --bright-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--bright-value));
        --bright-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--bright-value));
        --bright-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--bright-value));
        --semi-bright-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--semi-bright-value));
        --semi-bright-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--semi-bright-value));
        --semi-bright-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--semi-bright-value));
        --medium-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--medium-value));
        --medium-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--medium-value));
        --medium-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--medium-value));
        --semi-dark-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--semi-dark-value));
        --semi-dark-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--semi-dark-value));
        --semi-dark-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--semi-dark-value));
        --dark-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--dark-value));
        --dark-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--dark-value));
        --dark-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--dark-value));
        --darker-r: calc(var(--darkest-r) + (var(--brightest-r) - var(--darkest-r)) * var(--darker-value));
        --darker-g: calc(var(--darkest-g) + (var(--brightest-g) - var(--darkest-g)) * var(--darker-value));
        --darker-b: calc(var(--darkest-b) + (var(--brightest-b) - var(--darkest-b)) * var(--darker-value));

        --brighter: var(--brighter-r),var(--brighter-g),var(--brighter-b);
        --bright: var(--bright-r),var(--bright-g),var(--bright-b);
        --semi-bright: var(--semi-bright-r),var(--semi-bright-g),var(--semi-bright-b);
        --medium: var(--medium-r),var(--medium-g),var(--medium-b);
        --semi-dark: var(--semi-dark-r),var(--semi-dark-g),var(--semi-dark-b);
        --dark: var(--dark-r),var(--dark-g),var(--dark-b);
        --darker: var(--darker-r),var(--darker-g),var(--darker-b);

        --hss-red-h: 355;
        --hss-green-h: 134;
        --hss-blue-h: 220;
        --hss-yellow-h: 33;
        --hss-orange-h: 12;
        --hss-default-s: 38%;
        --hss-vibrant-s: 60%;
        --hss-muted-s: 30%;
        --hss-default-l: 50%;
        --hss-brightest-l: 90%;
        --hss-brighter-l: 80%;
        --hss-bright-l: 70%;
        --hss-semi-bright-l: 60%;
        --hss-semi-dark-l: 40%;
        --hss-dark-l: 30%;
        --hss-darker-l: 20%;
        --hss-darkest-l: 10%;

        --nav-color: rgb(var(--darkest));
        --nav-text-color: rgb(var(--brightest));
        --background-color: rgb(var(--brightest));
        --nav-hover-text-color: rgba(var(--brightest), 0.7);
        --default-text-visited-color: rgb(var(--dark));
        --default-text-color: rgb(var(--darkest));
        --default-font: Cousine, Consolas, Courier, monospace;
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
