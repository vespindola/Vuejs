<template>
    <div class="comp">
        <h2>{{title}}</h2>
        <table>
            <tr>
                <td>Nome</td>
                <td>Completada?</td>
            </tr>
            <tr v-for="(task, index) in tasks" :key="index">
                <td>{{task.name}}</td>
                <td>{{task.completed ? 'sim' : 'não'}}</td>
            </tr>
        </table>
    </div>
</template>

<script>
export default {
    data (){
        return{
            tasks:[
                {name: 'Arrumar quarto', completed: true},
                {name: 'Formatar computador', completed: false},
                {name: 'Assistir TV', completed: true},
                {name: 'Desenvolver sistema', completed: true},
            ],
            title: 'TaskComponents'
        }
    }
}
</script>

<style scoped>
.comp{border: 1px solid yellow; margin: 5px; padding: 5px;}
</style>