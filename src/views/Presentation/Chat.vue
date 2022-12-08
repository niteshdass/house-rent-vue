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
    <section>
        <div class="container py-5">

            <div class="row">

                <div class="col-md-6 col-lg-5 col-xl-4 mb-4 mb-md-0">

                    <h5 class="font-weight-bold mb-3 text-center text-lg-start">Member</h5>

                    <div class="card">
                        <div class="card-body">

                            <ul class="list-unstyled mb-0">
                                <li class="p-2 border-bottom" style="background-color: #eee;">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-8.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">John Doe</p>
                                                <p class="small text-muted">Hello, Are you there?</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">Just now</p>
                                            <span class="badge bg-success float-end">1</span>
                                        </div>
                                    </a>
                                </li>
                                <li class="p-2 border-bottom">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-1.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">Danny Smith</p>
                                                <p class="small text-muted">Lorem ipsum dolor sit.</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">5 mins ago</p>
                                        </div>
                                    </a>
                                </li>
                                <li class="p-2 border-bottom">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-2.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">Alex Steward</p>
                                                <p class="small text-muted">Lorem ipsum dolor sit.</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">Yesterday</p>
                                        </div>
                                    </a>
                                </li>
                                <li class="p-2 border-bottom">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-3.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">Ashley Olsen</p>
                                                <p class="small text-muted">Lorem ipsum dolor sit.</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">Yesterday</p>
                                        </div>
                                    </a>
                                </li>
                                <li class="p-2 border-bottom">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-4.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">Kate Moss</p>
                                                <p class="small text-muted">Lorem ipsum dolor sit.</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">Yesterday</p>
                                        </div>
                                    </a>
                                </li>
                                <li class="p-2 border-bottom">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-5.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">Lara Croft</p>
                                                <p class="small text-muted">Lorem ipsum dolor sit.</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">Yesterday</p>
                                        </div>
                                    </a>
                                </li>
                                <li class="p-2">
                                    <a href="#!" class="d-flex justify-content-between">
                                        <div class="d-flex flex-row">
                                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-6.webp"
                                                alt="avatar"
                                                class="rounded-circle d-flex align-self-center me-3 shadow-1-strong"
                                                width="60">
                                            <div class="pt-1">
                                                <p class="fw-bold mb-0">Brad Pitt</p>
                                                <p class="small text-muted">Lorem ipsum dolor sit.</p>
                                            </div>
                                        </div>
                                        <div class="pt-1">
                                            <p class="small text-muted mb-1">5 mins ago</p>
                                            <span class="text-muted float-end"><i class="fas fa-check"
                                                    aria-hidden="true"></i></span>
                                        </div>
                                    </a>
                                </li>
                            </ul>

                        </div>
                    </div>

                </div>

                <div class="col-md-6 col-lg-7 col-xl-8">

                    <ul class="list-unstyled">
                        <li class="d-flex justify-content-between mb-4">
                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-6.webp" alt="avatar"
                                class="rounded-circle d-flex align-self-start me-3 shadow-1-strong" width="60">
                            <div class="card">
                                <div class="card-header d-flex justify-content-between p-3">
                                    <p class="fw-bold mb-0">Brad Pitt</p>
                                    <p class="text-muted small mb-0"><i class="far fa-clock"></i> 12 mins ago</p>
                                </div>
                                <div class="card-body">
                                    <p class="mb-0">
                                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                        incididunt ut
                                        labore et dolore magna aliqua.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="d-flex justify-content-between mb-4">
                            <div class="card w-100">
                                <div class="card-header d-flex justify-content-between p-3">
                                    <p class="fw-bold mb-0">Lara Croft</p>
                                    <p class="text-muted small mb-0"><i class="far fa-clock"></i> 13 mins ago</p>
                                </div>
                                <div class="card-body">
                                    <p class="mb-0">
                                        Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
                                        doloremque
                                        laudantium.
                                    </p>
                                </div>
                            </div>
                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-5.webp" alt="avatar"
                                class="rounded-circle d-flex align-self-start ms-3 shadow-1-strong" width="60">
                        </li>
                        <li class="d-flex justify-content-between mb-4">
                            <img src="https://mdbcdn.b-cdn.net/img/Photos/Avatars/avatar-6.webp" alt="avatar"
                                class="rounded-circle d-flex align-self-start me-3 shadow-1-strong" width="60">
                            <div class="card">
                                <div class="card-header d-flex justify-content-between p-3">
                                    <p class="fw-bold mb-0">Brad Pitt</p>
                                    <p class="text-muted small mb-0"><i class="far fa-clock"></i> 10 mins ago</p>
                                </div>
                                <div class="card-body">
                                    <p class="mb-0">
                                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                        incididunt ut
                                        labore et dolore magna aliqua.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="bg-white mb-3">
                            <div class="form-outline">
                                <textarea class="form-control" id="textAreaExample2" rows="4"></textarea>
                                <label class="form-label" for="textAreaExample2">Message</label>
                            </div>
                        </li>
                        <button type="button" class="btn btn-info btn-rounded float-end">Send</button>
                    </ul>

                </div>

            </div>

        </div>
    </section>
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
