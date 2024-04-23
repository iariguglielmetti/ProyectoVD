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

        <img src="/images/logo.png" width="180" alt="180" />
        <h1 class="headline">Hobbies</h1>
        <h2 class="subtitulo">Arte, Deporte, Educación y Entretenimiento </h2>
        <p id="bajada">Explorando los hobbies a través de datos</p>

    </div>

    <div class="categorias">
      
      <h2 class="categoriasSub">Categorias</h2>
      <img id="img-arte" src="/images/arte.png" width="100" alt="100"/>
      <img id="img-educacion" src="/images/educacion.png" width="100" alt="100"/>
      <img id="img-entretenimiento" src="/images/entretenimiento.png" width="100" alt="100"/>
      <img id="img-deporte" src="/images/deportes.png" width="100" alt="100"/>
      <p id="arte">Arte</p>
      <p id="educacion">Educación</p>
      <p id="entretenimiento">Entretenimiento</p>
      <p id="deportes">Deportes</p>

    </div>

    <div class="dificultad">

      <h2 class="dificultadSub">Dificultad</h2>
      <img id="img-estrella1" src="/images/estrella1.png" width="75" alt="0"/>
      <img id="img-estrella2" src="/images/estrella2.png" width="175" alt="0"/>
      <img id="img-estrella3" src="/images/estrella3.png" width="280" alt="0"/>
      <p id="estrella1">Baja</p>
      <p id="estrella2">Media</p>
      <p id="estrella3">Alta</p>

    </div>

    <div class="utilidad">

      <h2 class="utilidadSub">Utilidad generada</h2>
      <img id="bajaUtilidad" src="/images/bajaUtilidad.png" width="100" alt="100"/>
      <img id="mediaUtilidad" src="/images/mediaUtilidad.png" width="100" alt="100"/>
      <img id="altaUtilidad" src="/images/altaUtilidad.png" width="100" alt="100"/>
      <p id="baja">Baja</p>
      <p id="media">Media</p>
      <p id="alta">Alta</p>
      
    </div>

    <div class="recursos">

      <h2 class="recursosSub">Recursos necesarios</h2>
      <p id="pocosRecursos">Pocos</p>
      <p id="algunosRecursos">Algunos</p>
      <p id="muchosRecursos">Muchos</p>
      <img id="imgArtePocos" src="/images/artePocosRecursos.png" width="100" alt="100"/>
      <img id="imgArteAlgunos" src="/images/arteAlgunosRecursos.png" width="100" alt="100"/>
      <img id="imgArteMuchos" src="/images/arteMuchosRecursos.png" width="100" alt="100"/>
      <img id="imgEduPocos" src="/images/educacionPocosRecursos.png" width="100" alt="100"/>
      <img id="imgEduAlgunos" src="/images/educacionAlgunosRecursos.png" width="100" alt="100"/>
      <img id="imgEduMuchos" src="/images/educacionMuchosRecursos.png" width="100" alt="100"/>
      <img id="imgEntrePocos" src="/images/entretenimientoPocosRecursos.png" width="100" alt="100"/>
      <img id="imgEntreAlgunos" src="/images/entretenimientoAlgunosRecursos.png" width="100" alt="100"/>
      <img id="imgEntreMuchos" src="/images/entretenimientoMuchosRecursos.png" width="100" alt="100"/>
      <img id="imgDepPocos" src="/images/deportesPocosRecursos.png" width="100" alt="100"/>
      <img id="imgDepAlgunos" src="/images/deportesAlgunosRecursos.png" width="100" alt="100"/>
      <img id="imgDepMuchos" src="/images/deportesMuchosRecursos.png" width="100" alt="100"/>
    </div>
    
    <div class="antiguedad">

      <h2 class="antiguedadSub">Antiguedad</h2>
      <img src="/images/vasoBajo.png" width="200" alt="100"/>
      <img src="/images/vasoMedio.png" width="211" alt="100"/>
      <img src="/images/vasoAlto.png" width="200" alt="100"/>
      <p id="hasta6años">Hasta 6 años</p>
      <p id="de7a13años">De 7 a 13 años</p>
      <p id="de14a20años">De 14 a 20 años</p>

    </div>

    <div class="frecuencia">

      <h2 class="frecuenciaSub">Frecuencia</h2>
      <p id="frecuenciaBaja">Baja</p>
      <p id="frecuenciaMedia">Media</p>
      <p id="frecuenciaAlta">Alta</p>
      <img id="frecuenciaBajaAma" src="/images/frecuenciaBajaAmarilla.png" width="60" alt="100"/>
      <img id="frecuenciaMediaAma" src="/images/frecuenciaMediaAmarilla.png" width="100" alt="100"/>
      <img id="frecuenciaAltaAma" src="/images/frecuenciaAltaAmarilla.png" width="150" alt="100"/>
      <img id="frecuenciaBajaG" src="/images/frecuenciaBajaGris.png" width="60" alt="100"/>
      <img id="frecuenciaMediaG" src="/images/frecuenciaMediaGris.png" width="100" alt="100"/>
      <img id="frecuenciaAltaG" src="/images/frecuenciaAltaGris.png" width="150" alt="100"/>
      <img id="frecuenciaBajaAz" src="/images/frecuenciaBajaAzul.png" width="60" alt="100"/>
      <img id="frecuenciaMediaAz" src="/images/frecuenciaMediaAzul.png" width="100" alt="100"/>
      <img id="frecuenciaAltaAz" src="/images/frecuenciaAltaAzul.png" width="150" alt="100"/>
      <a id="textoVacio">textoVacio</a>

    </div>
