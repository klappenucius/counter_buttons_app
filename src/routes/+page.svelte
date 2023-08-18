<script lang="ts">
    let n: number;
    n = 0;
</script>

<style>
    * {
        margin: auto;
        max-width: 1150px;
        font-family:Verdana, Geneva, Tahoma, sans-serif;
    }

    .container_row {
        display: flex;
        flex-direction: row;
    }

    .container_column {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    h1 {
        text-align: center;
        width: 20%;
        margin: 5% 40% 2% 40%;
    }

    #wrapper {
        width: 20%;
        margin: 2% 40%;
    }

    button {
        width: 40%;
        padding: 5% 5%;
        margin: 5%;
        border-radius: 15px;
        color: white;
        font-size: 32px;
        text-align: center;
    }

    #plus_button {
        background-color: #2071AC;
        border: solid 2px #115280;
    }

    #minus_button {
        background-color: #00A884;
        border: solid 2px #017a60;
    }
</style>

<div class="container_column">
    <h1>{n}</h1>
<div id="wrapper" class="container_row">
<button on:click={(e) => {n += 1}} id="plus_button" >+</button>

<button on:click={(e) => {n -= 1}} id="minus_button">-</button>
</div>
</div>
