<template>
    <div id="main">
        <h1>{{ mensaje }}</h1>
        <form>
            <input type="text" id="input_text" v-model="input_text" value="Steven" >
            <label for="input_text">Texto</label>
            <input type="date" name="" id="date" placeholder="Fecha">
            <label for="date">Fecha</label>
            <input type="email" name="" id="email" placeholder="Email">
            <label for="">Email</label>
            <input type="file" name="" id="file" placeholder="Archivo">
            <label for="file">Archivo</label>
            <input type="image" src="" alt="img" placeholder="Imagen">
            <label for="img">Imagen</label>
            <input type="number" name="" id="number" placeholder="Numero">
            <label for="number">Numero</label>
            <input type="password" name="" id="password" placeholder="Password">
            <label for="password">Contraseña</label>
            <input type="radio" name="" id="radio" placeholder="Fecha">
            <label for="radio">Radio Button</label>
            <input type="search" name="" id="search" placeholder="Buscar">
            <label for="search">Buscar</label>
            <input type="tel" name="" id="tel" placeholder="Telefono">
            <label for="tel">Telefono</label>
            <input type="week" name="" id="Semana">
            <label for="Semana">Semana</label>
            <input type="submit" value="Steven" @click="handleSubmit">
            <input type="reset" value="">
        </form>
    </div>
</template>
<style scoped>
    #main{
        display: grid;
        align-items: center;
        align-content: center;
        height: 100vh;
    }
    h1{
        color: white;
        text-align: center;
    }
    form{
        display: grid;
        justify-content: center;
        align-items: center;
    }
</style>
<script>
    export default{
        data(){
            return{
                mensaje: "Steven",
                input_text: "",
            };
        },
        methods: {
            handleSubmit() {
                window.alert(`Steven: ${this.input_text}`);
            },
        },
    };
</script>