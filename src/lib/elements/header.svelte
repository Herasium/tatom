<script>
    import logo from "$lib/img/Logo.png"
    import { onMount } from "svelte";
    var page = ""
    onMount(() => {
        var path = window.location.pathname;
        page = path.split("/").pop();
        page = page[0].toUpperCase() + page.slice(1);

    })

</script>

<div id="header">
    <img src={logo} />
    <div class="text">Tatom Corp.</div>
</div>
<div id="page">{page}</div>

<style>
    #header {
        z-index: 10;
        width: 90%;
        display: flex;
        justify-content: flex-start;
        align-items: center;
        margin-top: 10px;
        margin-left: 10px;
    }

    #header img {
        z-index: 10;
    }

    .text {
        font-family: "Montserrat", sans-serif;
        color:white;
        font-size: 44px;
        margin: 15px;
    }

    #page {
        z-index: 10;
        width: 100%;
        top:0;
        position: absolute;
        left: 0;
        margin-top: 10px;
        text-align: center;
        font-family: "Montserrat", sans-serif;
        color:white;
        font-size: 44px;
    }
</style>
