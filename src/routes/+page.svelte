<script>
    import Header from "$lib/elements/header.svelte"
    import Navbar from "$lib/elements/navbar.svelte"
</script>



<Header />
<div class="text">We build things <span>today</span><br> For a better web <span>tomorrow</span></div>
<Navbar />

<style>
    .text {
        font-family: "Montserrat", sans-serif;
        color:white;
        font-size: 50px;
        margin-left: 10px;
        margin-top: 100px;
    }

    .text span {
        color:#00E8FF
    }
</style>