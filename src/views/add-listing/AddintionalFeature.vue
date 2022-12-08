<template>
    <div style="padding: 20px" class="row">
        <div class="col-lg-10 mx-auto d-flex justify-content-center flex-column">
            <!-- <h3 class="text-center">Contact us</h3> -->
            <form role="form" id="contact-form" method="post" autocomplete="off">
                <h4 class="my-4">Rooms and inventory</h4>
                <div class="card-body">
                    <div class="row">
                        <h6 for="name">Title for the listing</h6>
                        <div class="col-md-12" style="display: flex; margin-bottom: 10px;">
                            <div class="form-check">
                                <input type="radio" class="form-check-input mx-2" id="radio1" name="optradio"
                                    value="option1" checked>Unfurnished
                                <label class="form-check-label" for="radio1"></label>
                            </div>
                            <div class="form-check">
                                <input type="radio" class="form-check-input mx-2" id="radio2" name="optradio"
                                    value="option2">Furnished
                                <label class="form-check-label" for="radio2"></label>
                            </div>
                            <div class="form-check">
                                <input type="radio" class="form-check-input mx-2" id="radio2" name="optradio"
                                    value="option2">Party Furnished
                                <label class="form-check-label" for="radio2"></label>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <h6 for="name">Type of rooms</h6>
                        <div class="col-md-6">
                            <div class="row">
                                <div class="col-md-8">
                                    <MaterialCheckbox id="unfurnished" label="Furnished">
                                        Bedroom
                                    </MaterialCheckbox>
                                </div>
                                <div class="col-md-3 mini-input">
                                    <input class="mini-input" type="number" value="1" />
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="row">
                                <div class="col-md-8">
                                    <MaterialCheckbox id="unfurnished" label="Furnished">
                                        Bathroom
                                    </MaterialCheckbox>
                                </div>
                                <div class="col-md-3 mini-input">
                                    <input class="mini-input" type="number" value="1" />
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="row">
                                <div class="col-md-8">
                                    <MaterialCheckbox id="unfurnished" label="Furnished">
                                        Living Room
                                    </MaterialCheckbox>
                                </div>
                                <div class="col-md-3 mini-input">
                                    <input class="mini-input" type="number" value="1" />
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="row">
                                <div class="col-md-8">
                                    <MaterialCheckbox id="unfurnished" label="Furnished">
                                        Kitchen
                                    </MaterialCheckbox>
                                </div>
                                <div class="col-md-3 mini-input">
                                    <input class="mini-input" type="number" value="1" />
                                </div>
                            </div>
                        </div>
                    </div>
                    <h4 class="my-4">Included in rent</h4>
                    <div class="row">
                        <div class="col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Comon room cleaning
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Cable tv
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Electricity
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Gas
                            </MaterialCheckbox>
                        </div>
                        <div class="col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Heating
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Hot water
                            </MaterialCheckbox>
                        </div>
                        <div class="col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Internet
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Parking
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Private room cleaning
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Water
                            </MaterialCheckbox>
                        </div>
                    </div>
                    <h4 class="my-4">Facilities</h4>
                    <div class="row">
                        <div class="col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Aircondition
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Alarm
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Broadband Internet
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Charging Options
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Elevator
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Garden
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Pool
                            </MaterialCheckbox>
                        </div>
                        <div class="col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                No Insight
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Pets Allowed
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Smoking Allowed
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Laundromat
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Cabal-TV
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Dishwasher
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Kids-Friendly
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Microwave
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Parking / Garage
                            </MaterialCheckbox>
                        </div>
                        <div class="col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Laundromat
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Fireplace
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Oven
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                TV
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Balcony
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Calm
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Dryer
                            </MaterialCheckbox>
                            <MaterialCheckbox id="unfurnished" label="Furnished">
                                Fridge
                            </MaterialCheckbox>
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
<style scoped>
.mini-input {
    max-height: 28px;
    max-width: 37px;
    font-size: 13px;
    font-weight: 500;
    color: gray;
    text-align: center;
}
</style>