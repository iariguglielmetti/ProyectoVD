<script>
  
    import * as d3 from "d3"
    import {onMount} from "svelte"
    
    //import 
    let nombre = []

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
    })
  })
</script>



<main>
    <div class="header">

      <img src="/images/logo.svg" width="160" alt=""/>
    </div>
  <div class= "headersito">
        <h1 class="headline">Hobbies</h1>
        <h2 class="subtitulo">Arte, Deporte, Educación y Entretenimiento </h2>
        <p id="bajada">Explorando los hobbies a través de datos</p>
  </div>


</main>


<style>
  .header{
    text-align: center;
  }
  .headersito{
    text-align: center;
  }
  .headersito h1 {
    font-family: "krona One";
    font-size: 450%;
    position: relative;
    bottom: 50px;

    background: linear-gradient(to right, #FE004C, #27AAF4);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    display: inline-block;
  }
  .headersito h2{
    font-family: "kameron", serif;
    position: relative;
    bottom: 90px;
  }
  .headersito p{
    font-family: "kameron", serif;
    font-size: 115%;
    position: relative;
    bottom: 105px;
  }
</style>
