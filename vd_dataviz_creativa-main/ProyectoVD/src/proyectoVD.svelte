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

        <img src="/images/logo.png" width="150" alt="150" />
        <h1 class="headline" width=200px alt=200px>Hobbies</h1>
        <h2 class="subtitulo">Arte, Deporte, Educación y Entretenimiento </h2>
        <p id="bajada">Explorando los hobbies a través de datos</p>

    </div>

    <div class="categorias">
      
      <h2 class="categoriasSub">Categorias</h2>
      <img id="img-deporte" src="/images/deportes.png" width="100" alt="100"/>
      <img id="img-educacion" src="/images/educacion.png" width="100" alt="100"/>
      <img id="img-entretenimiento" src="/images/entretenimiento.png" width="100" alt="100"/>
      <img id="img-arte" src="/images/arte.png" width="100" alt="100"/>
      <p id="deportes">Deportes</p>
      <p id="educacion">Educación</p>
      <p id="entretenimiento">Entretenimiento</p>
      <p id="arte">Arte</p>

    </div>
<!--
    <div class="dificultad">

      <h2 class="dificultadSub">Dificultad</h2>
      <img src="/images/estrella1.png" width="100" alt="100"/>
      <img src="/images/estrella2.png" width="100" alt="100"/>
      <img src="/images/estrella3.png" width="100" alt="100"/>
      <p id="estrella1">Baja</p>
      <p id="estrella2">Media</p>
      <p id="estrella3">Alta</p>

    </div>

    <div class="utilidad">

      <h2 class="utilidadSub">Utilidad generada</h2>
      <img src="/images/bajaUtilidad.png" width="100" alt="100"/>
      <img src="/images/mediaUtilidad.png" width="100" alt="100"/>
      <img src="/images/altaUtilidad.png" width="100" alt="100"/>
      <p id="baja">Baja</p>
      <p id="media">Media</p>
      <p id="alta">Alta</p>
      
    </div>

    <div class="recursos">

      <h2 class="recursosSub">Recursos necesarios</h2>
      <img src="/images/deportesPocosRecursos.png" width="100" alt="100"/>
      <img src="/images/deportesAlgunosRecursos.png" width="100" alt="100"/>
      <img src="/images/deportesMuchosRecursos.png" width="100" alt="100"/>
      <img src="/images/educacionPocosRecursos.png" width="100" alt="100"/>
      <img src="/images/educacionAlgunosRecursos.png" width="100" alt="100"/>
      <img src="/images/educacionMuchosRecursos.png" width="100" alt="100"/>
      <img src="/images/entretenimientoPocosRecursos.png" width="100" alt="100"/>
      <img src="/images/entretenimientoAlgunosRecursos.png" width="100" alt="100"/>
      <img src="/images/entretenimientoMuchosRecursos.png" width="100" alt="100"/>
      <img src="/images/artePocosRecursos.png" width="100" alt="100"/>
      <img src="/images/arteAlgunosRecursos.png" width="100" alt="100"/>
      <img src="/images/arteMuchosRecursos.png" width="100" alt="100"/>
      <p id="pocos">Pocos</p>
      <p id="algunos">Algunos</p>
      <p id="muchos">Muchos</p>
  
    </div>

    <div class="antiguedad">

      <h2 class="antiguedadSub">Antiguedad, en años</h2>
      <img src="/images/vasoBajo.png" width="100" alt="100"/>
      <img src="/images/vasoMedio.png" width="100" alt="100"/>
      <img src="/images/vasoAlto.png" width="100" alt="100"/>
      <p id="0-6">Hasta 6 años</p>
      <p id="7-13">De 7 a 13 años</p>
      <p id="14-20">De 14 a 20 años</p>

    </div>

    <div class="frecuencia">

      <h2 class="frecuenciaSub">Frecuencia</h2>
      <img src="/images/frecuenciaBajaAmarilla.png" width="100" alt="100"/>
      <img src="/images/frecuenciaMediaAmarilla.png" width="100" alt="100"/>
      <img src="/images/frecuenciaAltaAmarilla.png" width="100" alt="100"/>
      <img src="/images/frecuenciaBajaGris.png" width="100" alt="100"/>
      <img src="/images/frecuenciaMediaGris.png" width="100" alt="100"/>
      <img src="/images/frecuenciaAltaGris.png" width="100" alt="100"/>
      <img src="/images/frecuenciaBajaAzul.png" width="100" alt="100"/>
      <img src="/images/frecuenciaMediaAzul.png" width="100" alt="100"/>
      <img src="/images/frecuenciaAltaAzul.png" width="100" alt="100"/>
      <p id="baja">Baja</p>
      <p id="media">Media</p>
      <p id="alta">Alta</p>

    </div>
 -->
</main>


<style>
  .header{
    text-align: center;
  }
  .header h1 {
    font-family: IM FEEL English;
    font-size: 450%;
    position: relative;
    bottom: 50px;
  }
  .header h2{
    font-family: IM FEEL English;
    position: relative;
    bottom: 100px;
  }
  .header p{
    font-family: IM FEEL English;
    font-size: 115%;
    position: relative;
    bottom: 110px;
  }

  .categorias{
    display: inline-block;
  }
  .categorias h2{
    font-family: 'Times New Roman';
    font-size: 30px;
 }
 .categorias img{
   position: relative;
 }
 #img-educacion{
  left: 2%;
 }
 #img-entretenimiento{
  left: 7%;
 }
 #img-arte{
  left: 12%;
 }
 .categorias p{
    display: inline;
    font-size: 20px;
    font-family: 'Times New Roman';
    position: relative;
    top: 30px;
  }
  #deportes{
    right: 52%;  
  }
  #educacion{
    right: 48%;  
  }
  #entretenimiento{
    right:46%;
  }
  #arte{
    right: 38%;  
  }

  /*.dificultad{
    display: inline-block;
  }
  .dificultad h2{font-family: josefin slab;
    font-size: 30px;}
  .dificultad p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    top: 20px;
    right: 300px;
  }
  .estrella1{}
  .estrella2{}
  .estrella3{}

  .utilidad{
    display: inline-block;
  }
  .utilidad h2{}
  .utilidad p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    top: 20px;
    right: 300px;
  }
  .utiliadad p #baja{}
  .utiliadad p #media{}
  .utiliadad p #alta{}

  .recursos{
    display: inline-block;
  }
  .recursos h2{}
  .recursos p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    top: 20px;
    right: 300px;
  }
  .pocos{}
  .algunos{}
  .muchos{}

  .antiguedad{
    display: inline-block;
  }
  .antiguedad h2{}
  .antiguedad p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    top: 20px;
    right: 300px;
  }
  .0-6{}
  .7-13{}
  .14-20{}

  .frecuencia{
    display: inline-block;
  }
  .frecuencia h2{}
  .frecuencia p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    top: 20px;
    right: 300px;
  }
  .frecuencia p #baja{}
  .frecuencia p #media{}
  .frecuencia p #alta{}*/


</style>
 <!-- no se si las clase pueden tener solamente numeros en el nombre / TAMBIEN DE 1 A 6 AÑOS-->