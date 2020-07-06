<script>
    import NavLinks from './_components/NavLinks.svelte'
</script>

<style>
    .sh-container .sh-nav{
        margin: 0 auto;
        padding: 20px 5%;
    }
    .sh-container .sh-content{
        margin: 0 auto;
        padding: 20px 5%;
        max-width: 1300px;
    }
    
    .sh-content {
        margin-top: 2.5em;
    }
</style>

<div class="sh-container">
    <div class="sh-nav">
        <NavLinks />
    </div>
    <div class="sh-content">
        <slot>
        </slot>
    </div>
</div>
