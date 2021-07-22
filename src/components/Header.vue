<template>
      <header class="shadow w-screen">
       <nav>
           <nav class="flex items-center justify-between flex-wrap bg-green-400 p-6">
               <div class="flex items-center flex-shrink-0 text-white mr-6">
                 <LogoHeader />
                   <router-link :to="{name: 'home'}" class="font-semibold text-xl tracking-tight">Thierno Exchange</router-link>
               </div>
               <div class="hidden sm:block w-full block flex-grow lg:flex lg:items-center lg:w-auto">
          <div class="text-sm lg:flex-grow">
            <router-link
              v-for="l in links"
              :key="l.title"
              :to="l.to"
              class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4"
            >{{ l.title }}</router-link>
          </div>
                  
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
  },
  props:{
links:{
type:Array,
default:() => []
}
  },
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
