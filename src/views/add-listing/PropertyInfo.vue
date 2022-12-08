<template>
    <div style="padding: 20px" class="row">
        <div class="col-lg-10 mx-auto d-flex justify-content-center flex-column">
            <!-- <h3 class="text-center">Contact us</h3> -->
            <form role="form" id="contact-form" method="post" autocomplete="off">
                <h4 class="my-4">Property information</h4>
                <div class="card-body">
                    <h6 for="name">Title for the listing</h6>
                    <div class="col-md-12">
                        <MaterialInput class="input-group-outline mb-4" placeholder="Title for your house"
                            type="text" />
                    </div>
                    <div class="row">
                        <div class="col-md-6">
                            <h6 for="name">Type of property</h6>
                            <select placeholder="Choose" class="form-select p-2">
                                <option>GArdern</option>
                                <option>Home</option>
                                <option>3</option>
                                <option>4</option>
                            </select>
                        </div>
                        <div class="col-md-6">
                            <h6 for="name">Size M<sup>2</sup></h6>
                            <MaterialInput class="input-group-outline mb-4" placeholder="Enter number" type="text" />
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-md-6">
                            <h6 for="name">Total bedrooms</h6>
                            <MaterialInput class="input-group-outline mb-4" placeholder="Enter number" type="number" />
                        </div>
                        <div class="col-md-6">
                            <h6 for="name">Floor<sup>2</sup></h6>
                            <MaterialInput class="input-group-outline mb-4" placeholder="Enter number" type="text" />
                        </div>
                    </div>
                    <h6 for="name">Address</h6>
                    <div class="row border-bottom">
                        <GoogleMapInput />
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
    }
}
</script>