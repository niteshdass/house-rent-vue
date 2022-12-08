<script setup>
import MaterialSocialButton from "@/components/MaterialSocialButton.vue";

defineProps({
    image: {
        type: [],
        required: true,
    },
    title: {
        type: String,
        required: true,
    },
    location: {
        type: String,
        required: true,
    },
    price: {
        type: String,
        required: true,
    },
    action: {
        type: Object,
        color: String,
        route: String,
        label: String,
        default: () => ({
            color: "bg-gradient-success",
            label: "View Details",
        }),
    },
});
</script>
<template>
    <div class="card">
        <div class="card-header p-0 position-relative mt-n4 mx-3 z-index-2">
            <!-- Carousel -->
            <div id="demo" class="carousel slide" data-bs-ride="carousel">

                <!-- Indicators/dots -->
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#demo" data-bs-slide-to="0" class="active"></button>
                    <button type="button" data-bs-target="#demo" data-bs-slide-to="1"></button>
                    <button type="button" data-bs-target="#demo" data-bs-slide-to="2"></button>
                </div>
         <!-- <a :href="action.route" class="d-block blur-shadow-image">
        <img :src="image" :alt="title" class="img-fluid border-radius-lg" />
      </a> -->
                <!-- The slideshow/carousel -->
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img :src="image[0]" alt="Los Angeles" class="d-block" style="width:100%; max-height: 212px;">
                    </div>
                    <div class="carousel-item">
                        <img :src="image[1]" alt="Chicago" class="d-block" style="width:100%; max-height: 212px;">
                    </div>
                    <div class="carousel-item">
                        <img :src="image[1]" alt="New York" class="d-block" style="width:100%; max-height: 212px;">
                    </div>
                </div>

                <!-- Left and right controls/icons -->
                <button class="carousel-control-prev" type="button" data-bs-target="#demo" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon"></span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#demo" data-bs-slide="next">
                    <span class="carousel-control-next-icon"></span>
                </button>
            </div>
        </div>
        <div class="card-body">
            <div style="display:flex">
                <h5 class="font-weight-normal">
                    <a href="javascript:;">{{ title }}</a>
                </h5>
                <button class="btn btn-sm">
                    <i style="font-size: 2.5rem; color:#43a047;" class="material-icons" aria-hidden="true">favorite</i>
                </button>
            </div>
            <p class="mb-0">
                {{ location }}
            </p>
            <h6>{{ price }}-Tk / Month</h6>
            <div class="d-flex align-items-center">
                <i class="material-icons me-1" aria-hidden="true">bathroom</i>
                2 Bathrooms
            </div>
            <div class="d-flex align-items-center">
                <i class="material-icons me-1" aria-hidden="true">bed</i>
                2 bedrooms
            </div>
            <div class="d-flex align-items-center">
                <i class="material-icons me-1" aria-hidden="true">square</i>
                3100 sqft
            </div>
            <router-link to="/details">
                <button type="button" class="btn btn-sm mb-0 mt-3" :class="action.color">
                    {{ action.label }}
                </button>
            </router-link>
            <button style="float: right;" type="button" class="btn btn-sm mb-0 mt-3 btn-facebook">
                <i style="font-size: 1.2rem;" class="material-icons me-1" aria-hidden="true">facebook</i> Share
            </button>
            <!-- <MaterialSocialButton
              route="https://www.facebook.com/sharer/sharer.php?u=https://www.creative-tim.com/product/material-design-system-pro"
              component="facebook-square"
              color="facebook"
              label="Share"
            /> -->
        </div>
    </div>
</template>
