<script>
    import NavLinks from './_components/NavLinks.svelte'
</script>

<style>
    .sh-container {
        margin: 0 auto;
        padding: 20px 5%;
        max-width: 1400px;
    }
</style>

<div class="sh-container">
    <NavLinks />
    <slot>
    </slot>
</div>
