<template>
      <header class="shadow w-screen">
       <nav>
           <nav class="flex items-center justify-between flex-wrap bg-green-400 p-6">
               <div class="flex items-center flex-shrink-0 text-white mr-6">
                 <LogoHeader />
                   <span class="font-semibold text-xl tracking-tight">PlatziExchange</span>
               </div>
               <div class="hidden sm:block w-full blok flex-grow lg:flex lg:items-center lg:wauto">
                   <div class="text-sm lg:flex-grow"></div>
               </div>
           </nav>
       </nav>
    </header> 
</template>

<script>
import LogoHeader from '@/components/LogoHeader.vue'

export default {
  name: 'HelloWorld',
  components: {
   LogoHeader
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
