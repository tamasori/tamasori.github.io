<template>
    <header class="row">
        <img src="../assets/logo.png" alt="Tamás Őri Logo">
        <a v-for="{icon, name, url} in menu_items" :key="name"  :href="url"><p><i :data-feather="icon"></i> {{name}}</p></a>
    </header>
</template>

<script>

    export default {
        name: "HeaderMenu",
        components:{
        },
        data: () =>{
            return {
                menu_items:[
                    {icon: 'circle', name: 'Test Name', url: '#test'},
                    {icon: 'feather', name: 'Test Name', url: '#test'},
                    {icon: 'feather', name: 'Test Name', url: '#test'},
                    {icon: 'feather', name: 'Test Name', url: '#test'},
                    {icon: 'feather', name: 'Test Name', url: '#test'},
                    {icon: 'feather', name: 'Test Name', url: '#test'},
                    {icon: 'feather', name: 'Test Name', url: '#test'},
                ],
            };
        },

    }
</script>

<style scoped>
    header{
        margin: 0;
        display: flex;
        flex: 1;
        align-items: center;
        justify-content: space-around;
        width: 60%;
        background: wheat;
        padding: 10px;
        position: fixed;
        top: 30px;
        left: 50%;
        transform: translateX(-50%);
    }

    header img{
        width: 3rem;
        height: 3rem;

    }

    header svg {
        height: .8rem;
        width: .8rem;
    }

    header a{
        height: 1rem;
    }
    header p{
        font-size: 1rem;
        line-height: 1rem;
    }
</style>