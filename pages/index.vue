<template>
  <!DOCTYPE html>
<html lang="es">
<head>
    <title>Formulario de Registro</title>

</head>
<body>

    <div class="form-container">
        <h2>Registro de Usuario</h2>
        <form action="procesar.php" method="POST">
            <!-- Nombre -->
            <label for="nombre">Nombre Completo:</label>
            <input type="text" id="nombre" name="nombre" required minlength="3">

            <!-- Correo -->
            <label for="email">Correo Electrónico:</label>
            <input type="email" id="email" name="email" required>

            <!-- Contraseña -->
            <label for="password">Contraseña:</label>
            <input type="password" id="password" name="password" required minlength="6">
            <!--pone puntos al escribir la contraseña-->
            
            <!-- Fecha de nacimiento -->
            <label for="fecha">Fecha de Nacimiento:</label>
            <input type="date" id="fecha" name="fecha" required>

            <!-- País -->
            <label for="pais">País:</label>
            <select id="pais" name="pais" required>
                <option value="">Selecciona tu país</option>
                <option value="mexico">México</option>
                <option value="españa">España</option>
                <option value="argentina">Argentina</option>
                <option value="colombia">Colombia</option>
                <option value="otros">Otros</option>
            </select>

            <!-- Género -->
            <label>Género:</label>
            <div class="radio-group">
                <input type="radio" id="hombre" name="genero" value="hombre" required>
                <label for="hombre">Hombre</label>

                <input type="radio" id="mujer" name="genero" value="mujer">
                <label for="mujer">Mujer</label>

                <input type="radio" id="otro" name="genero" value="otro">
                <label for="otro">Otro</label>
            </div>

            <!-- Intereses -->
            <label>Intereses:</label>
            <div class="checkbox-group">
                <input type="checkbox" id="deporte" name="intereses" value="deporte">
                <label for="deporte">Deporte</label>

                <input type="checkbox" id="musica" name="intereses" value="musica">
                <label for="musica">Música</label>

                <input type="checkbox" id="tecnologia" name="intereses" value="tecnologia">
                <label for="tecnologia">Tecnología</label>
                <!--el for es para que al hacer click en la etiqueta donde pone tecnologia, se vaya el foco al cuadro de texto-->
            </div>

            <!-- Comentarios -->
            <label for="comentarios">Comentarios:</label>
            <textarea id="comentarios" name="comentarios" rows="3"></textarea>

            <!-- Botón de enviar -->
            <button type="submit">Registrarse</button>
        </form>
    </div>

</body>
</html>
</template>
<style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .form-container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            width: 400px;
        }
        h2 {
            text-align: center;
        }
        label {
            font-weight: bold;
            display: block;
            margin: 10px 0 5px;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .radio-group, .checkbox-group {
            display: flex;
            gap: 10px;
        }
        button {
            width: 100%;
            padding: 10px;
            background: blue;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background: darkblue;
        }
    </style>
<!--PARA GRID-->
<!--<template>

  <!DOCTYPE html>
  <html lang="es">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Ejemplo con Grid</title>
  </head>
  <body>

      <h1 style="text-align: center;">Ejemplo con CSS Grid</h1>
      <div class="grid-container">
          <div class="item">Caja 1</div>
          <div class="item">Caja 2</div>
          <div class="item">Caja 3</div>
          <div class="grid-container2">
            <div class="item">Caja 4</div>
            <div class="item">Caja 5</div>
            <div class="item">Caja 6</div>
          </div>
          <div class="item">Caja 7</div>
      </div>

  </body>
  </html>

</template>
<style>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

.grid-container {
    display: grid;
    grid-template-rows: 100px auto 200px 200px;
    gap: 20px;
    padding: 20px;
}

.grid-container2 {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    padding: 10px;
}

.item {
    background-color: lightblue;
    padding: 20px;
    text-align: center;
    border-radius: 8px;
}

/* Para hacer el layout responsive */
@media (max-width: 768px) {
    .grid-container {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 480px) {
    .grid-container {
        grid-template-columns: 1fr;
    }
}
</style>-->

<!--PARA LO DEL HEADER, FOOTER Y TAL-->
<!-- src/App.vue
<template>
  <div id="app">
    Usamos los componentes Header, Card y Footer
    <Header />
    <Card title="Componente de Tarjeta 1" description="Este es el primer componente de tarjeta." />
    <Card title="Componente de Tarjeta 2" description="Este es el segundo componente de tarjeta." />
    <Footer />
  </div>
</template>

<script>
// Importamos los componentes
import Card from '/components/Card.vue';
import Footer from '/components/Footer.vue';
import Header from '/components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
    Card,
    Footer
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin: 20px;
}
</style>
 -->