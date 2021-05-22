# proyecto1
<html><head>
 <!--CDN version de desarrollo VUE.js, incluye advertencias de ayuda en la consola--> 
        <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script> 
        <!--CDN Boostrap CSS--> 
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous"> 
        <!--CDN de Awsome Fonts--> 
        <link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css" integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous"> 
    </head>
<body>
    <div id="app" class="container"> <!--id es un identificador unico de cada elemento HTML-->
          <h1 class="text-primary">Poke API</h1>
          <h2 class="text-danger">MARIANA GUADALUPE LOPEZ NATAREN</h2>
        <div class="row"> <!--sistema de Grid de Boostrap row-renglon-->
            <div class="col-md"> <!--sistema de Grid de Boostrap col=columna-->
                <ul>              <!--tamaños de columna sm, md,lg,xl-->
                    <li v-for="poke in pokes">
                      {{poke.name}} --
                     <btn class="btn btn-warning" v-bind:href="poke.url" v-on:click="pokesImg(poke.url)">{{poke.url}}</btn>
                        <br><br>
                    </li>
                </ul>
            </div> <!--cerramos div class="col-md"-->
            <div class="col-sm">
                Aqui vamos a poner la imagen del pokemon--&gt;
                <img width="50%" heigth="50%" v-bind:src="pokeImg.dream_world.front_default">
            </div> <!--cerramos div class="col-sm"-->
        </div> <!--cerramos div class="row"-->
    </div> <!--cerramos div class="container"-->
  <script src="vuepoke.js"></script>
</body></html>
