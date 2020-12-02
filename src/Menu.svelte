<script lang='ts'>
import MenuButton from "./MenuButton.svelte";
enum SelectedPage {
    NowPlaying,
    Search
}    

var selPage: SelectedPage = SelectedPage.NowPlaying;

function activePage(page: SelectedPage) : boolean {
    return false;
}

function activatePage(page: SelectedPage) : void {
    
}

</script>

<div>
    <MenuButton text="Now Playing" active={activePage(SelectedPage.NowPlaying)} on:click={activatePage()}/>
    <MenuButton text="Search" active={activePage(SelectedPage.Search)}/>

</div>

<style>
    div {
        margin: 0px;
        width: 160px;
        height: 100%;
        background-color: #e1e1e1;
        box-sizing: border-box;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
</style>