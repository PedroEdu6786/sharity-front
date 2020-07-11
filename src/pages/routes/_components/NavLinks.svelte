<script>
    import { url } from '@sveltech/routify';
    import { SearchIcon } from 'svelte-feather-icons';
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

    .item {
        margin-left: 1.5em;
        font-family: 'Righteous', cursive;
    }

    .search-bar {
        line-height: 14px;
        margin-top: .5em;
        position: relative;
    }

    label { 
        position: absolute;
        left: 20px;
        top: 14px;
        padding: 0 2px;
        pointer-events: none;
        background: #fff;
        font-family: 'Righteous', cursive;
        -webkit-transition: -webkit-transform 100ms ease;
        -moz-transition: -moz-transform 100ms ease;
        -o-transition: -o-transform 100ms ease;
        -ms-transition: -ms-transform 100ms ease;
        transition: transform 200ms ease;
    }

    input {
        height: 30px;
        width: 220px;
        border-radius: 8px;
        outline: none;
        position: relative;
        font-family: 'Righteous', cursive;
    }

    input:invalid + label {
        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -o-transform: translateY(0);
        -ms-transform: translateY(0);
        transform: translateY(0);
    }
    input:focus {
        border-color: #2b96f1;
    }
    input:focus + label {
        color: #2b96f1;
        -webkit-transform: translateY(-20px);
        -moz-transform: translateY(-20px);
        -o-transform: translateY(-20px);
        -ms-transform: translateY(-20px);
        transform: translateY(-20px);
    }


</style>

<header class="sh-header">
    <div class="left-nav">
        <a href={$url('dashboard')} class="sh-logo">
            <img src="../logo.svg" alt="sh-icon" class="logo">
            <div class="sh-name">Sharity</div>
        </a>
        <div class="search-bar">
            <input type="text" required>
            <label for="event">Search Events</label>
        </div>
    </div>

    <nav class="sh-nav">
        <ul class="sh-nav-container">
            <li class="item"><a href={$url('dashboard')}>Dashboard</a></li>
            <li class="item"><a href={$url('create-event')}>Create event</a></li>
            <li class="item"><a href=".">Sign in</a></li>
        </ul>
    </nav>
</header>