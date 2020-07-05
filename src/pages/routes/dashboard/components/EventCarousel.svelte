<script>
    import Carousel from '@beyonk/svelte-carousel';
    import { ChevronLeftIcon, ChevronRightIcon } from 'svelte-feather-icons';
    import EventCard from './EventCard.svelte';
</script>

<style>
    .slide-content {
        margin-right: 20px;
    }
</style>

<Carousel>
    <span class="control" slot="left-control">
        <ChevronLeftIcon />
    </span>
    {#each Array(10) as item, key}
        <div class="slide-content">
            <EventCard/>
        </div>
    {/each}
    <span class="control" slot="right-control">
        <ChevronRightIcon />
    </span>
</Carousel>