<script>
    let estudiantes = $state([
        {nombre: "Juan", edad: 16},
        {nombre: "Pedro", edad: 17},
        {nombre: "María", edad: 16},
        {nombre: "José", edad: 17},
        {nombre: "Luis", edad: 16},
        {nombre: "Ana", edad: 17},
        {nombre: "Sofía", edad: 16},
        {nombre: "Carlos", edad: 17},
        {nombre: "Andrés", edad: 16},
        {nombre: "Mónica", edad: 17},
        {nombre: "Julián", edad: 16},
        {nombre: "Laura", edad: 17},
        {nombre: "Camilo", edad: 16},
        {nombre: "Marcela", edad: 17},
        {nombre: "Santiago", edad: 16},
        {nombre: "Valentina", edad: 17},
        {nombre: "Mauricio", edad: 16},
        {nombre: "Catalina", edad: 17},
        {nombre: "Esteban", edad: 16},
        {nombre: "Daniela", edad: 17},
        {nombre: "Felipe", edad: 16},
        {nombre: "Isabela", edad: 17},
        {nombre: "David", edad: 16},
        {nombre: "Lina", edad: 17},
        {nombre: "Jorge", edad: 16},
        {nombre: "Patricia", edad: 17},
        {nombre: "Germán", edad: 16},
        {nombre: "Lorena", edad: 17},
        {nombre: "Hernán", edad: 16},
        {nombre: "Sara", edad: 17},
        {nombre: "Fernando", edad: 16},
        {nombre: "Carolina", edad: 17},
        {nombre: "Ricardo", edad: 16},
        {nombre: "Diana", edad: 17},
        {nombre: "Alberto", edad: 16},
        {nombre: "Natalia", edad: 17},
        {nombre: "Miguel", edad: 16},
        {nombre: "Gabriela", edad: 17},])
</script>

{#each estudiantes as estudiante}
    <div>
        <h2>{estudiante.nombre}</h2>
        <p>Edad: {estudiante.edad}</p>
    </div>
{/each}

<style>
   div {
       border: 1px solid black;
       margin: 10px 20px;
       padding: 10px;
       max-width: 50vh;
       margin: 20px auto;
   }
</style>