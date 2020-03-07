<template>
    <div>
        <b-modal :active.sync="isImageModalActive">
     
        <h1>{{text}}</h1>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea cupiditate fuga eaque unde sapiente aperiam neque, aut vel earum molestias minus placeat ducimus perferendis doloremque, dicta officia fugit incidunt iure?</p>
    </b-modal>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isImageModalActive: true
        }
    },
    props: ['text']
}
</script>