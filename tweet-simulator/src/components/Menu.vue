<template>
    <nav class="navbar navbar-dark bg-dark">
        <div class="container">
            <span class="navbar-brand">Simulador de Tweets</span>
            <button class="btn pl-4 pr-4 btn-success" 
                    :class="{'btn-success': !showForm, 'btn-danger':showForm}"    
                    @click="openCloseForm">
                Nuevo Tweet
                {{!showForm ? "Nuevo Tweet" : "Crear Usuario"}}
            </button>
        </div>
    </nav>
</template>

<script>
export default {
    props:{
        showForm: Boolean,
        openClosedForm: Function,
    }

}
</script>

<style>

</style>