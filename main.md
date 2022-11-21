---
theme : "White"
transition: "slide"
highlightTheme: "monokai"
slideNumber: true
title: "Title"
enableChalkboard: false
enableMenu: True
enableTitleFooter: true


---

<style type="text/css">
    /* 1. Style header/footer <div> so they are positioned as desired. */
    #header-left1 {
        position: absolute;
        top: 3.3%;
        left: 1%;
        color: gray;
        font-size: 0.4em;
    }
    #header-left2 {
        position: absolute;
        top: 5.3%;
        left: 1%;
        color: gray;
        font-size: 0.4em;
    }
    #header-right {
        position: absolute;
        top: 1.7%;
        right: 1%;
    }
    #footer-left {
        position: absolute;
        bottom: 3%;
        left: 7.5%;
        color: gray;
        font-size: 0.4em;
    }
</style>

<!-- 2. Create hidden header/footer <div> -->
<div id="hidden" style="display:none;">
    <div id="header">
        <div id="header-left1"> upper left header 1 </div>
        <div id="header-left2"> upper left header 2 </div>
        <div id="header-right"><img class="fragment" src="logo.png" width="75" height="75"> </div>
        <div id="footer-left"> lower left footer </div>
    </div>
</div>

<script src="https://code.jquery.com/jquery-2.2.4.min.js"></script>
<script type="text/javascript">
    // 3. On Reveal.js ready event, copy header/footer <div> into each `.slide-background` <div>
    var header = $('#header').html();
    if ( window.location.search.match( /print-pdf/gi ) ) {
        Reveal.addEventListener( 'ready', function( event ) {
            $('.slide-background').append(header);
        });
    }
    else {
        $('div.reveal').append(header);
   }
</script>

------
#### <span style="color:#3070b3"> Title </span>
------


---

<span style="color:#3070b3"> Page Title </span>

<img class="r-stretch" src="noise.png">
