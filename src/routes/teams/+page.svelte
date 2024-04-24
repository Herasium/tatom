<script>
    import Header from "$lib/elements/header.svelte"
    import Navbar from "$lib/elements/navbar.svelte"

    import hera from "$lib/img/hera.png"
    import s4il from "$lib/img/s4il.png"

    import birdy from "$lib/img/birdy.webp"
    import mater from "$lib/img/mater.webp"
    import flux from "$lib/img/flux.webp"
    import hammer from "$lib/img/hammer.webp"
</script>


<div id="top-container">
    <Header />
    <Navbar id="nav"/>
</div>

<div id="main">
    <div class="text">Tatom Team</div>
    <div class="text small">Administrators</div>
    <div class="img">
        <div class="textcontainer">
            <img src={hera} />
            <div class="text verysmall">Hera</div>
        </div>
        <div class="textcontainer">
            <img src={s4il} />
            <div class="text verysmall">S4IL</div>
        </div>
    </div>
    <br>
    <br>
    <div class="text">Blockcoin Team</div>
    <div class="text small">Administrators</div>
    <div class="img">
        <div class="textcontainer">
            <img src={hera} />
            <div class="text verysmall">Hera</div>
        </div>
        <div class="textcontainer">
            <img src={birdy} />
            <div class="text verysmall">BusyBird</div>
        </div>
        <div class="textcontainer">
            <img src={s4il} />
            <div class="text verysmall">S4IL</div>
        </div>
    </div>
    <div class="text small">Developers</div>
    <div class="img">
        <div class="textcontainer">
            <img src={mater} />
            <div class="text verysmall">Mater</div>
        </div>
        <div class="textcontainer">
            <img src={hammer} />
            <div class="text verysmall">Hammer</div>
        </div>
        <div class="textcontainer">
            <img src={flux} />
            <div class="text verysmall">Flux</div>
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
        width:80px;
        height: 80px;
    }
    
    .textcontainer {
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