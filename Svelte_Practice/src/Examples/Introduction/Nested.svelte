<script>
    import Stylez from "./Styled.svelte"
</script>

<p>this is Stylez from ./styled.svelte: </p>
<Stylez/>

<p id="newstyle">This is the new style</p>

<style>
    #newstyle{
        font-size: 100px;
        color: orange;
        background-color: green;
    }
</style>