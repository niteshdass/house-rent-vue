<script>
import { onMounted, onUnmounted } from "vue";

//example components
import NavbarDefault from '@/examples/navbars/NavbarDefault.vue';
import PropertyInfo from '@/views/add-listing/PropertyInfo.vue';
import Abibility from '@/views/add-listing/Abibility.vue';
import AddintionalFeature from '@/views/add-listing/AddintionalFeature.vue';
import DescriptionMedia from '@/views/add-listing/DescriptionMedia.vue';

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

export default {
    components: {
        NavbarDefault,
        PropertyInfo,
        Abibility,
        AddintionalFeature,
        DescriptionMedia
    },
    data() {
        return {
            activeItem: 1,
        }
    },
    mounted() {
        const stepButtons = document.querySelectorAll('.step-button');
        const progress = document.querySelector('#progress');

        Array.from(stepButtons).forEach((button, index) => {
            button.addEventListener('click', () => {
                progress.setAttribute('value', index * 100 / (stepButtons.length - 1));//there are 3 buttons. 2 spaces.

                stepButtons.forEach((item, secindex) => {
                    if (index > secindex) {
                        item.classList.add('done');
                    }
                    if (index < secindex) {
                        item.classList.remove('done');
                    }
                })
            })
        })
    },
}
</script>

<template>
    <div class="container position-sticky z-index-sticky top-0">
        <div class="row">
            <div class="col-12">
                <NavbarDefault :sticky="true" />
            </div>
        </div>
    </div>
    <div>

        <section>
            <div class="container col-md-6">
                <div class="accordion" id="accordionExample">
                    <div class="steps">
                        <progress id="progress" value=0 max=100></progress>
                        <div class="step-item">
                            <button @click="activeItem = 1" class="step-button text-center" type="button"
                                data-toggle="collapse" data-target="#collapseOne" aria-expanded="true"
                                aria-controls="collapseOne">
                                <i style="font-size: 2.0rem;" class="material-icons" aria-hidden="true">home</i>
                            </button>
                            <div class="step-title">
                                Listing details
                            </div>
                        </div>
                        <div class="step-item">
                            <button @click="activeItem = 2" class="step-button text-center collapsed" type="button"
                                data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false"
                                aria-controls="collapseTwo">
                                <i style="font-size: 2.0rem;" class="material-icons" aria-hidden="true">border_color</i>
                            </button>
                            <div class="step-title">
                                Additional features
                            </div>
                        </div>
                        <div class="step-item">
                            <button @click="activeItem = 3" class="step-button text-center collapsed" type="button"
                                data-toggle="collapse" data-target="#collapseThree" aria-expanded="false"
                                aria-controls="collapseThree">
                                <i style="font-size: 2.0rem;" class="material-icons" aria-hidden="true">home</i>
                            </button>
                            <div class="step-title">
                                Description and photos
                            </div>
                        </div>
                    </div>
                    <div style="background: #e3e9e23d; margin-bottom: 70px;">
                        <div v-if="activeItem === 1">
                            <PropertyInfo />
                            <Abibility />
                        </div>
                        <div v-if="activeItem === 2">
                            <AddintionalFeature />
                        </div>
                        <div v-if="activeItem === 3">
                            <DescriptionMedia />
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </div>

    <!-- <DefaultFooter /> -->
</template>

<style>
:root {
    --prm-color: #417b4e;
    --prm-gray: #e9f0eb;
}

/*  unnecessary */
section {
    width: 100%;
    margin-top: 100px;
}

/*  unnecessary finished*/

/* CSS */
.steps {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;
    position: relative;
}

.step-button {
    width: 45px;
    height: 45px;
    border-radius: 50%;
    border: none;
    background-color: var(--prm-gray);
    transition: .4s;
}

.step-button[aria-expanded="true"] {
    width: 45px;
    height: 45px;
    background-color: var(--prm-color);
    color: #fff;
}

.done {
    background-color: var(--prm-color);
    color: #fff;
}

.step-item {
    z-index: 10;
    text-align: center;
    margin-left: -10px;
    margin-right: -54px;
}

#progress {
    -webkit-appearance: none;
    position: absolute;
    width: 95%;
    z-index: 5;
    height: 5px;
    margin-left: 18px;
    margin-bottom: 18px;
}

/* to customize progress bar */
#progress::-webkit-progress-value {
    background-color: var(--prm-color);
    transition: .5s ease;
}

#progress::-webkit-progress-bar {
    background-color: var(--prm-gray);

}
</style>
