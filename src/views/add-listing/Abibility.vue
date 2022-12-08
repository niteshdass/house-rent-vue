<template>
    <div style="padding: 20px" class="row">
        <div class="col-lg-10 mx-auto d-flex justify-content-center flex-column">
            <!-- <h3 class="text-center">Contact us</h3> -->
            <form role="form" id="contact-form" method="post" autocomplete="off">
                <h4 class="my-4">Availability and rent</h4>
                <div class="card-body">
                    <div class="row">
                        <div class="col-md-6">
                            <h6 for="name">Available</h6>
                            <div class="row">
                                <div class="col-md-6">
                                    <MaterialInput class="input-group-outline mb-4" placeholder="Title for your house"
                                    type="date" />
                                </div>
                                <div class="col-md-6">
                                    <MaterialInput class="input-group-outline mb-4" placeholder="Enter number"
                                        type="date" />
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <h6 for="name">Minimum stay</h6>
                            <MaterialInput class="input-group-outline mb-4" placeholder="Months" type="text" />
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-md-6">
                            <h6 for="name">Monthly rent</h6>
                            <MaterialInput class="input-group-outline mb-4" placeholder="Amount" type="number" />
                        </div>
                        <div class="col-md-6">
                            <h6 for="name">Deposite</h6>
                            <MaterialInput class="input-group-outline mb-4" placeholder="Amount" type="text" />
                        </div>
                    </div>
                    <!-- <div class="row border-bottom">
                        <GoogleMapInput />
                    </div>
                    <h6 for="name">Area</h6>
                    <div class="row border-bottom">
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Lamabazar
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Subidbazar
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Bagbari
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Modina market
                            </MaterialCheckbox>
                        </div>
                    </div>
                    <h6 for="name">Number of bedrooms</h6>
                    <div class="row border-bottom">
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                1
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                2
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                3
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                4
                            </MaterialCheckbox>
                        </div>
                    </div>
                    <h6 for="name">Available from</h6>
                    <div class="row border-bottom">
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                January
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                February
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                March
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                April
                            </MaterialCheckbox>
                        </div>
                    </div>
                    <h6 for="name">Rent prize</h6>
                    <div class="row border-bottom">
                        <div class="form-check col-md-4">
                            <PrizingSlide />
                        </div>
                    </div>
                    <h6 for="name">Included in rent</h6>
                    <div class="row border-bottom">
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Cable TV
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Common Room Cleaning
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Electricity
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Gas
                            </MaterialCheckbox>
                        </div>
                        <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished">
                                Water
                            </MaterialCheckbox>
                        </div>
                    </div> -->
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