<!-- -->
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
    bottom: 90px;
  }
  .header p{
    font-family: IM FEEL English;
    font-size: 115%;
    position: relative;
    bottom: 105px;
  }
  
  .categorias{
    display: inline-block;
    position: relative;
    left: 25px;
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
 #img-deporte{
  left: 12%;
 }
 .categorias p{
    display: inline;
    font-size: 20px;
    font-family: 'Times New Roman';
    position: relative;
    top: 30px;
  }
  #arte{
    right: 52%;  
  }
  #educacion{
    right: 45%;  
  }
  #entretenimiento{
    right:40%;
  }
  #deportes{
    right: 34%;  
  }
  
  .dificultad{
    display: inline-block;
    position: relative;
    top: 25px;
    left: 25px;
  }
  .dificultad h2{
    font-family: 'Times New Roman';
    font-size: 30px;
  }
  .dificultad p{
    display: inline;
    font-family: 'Times New Roman';
    font-size: 20px;
  }
  .dificultad img{
   position: relative;
 }
  #img-estrella1{
    bottom: 6px;
  }
  #img-estrella2{
    left: 8%;
  }
  #img-estrella3{
    left:15%
  }
  
  .dificultad p{
    position: relative;
    top:20px;
  }
  #estrella1{
    right: 520px;
  }
  #estrella2{
    right: 390px;
  }
  #estrella3{
    right: 157px;
  }

  .utilidad{
    display: inline-block;
    position: relative;
    bottom: 200px;
    left: 50px;
  }
  .utilidad h2{
    font-family: 'Times New Roman';
    font-size: 30px;
  }
  .utilidad img{
    display: inline-block;
    position: relative;
    
  }
  #bajaUtilidad{
    left: 75px;
  }
  #mediaUtilidad{
    left: 125px;
  }
  #altaUtilidad{
    left: 175px;
  }
  .utilidad p{
    display: inline;
    font-family: 'Times New Roman';
    font-size: 20px;
    position: relative;
  }
  #baja{
    top: 30px;
    right: 203px;
  }
  #media{
    top: 30px;
    right: 100px;
  }
  #alta{
    top: 30px;
    left: 10px;
  }

  .recursos{
    display: inline-block;
    position: relative;
    left: 700px;
    bottom: 160px;
  }
  .recursos h2{
    font-family: 'Times New Roman';
    font-size: 30px;
    position: relative;
    left: 30px;
  }
  .recursos p{
    display: inline;
    font-family: 'Times New Roman';
    font-size: 20px;
    position: relative;
    bottom: 80px;
    left: 100px;
  }
  #algunosRecursos{
    left: 225px;
  }
  #muchosRecursos{
    left: 350px;
  }
  
  .recursos img{
    position: relative;
    top: 50px;
  }
  #imgArtePocos {
    right: 120px;
  }
  #imgArteAlgunos{
    right: 40px;
  }
  #imgArteMuchos{
    left: 45px;
  }
  #imgEduPocos {
    top: 170px;
    right: 430px;
  }
  #imgEduAlgunos{
    top: 170px;
    right: 350px;
  }
  #imgEduMuchos{
    top: 170px;
    right: 260px;
  }
  #imgEntrePocos {
    top: 270px;
    right: 740px;
  }
  #imgEntreAlgunos{
    top: 270px;
    right: 660px;
  }
  #imgEntreMuchos{
    top: 270px;
    right: 572px;
  }
  #imgDepPocos {
    top: 380px;
    right: 1050px;
  }
  #imgDepAlgunos{
    top: 272px;
    left: 260px;
  }
  #imgDepMuchos{
    top: 272px;
    left: 350px;
  }
  
  .antiguedad{
    display: inline;
    font-size: 20px;
    font-family: 'Times New Roman';
    position: relative;
    bottom: 250px;
    left: 25px;
  }
  .antiguedad p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    top: 50px;
  }
  #hasta6años{
    right: 565px;
  }
  #de7a13años{
    right: 480px;
  }
  #de14a20años{
    right: 405px;
  }
  
  .frecuencia{
    display: inline;
    font-size: 20px;
    font-family: 'Times New Roman';
    position: relative;
    bottom: 180px;
    left: 25px;
  }
  .frecuencia p{
    display: inline;
    font-family: 'Times New Roman';
    position: relative;
    bottom: 130px;
  }
  
  #frecuenciaBaja{
    left: 90px;
  }
  #frecuenciaMedia{
    left: 250px;
  }
  #frecuenciaAlta{
    left: 420px;
  }
  .frecuencia img{
    position: relative;
  }
  #frecuenciaBajaAma{
    top: 15px;
    right: 57px;
  }
  #frecuenciaMediaAma{
    top: 30px;
    left: 68px;
  }
  #frecuenciaAltaAma{
    top: 50px;
    left: 155px;
  }
  #frecuenciaBajaG{
    top: 180px;
    right: 382px;
  }
  #frecuenciaMediaG{
    top: 198px;
    right: 255px;
  }
  #frecuenciaAltaG{
    top: 220px;
    right: 170px;
  }
  #frecuenciaBajaAz{
    top: 350px;
    right: 705px;
  }
  #frecuenciaMediaAz{
    top: 363px;
    right: 582px;
  }
  #frecuenciaAltaAz{
    top: 390px;
    right: 495px;
  }
  #textoVacio{
    position: relative;
    top: 400px;
    color: black;
  }
  
</style>
