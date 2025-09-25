<script lang="ts">

export default {
    props: {
        prato: { type: String, required: true}
    },
}

</script>

<template>
    <section> 
        {{ prato }}
    </section>
</template>