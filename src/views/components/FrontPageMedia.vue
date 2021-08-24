<template> 
<div class="   pt-8   pb-2 mb-12 text-white" style="min-height:300px">
            
            


            <div class="  flex flex-col" >
            <div class="my-4 inline-block" >
                
               Useful tools for the Shadow Super Coders
               </div> 
               <div class="my-4 inline-block" >

                  
              </div> 
 
                
           </div> 


 </div>
 </template>



<script>
    export default {
    name: 'FrontPageMedia',
    props: [ ],
    data() {
        return {
            startTime: 0
        }
    },
    created(){
        this.startTime= Date.now()

        setInterval(this.update,500)
    },
    methods: {
         update(){
             this.$forceUpdate()
         },
         getTimeElapsed(){
             return Date.now() - this.startTime
         }
    }
    }
</script>
