<template>

<div class="bloc-modale" v-if="revele">

    <div class="overlay" v-on:click="toggleModale"></div>

    <div class="modale card">
        <div v-on:click="toggleModale" class="btn-modale btn btn-danger">X</div>
        <h2>Le contenu de la modale de test s'affichera ici</h2>
        
    </div>
</div>
</template>


<script>

export default {
    name: 'Modale',
    props: ['revele','toggleModale']
}

</script>


<style scoped>
.bloc-modale {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: center;
    align-items: center;

}

.overlay {
    background: rgba(0,0,0,0.5);
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
}

.modale {
    background: (f1,f1,f1);
    color: #333;
    padding: 50px;
    position: fixed;
    top: 30%;

}

.btn-modale {
    position: absolute;
    top: 10px;
    right: 10px;
}

.btn {
    .box-shadow::after {
    content: "";
    display: block;
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    box-shadow: 0 0 20px 10px rgba(0, 0, 0, 0.5);
}
}

</style>