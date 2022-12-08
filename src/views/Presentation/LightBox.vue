<template>
    <div class="container pt-4">
        <h2>Sentral 3-roms leilighet i 3.etasje. Nyoppusset | Balkong | Heis | Hvitevarer</h2>
        <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
            <i style="font-size: 1.4rem;" class="material-icons" aria-hidden="true">location_on</i>
            <span>Lamabazar sylhet</span>
        </p>
        <div class="row">
            <div class="col-md-4 text-white">
                <button @click="showMultiple" style="border: none">
                    <img style="max-width: 100%" :src="imagaes[0]" class="rounded" alt="Cinque Terre" />
                </button>
            </div>
            <div class="col-md-4 text-white">
                <button @click="showMultiple" style="border: none">
                    <img style="max-width: 100%" :src="imagaes[1]" class="rounded" alt="Cinque Terre" />
                </button>
            </div>
            <div class="col-md-4 text-white">
                <button @click="showMultiple" style="border: none">
                    <img style="max-width: 100%" :src="imagaes[2]" class="rounded" alt="Cinque Terre" />
                </button>
            </div>
        </div>
        <VueEasyLightbox :visible="visible" :imgs="imgs" :index="index" @hide="handleHide"></VueEasyLightbox>
    </div>
</template>
  
<script>
import VueEasyLightbox from 'vue-easy-lightbox';
import slide1 from '@/assets/img/slide1.jpg';
import slide2 from '@/assets/img/slide2.jpg';
import slide3 from '@/assets/img/slide3.jpg';


export default {
    components: {
        VueEasyLightbox
    },
    data() {
        return {
            imgs: '',  // Img Url , string or Array
            visible: false,
            index: 0,   // default
            imagaes: [slide1, slide2, slide3]
        }
    },
    methods: {
        showSingle() {
            this.imgs = slide1;
            this.show()
        },
        showMultiple() {
            this.imgs = [slide1, slide2, slide3]
            this.index = 1  // index of imgList
            this.show()
        },
        show() {
            this.visible = true
        },
        handleHide() {
            this.visible = false
        }
    }
}
</script>