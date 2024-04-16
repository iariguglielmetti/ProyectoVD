<script>
    import * as d3 from "d3"
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
      personas = data
    })
  })
</script>


<main>
    <div class="header">
        <img src="/images/logo.png" width="150" alt="150" />
        <h2 class="headline" width=200px alt=200px>Hobbies</h2>
        <h3 class="subtitulo">Arte, Deporte, Educación y Entretenimiento </h3>
        <p class="bajada">Explorando los hobbies a través de datos</p>
    </div> 
</main>


<style>
  .header{
    text-align: center;
    
  }
  h2 {
    display: inline;
    font-family: IM FEEL English;
    font-size: 450%;
    position: relative;
    bottom: 75px;
  }
  h3{
    font-family: IM FEEL English;
    font-size: 140%;
    position: relative;
    bottom: 110px;
    left: 150px;
  }
  p{
    font-family: IM FEEL English;
    font-size: 115%;
    position: relative;
    bottom: 120px;
    left: 100px; 
  }
</style>