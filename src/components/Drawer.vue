<template>
  <div class="drawer ">
    <input id="my-drawer" type="checkbox" class="drawer-toggle" />
    <div class="drawer-content">
      <!-- Page content here -->
      <label for="my-drawer" class="btn btn-primary drawer-button fixed top-3 left-3 ">Edit Content</label>
     
    </div> 
    <div class="drawer-side z-99 ">
      <label for="my-drawer" aria-label="close sidebar" class="drawer-overlay"></label>
      <ul class="menu p-4 w-80 min-h-full bg-base-200 text-base-content ">

        <div class="mt-10">

          <input type="text "  v-model="content.schoolName" placeholder="School Name" class="input input-bordered w-full max-w-xs my-1" />

<input type="text " v-model="content.title1" placeholder="Title 1" class="input input-bordered w-full max-w-xs my-1" />
<input type="text" v-model="content.title2" placeholder="Title 2" class="input input-bordered w-full max-w-xs my-1" />
<input type="text" v-model="content.date" placeholder="Date" class="input input-bordered w-full max-w-xs my-1" />
        </div>
     
      </ul>
    </div>
  </div>
</template>

<script>
import { useContentStore } from '@/store/content'
import { storeToRefs } from 'pinia'
export default {

  setup(){
    const contentStore = useContentStore()

    const {content} = storeToRefs(contentStore)

    return {
      content
    }
  }
}
</script>

<style>
.drawer{
    z-index: 99 !important;
}
</style>