<template>
    <div class="comp">
        <h2>{{title}}</h2>
        <p>Teste</p>
        <form-components></form-components>
        <h2>{{msg}}</h2>
    </div>
</template>

<script>
import FormComponents from './FormComponents'
export default {
    data() {
        return{
            msg: 'Curso VueJs',
            title: 'TestComponents'
        }
    },
    components:{
        FormComponents, 
    }
}
</script>

<style scoped>
.comp{border: 1px solid red; margin: 5px; padding: 5px;}
p{color: red;}
</style>>
