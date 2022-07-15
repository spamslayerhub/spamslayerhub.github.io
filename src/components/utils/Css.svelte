<style global>
    @import url('https://fonts.googleapis.com/css2?family=Cousine:ital,wght@0,400;0,700;1,400;1,700&display=swap');

    :global(:root) {
        --brightest-r: 242;
        --brightest-g: 242;
        --brightest-b: 242;
        --darkest-r: 59;
        --darkest-g: 60;
        --darkest-b: 64;
        --brightest: var(--brightest-r), var(--brightest-g), var(--brightest-b);
        --darkest: var(--darkest-r), var(--darkest-g), var(--darkest-b);

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

        --brighter: var(--brighter-r), var(--brighter-g), var(--brighter-b);
        --bright: var(--bright-r), var(--bright-g), var(--bright-b);
        --semi-bright: var(--semi-bright-r), var(--semi-bright-g), var(--semi-bright-b);
        --medium: var(--medium-r), var(--medium-g), var(--medium-b);
        --semi-dark: var(--semi-dark-r), var(--semi-dark-g), var(--semi-dark-b);
        --dark: var(--dark-r), var(--dark-g), var(--dark-b);
        --darker: var(--darker-r), var(--darker-g), var(--darker-b);
    }

    :global(:root) {
        --hss-red-h: 355;
        --hss-green-h: 134;
        --hss-blue-h: 218;
        --hss-yellow-h: 33;
        --hss-orange-h: 25;
        --hss-default-s: 40%;
        --hss-vibrant-s: 65%;
        --hss-semi-vibrant-s: 55%;
        --hss-semi-muted-s: 33%;
        --hss-muted-s: 25%;
        --hss-default-l: 50%;
        --hss-brightest-l: 80%;
        --hss-brighter-l: 72%;
        --hss-bright-l: 64%;
        --hss-semi-bright-l: 57%;
        --hss-semi-dark-l: 43%;
        --hss-dark-l: 36%;
        --hss-darker-l: 28%;
        --hss-darkest-l: 20%;
    }

    :global(:root) {
        --nav-color: hsl(var(--hss-red-h), var(--hss-vibrant-s), var(--hss-darker-l));
        --nav-text-color: rgb(var(--brighter));
        --background-color: rgb(var(--brighter));
        --nav-hover-text-color: rgba(var(--brighter), 0.8);
        --default-text-color: rgb(var(--darkest));
        --title1-color: hsl(var(--hss-red-h), var(--hss-semi-vibrant-s), var(--hss-semi-dark-l));
        --title-link-color: hsl(var(--hss-orange-h), var(--hss-semi-vibrant-s), var(--hss-semi-dark-l));
        --title-link-visited-color: hsl(var(--hss-orange-h), var(--hss-semi-muted-s), var(--hss-default-l));
        --link-color: hsl(var(--hss-blue-h), var(--hss-semi-vibrant-s), var(--hss-default-l));
        --link-visited-color: hsl(var(--hss-blue-h), var(--hss-semi-muted-s), var(--hss-semi-bright-l));

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
        --nav-color: hsl(var(--hss-blue-h), var(--hss-default-s), var(--hss-brighter-l));
        --nav-text-color: rgb(var(--darkest));
        --nav-hover-text-color: rgba(var(--darkest), 0.8);
        --background-color: rgb(var(--darkest));
        --default-text-color: rgb(var(--bright));
        --title1-color: hsl(var(--hss-blue-h), var(--hss-vibrant-s), var(--hss-brighter-l));
        --title-link-color: hsl(var(--hss-blue-h), var(--hss-semi-vibrant-s), var(--hss-brighter-l));
        --title-link-visited-color: hsl(var(--hss-blue-h), var(--hss-default-s), var(--hss-semi-bright-l));
        --link-color: hsl(var(--hss-yellow-h), var(--hss-semi-vibrant-s), var(--hss-brighter-l));
        --link-visited-color: hsl(var(--hss-yellow-h), var(--hss-semi-muted-s), var(--hss-semi-bright-l));
    }

    * {
        font-family: var(--default-font);
        /* DEBUG */
        /* outline: 1px solid limegreen !important; */
    }

    h2,
    p,
    li::marker {
        color: var(--default-text-color);
    }
    h1 {
        color: var(--title1-color);
    }
    a.title-link {
        color: var(--title-link-color) !important;
    }
    a.title-link:visited {
        color: var(--title-link-visited-color) !important;
    }
    a {
        color: var(--link-color);
    }
    a:visited {
        color: var(--link-visited-color);
    }

    h1 {
        font-size: var(--default-h1-font-size);
    }

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
        transition: 0.2s;
    }

    #navbar ul li:hover {
        color: var(--nav-hover-text-color);
        transition: 0.2s;
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
