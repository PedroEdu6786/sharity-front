<script>
    // your script goes here
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Righteous&display=swap');


    * {
        margin: 0;
    }

    .sh-header {
        box-sizing: border-box;
        display: flex;
        font-family: 'Righteous', cursive;
        margin: 0 auto;
        padding: .5em 1em;
        max-width: 1300px;
        justify-content: space-between;
    }

    .left-nav {
        margin: 0;
        padding: 0;
    }

    .sh-logo {
        display: flex;
    }

    .sh-nav-container {
        list-style: none;
        display: flex;
    }

    .search-bar {
        display: flex;
        position: absolute;
        width: 350px;
        height: 2.5em;
        background: #EDEDED;
        border-radius: 10px;
    }

    .sh-header .sh-nav .sh-nav-container a{
        padding: 0 .6em;
    }

    .search-bar {
        margin: 1em 0;
    }

    a { 
        text-decoration: none;
    }
</style>

<header class="sh-header">
    <div class="left-nav">
        <a href="." class="sh-logo">
            <img src="../logo.svg" alt="sh-icon" class="logo">
            <div class="sh-name">Sharity</div>
        </a>
        <div class="search-bar">
            <img src="" alt="search" class="search-icon">
            <div class="search-txt">Search events</div>
        </div>
    </div>

    <nav class="sh-nav">
        <ul class="sh-nav-container">
            <li class="item"><a href=".">Create event</a></li>
            <li class="item"><a href=".">Sign in</a></li>
        </ul>
    </nav>
</header>