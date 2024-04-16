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
    
      /* Actualizamos dominio con la data de edad */
      /*let minMaxEdad = d3.extent(data, d => d.edad)
      grosor = grosor.domain(minMaxEdad)

      /* Actualizamos dominio y rango con la data de altura */
      /*let minMaxAltura = d3.extent(data, d => d.altura
      radioAltura = radioAltura.domain(minMaxAltura).range([25, 50])*/
   
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

    <div class="introduction">
      <p>Acá nose si tengo que poner algo escrito para explicar masomenos el tema pero bueno nada.</p>

    </div>

    <div class="Proyecto">
        <div class="logos_de_los_hobbies">
          <img src="/images/repr_categorias.png" width="700" alt="150"/>
        </div>

    </div>
</main>


<style>
  .header{
    text-align: center;
  }
  h2 {
    font-family: IM FEEL English;
    font-size: 450%;
    position: relative;
    bottom: 75px;
  }
  h3{
    font-family: IM FEEL English;
    font-size: 140%;
    position: relative;
    bottom: 135px;
  }
  p{
    font-family: IM FEEL English;
    font-size: 115%;
    position: relative;
    bottom: 150px;
  }
  .introduction{
    text-align: center;
  }
  .Proyecto{
    text-align: center;
  }
  .logos_de_los_hobbies{
    margin-top: -100px;
  }

/*iara no te enojes, solo puse la imagen para ver como iba a quedar obviamente vamos a hacer una a una y bien*/

</style>
