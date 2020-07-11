<script>
    import EventCarousel from './components/EventCarousel.svelte';

    let promise = getEvents();
    let data = [];

    async function getEvents() {
        const res = await fetch("http://localhost:3000/event/all");
        const json = await res.json();
        data = json;
        if(res.ok) {
            return json;
        } else {
            throw new Error(json);
        }
    }
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
        {#await promise}
            <h1>wait</h1>
        {:then data}
            <EventCarousel data={data}/>
        {:catch error}
            <h1>Not Found</h1>>
        {/await}
    </section>

    <!-- New Events -->
    <!-- <section class="events-container">
        <div class="sh-events">
            <h1>New Events</h1>
        </div>
        <EventCarousel />
    </section> -->

    <!-- More Events -->
    <!-- <section class="events-container">
        <div class="sh-events">
            <h1>More Events</h1>
        </div>
        <EventCarousel />
    </section> -->

</div>
<slot>
</slot>