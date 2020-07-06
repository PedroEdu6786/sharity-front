<script>
    // your script goes here
</script>

<style>

    .ev-container {
        justify-content: space-between;
        display: flex;
    }

    .event-left {
        width:60%;
    }

    .event-right {
        width:40%;
        padding-left: 4em;
    }

    .sh-hero-container {
        background-image: url("https://via.placeholder.com/468x60?text=Visit+Blogging.com+Now");
        border-radius: 20px;
        height: 200px;
    }

    .ev-container {
        margin-top: 3em;
    }

    .sh-left-container {
        margin-bottom: 3em;
    }

    .sh-font {
        font-family: 'Righteous', cursive;
    }

    .sh-subfont  {
        font-family: 'Varela', sans-serif;
    }

    .sh-donations {
        list-style: none;
    }

    .goal-bar {
        width: 50%;
        height: 20px;
        background-color: darkgrey;
        border-radius: 5px;
        justify-content: flex-end;
    }

    .hero-content {
        padding: 1.5em 2em;
    }
    
</style>

<div class="sh-hero-container">
    <div class="hero-content sh-font">
        <h1>Event Name</h1>
        <h3>Event Host</h3>
        <h3>01-10-2020</h3>
    </div>
</div>
<div class="ev-container">
    <section class="split event-left sh-font">
        <div class="sh-left-container">
            <h2>About the event</h2>
            <p class="sh-subfont">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores beatae consequatur fuga aperiam facere, autem quia dolor ea eveniet corporis velit culpa reiciendis ut harum ullam asperiores veritatis quidem incidunt.
            </p>
        </div>

        <div class="sh-left-container">
            <h2>Donation Goals</h2>
            <ul class="sh-donations">
                <li>
                    <span>Donation Item</span>
                    <div class="goal-reach">
                        <div class="goal-bar"><span>10</span></div>
                    </div>
                </li>
            </ul>
        </div>

    <button type="button" class="btn btn-primary btn-lg">Im Going</button>
        
    </section>

    <section class="split event-right sh-font">
        <div class="sh-left-container">
            <div class="ev-host-info">
                <h2>Location</h2>
                <p class="sh-subfont">Lorem ipsum, dolor sit amet consectetur adipisicing elit</p>
            </div>
        </div>
    </section>
</div>

<slot></slot>