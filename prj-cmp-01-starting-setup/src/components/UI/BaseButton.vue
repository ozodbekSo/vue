<template>
    <button :type="type" :class="caption"></button>
    
</template>

<script>
export default {
    props: ['type', 'mode', 'caption']
}
</script>

<style scoped>

button {
    padding: 0.75rem 1.5 rem;
    font-family: inherit;
    background-color: #3a0061;
    border: 1px solid #3a0061;
    color: black;
    cursor: pointer;
}

button:hover,
:button:active {
    background-color: transparent;
    border-color: #270041;
}

.flat {
    background-color:transparent;
    color: #3a0061;
    border: none;
}

.flat:hover,
.flat.active {
    background-color: #edd2ff;
}

</style>