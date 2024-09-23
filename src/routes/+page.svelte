<script lang="ts">
    import Texto from "./Texto.svelte";
    let nombre = $state("Futuros profesionales de Colombia")
    let mostrarTexto = $state(false);
    let miH2: HTMLHeadingElement | null;
</script>

<h1>
    Alumnos de 11
</h1>

<p>
    Aquí se mostrarán los alumnos de 11.
    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Deserunt adipisci natus delectus minus in, nemo rerum exercitationem facilis magni esse tempore explicabo. Nostrum, consectetur reiciendis! Deleniti minus facere voluptatem laboriosam.
</p>

<h2 bind:this={miH2}>Atentamente: {nombre}</h2>

<button onclick={()=>mostrarTexto = !mostrarTexto}>Mostrar componente texto</button>

{#if mostrarTexto}
    <Texto />
{/if}

<form style="margin: 20px auto">
    <label for="nombre">Nombre de usuario:</label>
    <input type="text" id="nombre" bind:value={nombre} />
</form>

<style>
    h1 {
        color: blue;
        text-align: center;
    }
    p {
        color: red;
        margin: 10px 20px;
    }
</style>