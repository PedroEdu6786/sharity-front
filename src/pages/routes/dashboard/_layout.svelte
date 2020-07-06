<script>
    import EventCarousel from './components/EventCarousel.svelte';
</script>

<style>
    /* your styles go here */
    .sh-content {
        margin: 0 auto;
        font-family: 'Righteous', cursive;
    }

    .events-container {
        margin-bottom: 5em;
    }

    .sh-events {
        margin-bottom: 1.5em;
    }

</style>

<div class="sh-content">
    <!-- Coming events -->
    <section class="events-container">
        <div class="sh-events">
            <h1>Up Coming Events</h1>
        </div>
        <EventCarousel />
    </section>

    <!-- New Events -->
    <section class="events-container">
        <div class="sh-events">
            <h1>New Events</h1>
        </div>
        <EventCarousel />
    </section>

    <!-- More Events -->
    <section class="events-container">
        <div class="sh-events">
            <h1>More Events</h1>
        </div>
        <EventCarousel />
    </section>

</div>
<slot>
</slot>