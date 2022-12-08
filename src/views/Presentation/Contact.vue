<script setup>
//Vue Material Kit 2 components
import MaterialButton from "@/components/MaterialButton.vue";
import MaterialInput from "@/components/MaterialInput.vue";
import MaterialTextArea from "@/components/MaterialTextArea.vue";
import MaterialSwitch from "@/components/MaterialSwitch.vue";
import MaterialCheckbox from "@/components/MaterialCheckbox.vue";
import PrizingSlide from '@/components/PrizingSlide.vue'
</script>
<style>
.modal-dialog {
    max-width: 900px !important;
}
</style>
<template>
    <div class="container">
        <div class="row">
            <div class="col-sm-3 col-md-4 mx-auto">

                <!-- Modal -->
                <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel"
                    aria-hidden="true">
                    <div class="modal-dialog">
                        <div class="modal-content">
                            <div class="modal-header justify-content-between">
                                <MaterialButton color="none" class="btn-close" data-bs-dismiss="modal"
                                    aria-label="Close">
                                    Close
                                </MaterialButton>
                                <i data-bs-dismiss="modal" style="font-size: 1.4rem; cursor: pointer;" class="material-icons" aria-hidden="true">close</i>
                            </div>
                            <div class="modal-body">
                                <div class="row">
                                    <div class="col-lg-10 mx-auto my-4 d-flex justify-content-center flex-column">
                                        <!-- <h3 class="text-center">Contact us</h3> -->
                                        <div class="container">
                                            <div class="row">
                                                <div class="mx-auto d-flex justify-content-center flex-column">
                                                    <h3 class="text-center">Contact with mr X</h3>
                                                    <form role="form" id="contact-form" method="post"
                                                        autocomplete="off">
                                                        <div class="card-body">
                                                            <div class="row">
                                                                <div class="col-md-6">
                                                                    <MaterialInput class="input-group-dynamic mb-4"
                                                                        :label="{ text: 'First Name', class: 'form-label' }"
                                                                        type="text" />
                                                                </div>
                                                                <div class="col-md-6 ps-2">
                                                                    <MaterialInput class="input-group-dynamic"
                                                                        :label="{ text: 'Last Name', class: 'form-label' }"
                                                                        type="text" />
                                                                </div>
                                                            </div>
                                                            <div class="mb-4">
                                                                <MaterialInput class="input-group-dynamic"
                                                                    :label="{ text: 'Enter your phone number', class: 'form-label' }"
                                                                    type="tel" />
                                                            </div>
                                                            <MaterialTextArea class="input-group-static mb-4"
                                                                id="message" :rows="4">Your message
                                                            </MaterialTextArea>
                                                        </div>
                                                        <div class="row">
                                                            <div class="col-md-12">
                                                                <div class="col-md-12">
                                                                    <MaterialButton type="submit" variant="gradient"
                                                                        color="dark" fullWidth>Send Message
                                                                    </MaterialButton>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </form>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
