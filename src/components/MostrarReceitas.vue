<script lang="ts">
import { obterReceitas } from '@/http';
import type IReceita from '@/interfaces/IReceita';
import BotaoPrincipal from './BotaoPrincipal.vue';
import CardReceita from './CardReceita.vue';

export default {
    data() {
        return {
            receitasEncontradas: [] as IReceitas[]
        };
    },
    async created() {
        const receitas = await obterReceitas();

        this.receitasEncontradas = receitas.slice (0, 8);
    },
    components: {BotaoPrincipal, CardReceita},
    emits: ['editarReceitas']
}

</script>


<template>
<section class="mostrar-receitas">

<h1 class="cabecalho titulo-receitas">Receitas</h1>

<p class="paragrafo-lg resultados-encontrados">
    Resultados encontrados: {{ receitasEncontradas.length }}
</p>


</section>

</template>