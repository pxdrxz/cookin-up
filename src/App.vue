<script lang="ts"> //e possivel utilizar <script setup> que tem a mesma funcao do export default, assim deixando o codigo mais enxuto
import Banner from './components/Banner.vue';

export default {
components: { Banner: Banner } //components->objeto / <Banner/> = Banner (logo "Banner : Banner")
}
</script>

<template>
 <Banner/>
</template>

