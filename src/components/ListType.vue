<template>
    <div class="container">
        <h2>Listado de elementos por Tipo</h2>
        <ListDefault :elementsList="elements"/>
    </div>
</template>
<script>
import ListDefault from '../partials/_ListDefault'
export default {
    components: {
        ListDefault
    },
    created(){
        this.findAll()
    },

    data(){
        return{
            elements: []
        };
    },
    methods: {
        findAll: function(){
            fetch('http://127.0.0.1:8000/api/type/'+this.$route.params.id+'/elements/?format=json')
            .then(res => res.json())
            .then(res => this.elements=res)
        }
    },
    
}
</script>
<style >
    .box {
        border: 3px solid #ccc;
        margin: 5px 0 0 0;
    }
</style>