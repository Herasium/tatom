<script>
    import Header from "$lib/elements/header.svelte"
    import Navbar from "$lib/elements/navbar.svelte"

    import blockcoin from "$lib/img/blockcoin.png"

    function goto() {
        window.location.href = "https://blockcoin.social"
    }

</script>


<div id="top-container">
    <Header />
    <Navbar id="nav"/>
</div>

<div id="main">
    <div class="img">
        <div class="textcontainer" on:click={goto}>
            <img src={blockcoin} />
            <div class="text verysmall">Blockcoin</div>
        </div>
    </div>
</div>

<style>
    .text {
        font-family: "Montserrat", sans-serif;
        color:white;
        font-size: 50px;
        text-align: center;
        margin-top: 20px;
    }

    .small {
        font-size: 40px;
    }
    .verysmall {
        font-size: 30px;
    }

    #top-container {
        position: absolute;
        top:0;
        left:0;
        display: flex;
        justify-content: flex-start;
        align-items: flex-start;
        width: 100%;
        flex-direction: column;
    }

    #main {
        margin-top: 5%;
        position: absolute;
        top:0;
        left: 0;
        width: 100%;
        height: auto;
        min-height: 70%;
        display: flex;
        justify-content: flex-start;
        align-items: center;
        flex-direction: column;
    }

    .img {
        margin-top: 20px;
        width:30%;
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-direction: row;
    }

    .img img {
        border-radius: 16px;
        width:120px;
        height: 120px;
    }
    
    .textcontainer {
        cursor: pointer;
        width:30%;
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-direction: column;
    }
    .textcontainer div{
        width: 100%;
    }

</style>