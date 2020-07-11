<script>
    import Carousel from '@beyonk/svelte-carousel';
    import { ChevronLeftIcon, ChevronRightIcon } from 'svelte-feather-icons';
    import EventCard from './EventCard.svelte';

    export let data;
</script>

<style>
    .slide-content {
        margin-right: 20px;
    }
</style>

<Carousel perPage="2">
    {#each data as item, key}
        <div class="slide-content">
            <EventCard item={item}/>
        </div>
    {/each}
    <span class="control" slot="left-control">
        <ChevronLeftIcon />
    </span>
    <span class="control" slot="right-control">
        <ChevronRightIcon />
    </span>
</Carousel>