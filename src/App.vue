<template>
  <div id="app">
    <div class="calculadora">
      <div class="contenedor">
        <div class="display">
          <div id="texto">1233985493859</div>
        </div>
        <div class="botoneras">
          <div class="botonera-izq">
            <button>1</button>
            <button>2</button>
            <button>3</button>
            <button>4</button>
            <button>5</button>
            <button>6</button>
            <button>7</button>
            <button>8</button>
            <button>9</button>
            <button>0</button>
            <button>=</button>
            <button>ac</button>
          </div>
          <div class="botonera-der">
            <button>+</button>
            <button>-</button>
            <button>*</button>
            <button>/</button>
          </div>
        </div>
        
      </div>
    </div>
    <div class="formulario">
      <div class="align-left">
        <span id="nombre">Bienvenido/a</span>
      </div>
    </div>
  </div>

</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",
  components: {
    /* HelloWorld */
  },
  data: () => ({}),
  computed: {},
  methods: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  display: flex;
  flex-direction: row;
  height: 97vh;
  justify-content: center;
}
.calculadora {
  background-color: gray;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-content: space-between;
  width: 70%;
  margin: 2px;
 
}
.contenedor {
  background-color: lightcoral;
  border-color: coral;
  flex: 1 0 auto;
  padding: 0.6em;
  border-radius: 1em;

}
.display {
  background-color: gray;
  color: 354E346;;
  height: 10%;
}

.botoneras {
  background-color: rgb(70, 155, 174);
  color: white;
  display: flex;
  flex-direction: row;
}

.formulario {
  background-color: rgb(146, 103, 33);
  display: flex;
  width: 30%;
 
}

.align-left {
    display: flex;
    padding: 8px;
}
#nombre {
    display: inline-block;
    margin-right: 10px;
    overflow: hidden;
    font-size: 14px;
    text-overflow: ellipsis;
    color: #fff;
}

.botonera-izq {
  width: 70%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;

}
.botoneras button {
  width: 33.3%;
  font-size: 150%;
  background: pink;
  border-radius: 0.5em;
}
.botonera-der{
  width: 30%;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
   align-items: center;
}
.botonera-der button{
  width: 70%;

}


</style>
