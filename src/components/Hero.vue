<template>
    <div class=" border-4 border-[#E2C799] py-20 px-10  text-gray-200   flex items-center  relative  content" >
        <div>

            <img class="w-20 md:w-32 absolute top-3 left-3" src="@/assets/corner.svg"/>
            <img class="w-20 md:w-32 absolute top-3  right-3" src="@/assets/corner.svg" style="transform: scalex(-1);"/>
            <img class="w-20 md:w-32 absolute bottom-3 right-3" src="@/assets/corner.svg" style="transform: scaleX(-1) scaleY(-1);"/>
            <img class="w-20 md:w-32 absolute bottom-3 left-3" src="@/assets/corner.svg" style="transform: scaleY(-1);"/>
          
        </div>

  
        <div class="w-full px-5 flex flex-col">
            <div class="flex text-[3vw] md:text-[4vw] font-bold poppins "> {{ content.schoolName }}</div>
           
            <HeroTitle :title="content.title1"/>
            <div class="flex text-[3vw] md:text-[5vw] mt-4 justify-center items-center rochester ">
                <div class="  md:h-20 pr-2  mr-2 md:pr-4  md:pr-4  md:mr-4  border-r-2 md:border-r-8 flex items-center border-[#E2C799]">
                    {{ content.title2 }}
                    
                </div>

              
                
                <div class="">
                    {{ content.date }}
                </div>
            </div>


        </div>

    </div>
</template>

<script>
import { useContentStore } from '@/store/content'
import { storeToRefs } from 'pinia'
import HeroTitle from './HeroTitle.vue'
export default {
    components:{HeroTitle},
    setup() {
        const contentStore = useContentStore()

        const { content } = storeToRefs(contentStore)
        return {
            content
        }
    }

}
</script>

<style>

.content{
    z-index: 0 !important;
}
</style>