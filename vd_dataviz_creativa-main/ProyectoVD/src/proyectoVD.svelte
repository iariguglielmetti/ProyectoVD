<script>
    /*import * as d3 from "d3"
    import {onMount} from "svelte"

    let personas = []

    let colorUtilidad = d3
        .scaleOrdinal()
        .domain([])
        .range([])

    let cantidadEstrellas = d3
    onMount(() => {
    d3.csv("./data/personas.csv", d3.autoType).then(data => {
      console.log(data)
    
      /* Actualizamos dominio con la data de edad */
      /*let minMaxEdad = d3.extent(data, d => d.edad)
      grosor = grosor.domain(minMaxEdad)

      /* Actualizamos dominio y rango con la data de altura */
      /*let minMaxAltura = d3.extent(data, d => d.altura
      radioAltura = radioAltura.domain(minMaxAltura).range([25, 50])*/
   
      //personas = data
    //})
 // })
</script>


<main>
    <div class="header">

        <img src="/images/logo.svg" width="150" alt="150" />
        <h1 class="headline">Hobbies</h1>
        <h2 class="subtitulo">Arte, Deporte, Educación y Entretenimiento </h2>
        <p id="bajada">Explorando los hobbies a través de datos</p>

    </div>

</main>


<style>
/* HEADER */
  .header{
    text-align: center;
    font-family: "krona one";
  }
  /*.header h1{}*/
  .header h2{
    font-size: 20px;
  }
  
</style>
