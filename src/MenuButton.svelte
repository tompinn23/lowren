<script lang='ts'>
    export let text: string;
    export let active: boolean;
</script>

<button class='{active ? "active": "inactive"}'>
{text}
</button>

<style>

    button {
        font-size: small;
        margin: 10px;
        width: 90%;
        font-weight: bold;
        padding-left: 10px;
        padding-right: 10px;
        border-radius: 10px;
        background-color: #e1e1e1;
        border-color: #e1e1e1;
    }
    button:hover {
        border-color: #c2c2c2;
        background-color: #c2c2c2;
    }

    .active {
        border-color: #1ED760;
        background-color: #1ED760;
    }
</style>
