<script lang="ts">//e possivel utilizar <script setup> que tem a mesma funcao do export default, assim deixando o codigo mais enxuto
import Banner from './components/Banner.vue';
import ConteudoPrincipal from './components/ConteudoPrincipal.vue';

export default {
    components: { Banner, ConteudoPrincipal} //para declarar o componente, o mesmo deve estar dentro de components: { Banner, ConteudoPrincipal, . . . }
}
</script>

<template>
    <Banner /> 
    <ConteudoPrincipal />
</template>


