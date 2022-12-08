<template>
    <div style="padding: 20px" class="row">
        <div class="col-lg-10 mx-auto d-flex justify-content-center flex-column">
            <!-- <h3 class="text-center">Contact us</h3> -->
            <form role="form" id="contact-form" method="post" autocomplete="off">
                <h4 class="my-4">About</h4>
                <div class="card-body">
                    <div class="row">
                        <div class="col-md-12">
                            <h6 for="name">Describe the property and area</h6>
                            <MaterialTextArea placeholder="Type description" />
                        </div>
                    </div>
                </div>
                <h4 class="my-4">Property photos</h4>
                <div class="card-body">
                    <div class="row">
                        <div class="col-md-12">
                            <h6 for="name">Describe the property and area</h6>
                            <div class="col-md-12">
                                <form>
                                    <div class="form-group">
                                        <div style="border: 2px dashed #b7b8bc; text-align:center; padding: 20px">
                                            <input type="file" accept="image/*" multiple="multiple"
                                                @change="previewMultiImage" class="form-control-file" id="my-file">
                                        </div>
                                        <div class="border p-2 mt-3">
                                            <div>
                                                <p>Preview Here:</p>
                                            </div>
                                            <template v-if="preview_list.length" class="container">
                                                <div v-for="item, index in preview_list" :key="index" style="max-width: 100%">
                                                    <i @click="reset(index)" style="font-size: 2.0rem;"
                                                        class="material-icons cancel-button"
                                                        aria-hidden="true">cancel</i>
                                                    <img :src="item" class="img-fluid" />
                                                    <p class="mb-0">file name: {{ image_list[index].name }}</p>
                                                    <p>size: {{ image_list[index].size/1024 }}KB</p>
                                                </div>
                                            </template>
                                        </div>
                                    </div>
                                </form>
                            </div>
                        </div>
                    </div>
                </div>
            </form>
        </div>
    </div>
</template>
<script>
import MaterialInput from "@/components/MaterialInput.vue";
import MaterialTextArea from "@/components/MaterialTextArea.vue";
import MaterialButton from "@/components/MaterialButton.vue";
import MaterialSwitch from "@/components/MaterialSwitch.vue";
import MaterialCheckbox from "@/components/MaterialCheckbox.vue";
import GoogleMapInput from '@/components/GoogleMapInput.vue';
export default {
    components: {
        MaterialButton,
        MaterialInput,
        MaterialTextArea,
        MaterialSwitch,
        MaterialCheckbox,
        GoogleMapInput,
    },
    data() {
        return {
            preview_list: [],
            image_list: []
        }
    },
    methods: {
        previewMultiImage: function (event) {
            var input = event.target;
            var count = input.files.length;
            var index = 0;
            if (input.files) {
                while (count--) {
                    var reader = new FileReader();
                    reader.onload = (e) => {
                        this.preview_list.push(e.target.result);
                    }
                    this.image_list.push(input.files[index]);
                    reader.readAsDataURL(input.files[index]);
                    index++;
                }
            }
        },
        reset: function (index) {
            this.preview_list.splice(index, 1); // 2nd parameter means remove one item only
            this.image_list.splice(index, 1);
        }
    }
}
</script>
<style>
.cancel-button:hover {
    cursor: pointer;
}
</style>