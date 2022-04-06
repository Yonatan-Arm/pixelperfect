<template>
<div class="items-list flex">
    <ul>
        <item-preview v-for="item in items" :item="item"  :key="item"/>
    </ul>
</div>
  
</template>

<script>
    import itemPreview from '../components/item-preview.vue'
export default {
    data(){
        return{
            items:[
                {
                 prevImg:`../assets/images/icon-access-anywhere.svg`,
                 title:'Access your files, anywhere',
                 context:'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.',
                },
                {
                 prevImg:'../assets/images/icon-security.svg',
                 title:'Security you can trust',
                 context:'2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.',
                },
                {
                 prevImg:'../assets/images/icon-collaboration.svg',
                 title:'Real-time collaboration',
                 context:'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.',
                },
                {
                 prevImg:'../assets/images/icon-any-file.svg',
                 title:'Store any type of file',
                 context:'Whether youre sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared',
                }

            ]
        }
    },
    components:{
        itemPreview,
    }

}
</script>

<style>

</style>