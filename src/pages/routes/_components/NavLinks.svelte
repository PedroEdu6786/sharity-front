<script>
    // your script goes here
</script>

<style>

    .sh-header {
        display: flex;
        justify-content: space-between;
    }

    .sh-logo {
        display: flex;
        align-items: center;
        text-decoration: none;
    }

    .logo {
        height: 1.2em;
    }

    .sh-name {
        margin-left: .2em;
        font-size: 18px;
        color: black;
        font-family: 'Righteous', cursive;
    }

    .sh-nav-container {
        display: flex;
    }

    .sh-nav-container {
        list-style: none;
    }

    .txt-container {
        display: flex;
    }

    .item {
        margin-left: 1.5em;
        font-family: 'Righteous', cursive;
    }

</style>

<header class="sh-header">
    <div class="left-nav">
        <a href="." class="sh-logo">
            <img src="../logo.svg" alt="sh-icon" class="logo">
            <div class="sh-name">Sharity</div>
        </a>
        <div class="search-bar">
            <div class="txt-container">
                <i class="fas fa-search"></i>
                <div class="search-txt">Search events</div>
            </div>
        </div>
    </div>

    <nav class="sh-nav">
        <ul class="sh-nav-container">
            <li class="item"><a href=".">Dashboard</a></li>
            <li class="item"><a href=".">Create event</a></li>
            <li class="item"><a href=".">Sign in</a></li>
        </ul>
    </nav>
</header>