<template>
    <div>
        <vue-google-autocomplete ref="address" id="map" types="regions)" classname="form-control input-group-outline"
            placeholder="Please type your address" v-on:placechanged="getAddressData" country="bd">
        </vue-google-autocomplete>
    </div>
</template>
<script>
import VueGoogleAutocomplete from 'vue-google-autocomplete';
export default {
    components: {
        VueGoogleAutocomplete
    },
    data: function () {
        return {
            address: "",
        };
    },
    mounted() {
        // To demonstrate functionality of exposed component functions
        // Here we make focus on the user input
        this.$refs.address.focus();
    },

    methods: {
        /**
         * When the location found
         * @param {Object} addressData Data of the found location
         * @param {Object} placeResultData PlaceResult object
         * @param {String} id Input container ID
         */
        getAddressData: function (addressData, placeResultData, id) {
            console.log(addressData, id, placeResultData)
            this.address = addressData;
        },
    },
}
</script>