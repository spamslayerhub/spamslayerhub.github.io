<script lang="ts">
    import taiga from '../../imgs/taiga.png';
</script>

<div id="home">
    <img id="taiga-icon" src={taiga} alt="taiga" />
    <h1>SpamSlayerHub</h1>
    <p>where mod tools live</p>
</div>

<style>
    #home {
        padding-top: 180px;
        text-align: center;
    }
    #home img {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 250px;
        height: auto;
    }
    #home h1 {
        font-size: var(--default-title-font-size);
    }
    #home p {
        text-transform: capitalize;
    }
</style>
