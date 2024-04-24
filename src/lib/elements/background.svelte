<script>
    import corner1 from "$lib/img/corner1.svg"
    import corner2 from "$lib/img/corner2.svg"
</script>

<div id="bg" />
<img id="corner-1" src={corner1}/> 
<img id="corner-2" src={corner2}/> 

<style>

 #bg {
    top:0;
    left:0;
    height: 100%;
    width: 100%;
    position: fixed;
    background-color: #001220;
    z-index: -10;
 }

 #corner-1 {
    top:0;
    right: 0;
    position: fixed;
 }

 #corner-2 {
    bottom:0;
    left: 0;
    position: fixed;
 }

</style>
