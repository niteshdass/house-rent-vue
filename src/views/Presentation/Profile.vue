<script setup>
import { onMounted, onUnmounted } from "vue";

//example components
import NavbarDefault from "../..//examples/navbars/NavbarDefault.vue";
import PropertyCard from '@/views/Presentation/PropertyCard.vue';

const imageLink = [
    'https://img.freepik.com/free-psd/realistic-modern-double-bedroom-with-furniture-frame_176382-437.jpg?w=2000&t=st=1665840139~exp=1665840739~hmac=098d75b6cce96ee0a418f7c86e50a185c61f46b1208d81c37a4ab437fa7c38a6',
    'https://img.freepik.com/free-photo/modern-studio-apartment-design-with-bedroom-living-space_1262-12375.jpg?w=2000&t=st=1665840313~exp=1665840913~hmac=c0ce35e37f9e8f243d701a8058b36598655a673101c01a40db8c031cc55a83b9',
    'https://img.freepik.com/free-psd/realistic-modern-double-bedroom-with-furniture-frame_176382-442.jpg?w=2000&t=st=1665840350~exp=1665840950~hmac=46a890e516f32842c753bed9b0534d19ba7878787a71be69ce1b994f9cb92798'
]
//hooks
const body = document.getElementsByTagName("body")[0];
onMounted(() => {
    body.classList.add("presentation-page");
    body.classList.add("bg-gray-200");
});
onUnmounted(() => {
    body.classList.remove("presentation-page");
    body.classList.remove("bg-gray-200");
});
</script>

<template>
    <div class="container position-sticky z-index-sticky top-0">
        <div class="row">
            <div class="col-12">
                <NavbarDefault :sticky="true" />
            </div>
        </div>
    </div>
    <div class="container pt-6 mt-6">
        <div class="row border-bottom pt-6">
            <div class="col-md-4 mt-3 font">
                <div class="card">
                    <img class="card-img-top"
                        src="https://img.freepik.com/free-vector/white-abstract-background-design_23-2148825582.jpg?w=2000&t=st=1666089604~exp=1666090204~hmac=0ef633e720d17ca11bcc52e3442ecc66bd0a0b4ecd6b95a562018274a941be3e"
                        alt="Bologna">
                    <div class="card-body text-center">
                        <img class="avatar rounded-circle"
                            src="https://s3.eu-central-1.amazonaws.com/bootstrapbaymisc/blog/24_days_bootstrap/robert.jpg"
                            alt="Bologna">
                        <h4 class="card-title">Robert Downey Jr.</h4>
                        <h6 class="card-subtitle mb-2 text-muted">Famous Actor</h6>
                        <button style="width: 100%" class="btn btn-success" data-bs-toggle="modal"
                            data-bs-target="#exampleModal">Message</button>
                    </div>
                </div>
                <div class="mt-3 p-4">
                    <button style="width: 100%" class="btn btn-white">Personal info</button>
                    <button style="width: 100%" class="btn btn-white">Settings</button>
                    <button style="width: 100%" class="btn btn-white">Listing list</button>
                </div>
            </div>
            <div class="col-md-8 mb-8">
                <h3 class="mt-4">Personal info</h3>
                <div class="card">
                    <div class="px-4 py-2" style="display: flex">
                        <h6 class="px-2">Name:</h6>
                        <h6>Nitesh Das</h6>
                    </div>
                    <div class="px-4 py-2" style="display: flex">
                        <h6 class="px-2">Gmail:</h6>
                        <h6>dasnitesh780@gmail.com</h6>
                    </div>
                    <div class="px-4 py-2" style="display: flex">
                        <h6 class="px-2">Phone:</h6>
                        <h6>01747102896</h6>
                    </div>
                    <div class="px-4 py-2" style="display: flex">
                        <h6 class="px-2">About:</h6>
                        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has
                            been the industry's standard dummy text ever since the 1500s, when an unknown printer took a
                            galley of type and scrambled it to make a type specimen book. It has survived not only five
                            centuries, but also the leap into electronic typesetting, remaining essentially unchanged.
                            It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum
                            passages, and more recently with desktop publishing software like Aldus PageMaker including
                            versions of Lorem Ipsum</p>
                    </div>
                </div>
                <h3 class="mt-4">Listing's</h3>
                <div class="card mt-5">
                    <div class="row">
                        <div class="col-md-6">
                            <PropertyCard :action="{label: 'Edit' , color: 'bg-gradient-info'}" :image="imageLink"
                        title="3 Bed room | 2 dining | 1 kitchen | 1 living room | 1 bathroom"
                        location="Arnab 48/2, Mirermoydan, lamabazar, Sylhet" price="10000" />
                        </div>
                        <div class="col-md-6">
                            <PropertyCard :image="imageLink"
                        title="3 Bed room | 2 dining | 1 kitchen | 1 living room | 1 bathroom"
                        location="Arnab 48/2, Mirermoydan, lamabazar, Sylhet" price="10000" />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div style="padding-bottom: 100px;">
    </div>
</template>

<style>
.round-icon {
    font-size: 1.4rem;
    margin-right: 2px;
    border-radius: 50%;
    background-color: white;
    color: green;
    padding: 2px;
}

.avatar {
    border: 0.3rem solid rgba(#fff, 0.3);
    margin-top: -16rem;
    margin-bottom: 1rem;
    width: 16rem !important;
    height: 17rem !important;
}

.badge-item {
    background-color: #bab0b017;
    border-radius: 5%;
    padding-top: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    margin-right: 10px;
}

.box-inventory {
    text-align: center;
    box-shadow: 0px 0.8px 1px 1px rgb(236, 234, 234);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
</style>
