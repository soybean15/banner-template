<template>
    <div class="w-full m-5 border-2 py-20 px-10 flex  justify-center items-center aspect-video max-w-[1000px]" >

        <div class="w-full px-5 flex flex-col">
            <div class="flex text-2xl font-bold poppins "> {{ content.schoolName }}</div>
           
            <HeroTitle :title="content.title1"/>
            <div class="flex text-5xl rochester">
                <div class="">
                    {{ content.title2 }}
                    
                </div>

                <div class="mx-2">|</div>
                
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

<style></style>