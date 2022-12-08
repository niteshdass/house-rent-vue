<script setup>
import { onMounted, onUnmounted } from "vue";

//example components
import NavbarDefault from "../..//examples/navbars/NavbarDefault.vue";
import Header from "../../examples/Header.vue";
import Location from '@/views/Presentation/Location.vue';
import Contact from '@/views/Presentation/Contact.vue';
import LightBox from '@/views/Presentation/LightBox.vue';


//images
import vueMkHeader from "@/assets/img/slide1.jpg";
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

  <Header>
    <div class="page-header min-vh-75" :style="`background-image: url(${vueMkHeader})`" loading="lazy">
      <div class="container">
        <div class="row">
          <div class="col-lg-7 text-center mx-auto position-relative">
          </div>
        </div>
      </div>
    </div>
  </Header>

  <LightBox />
  <div class="container pt-4">
    <div class="row border-bottom">
      <div class="col-md-9">
        <div class="row">
          <div class="col-md-4 font">
            <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
              <i style="font-size: 1.4rem; margin-right: 2px;" class="material-icons" aria-hidden="true">home</i>
              <span>Detached house</span>
            </p>
            <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
              <i style="font-size: 1.4rem;margin-right: 2px;" class="material-icons"
                aria-hidden="true">calendar_month</i>
              <span>Abailable form: 11/12/2022</span>
            </p>
            <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
              <i style="font-size: 1.4rem;margin-right: 2px;" class="material-icons" aria-hidden="true">credit_card</i>
              <span>Price: 150000 tk</span>
            </p>
          </div>
          <div class="col-md-3 mt-3 font">
            <p style="font-size: 22px; margin: 0; font-weight: 600;">Total space</p>
            <span style="display: flex">
              <h4>56</h4>
              <h6>M</h6><sub>2</sub>
            </span>
          </div>
          <div class="col-md-3 mt-3 font">
            <p style="font-size: 22px; margin: 0; font-weight: 600;">Bedrooms</p>
            <span style="display: flex">
              <h4>56</h4>
            </span>
          </div>
          <div class="col-md-2 mt-3 font">
            <p style="font-size: 22px; margin: 0; font-weight: 600;">Gas</p>
            <span style="display: flex">
              <h4>Cylinder</h4>
            </span>
          </div>
        </div>
        <div>
          <h5>About</h5>
          <p style="font-weight: 400;">
            Velkommen til Pilestredet Park 19! Fra boligen er det kort vei til et yrende kafe- og uteliv, restauranter, samt et mangfold av spennende forretninger og sjarmerende butikker. Det er også flere flotte parkområder i nærheten som St. Hanshaugen park og Slottsparken for tur- og rekreasjon hele året. Leiligheten ligger i gangavstand til flere utdanningsinstitusjoner som Juridisk fakultet på St. Olavs plass, Høgskolesenteret på Bislett, Høyskolen i Oslo, Tannlegehøgskolen, Veterinærinstituttet samt en kort busstur unna Handelshøyskolen BI og Blindern m.fl. Pilestredet Park har nærhet til et godt utvalg av daglige servicetilbud. Det er et stort utvalg matbutikker i nærheten, hvorav flere er søndagsåpne.
          </p>
        </div>
        <h5>Rooms and inventory</h5>
        <div class="row" style="align-items: center; margin-bottom: 20px;">
          <div class="col-md-2 box-inventory">
            <i style="font-size: 2.4rem;" class="material-icons" aria-hidden="true">bed</i>
            <p style="font-weight: 500;">Bedroom 2</p>
          </div>
          <div class="col-md-2 box-inventory">
            <i style="font-size: 2.4rem;" class="material-icons" aria-hidden="true">bathroom</i>
            <p style="font-weight: 500;">Bathroom 4</p>
          </div>
          <div class="col-md-2 box-inventory">
            <i style="font-size: 2.4rem;" class="material-icons" aria-hidden="true">chair</i>
            <p style="font-weight: 500;">Living room 1</p>
          </div>
          <div class="col-md-2 box-inventory">
            <i style="font-size: 2.4rem;" class="material-icons" aria-hidden="true">local_cafe</i>
            <p style="font-weight: 500;">Kitchen 1</p>
          </div>
        </div>
        <h5>Included in rent</h5>
        <div class="row">
          <div class="col-md-2 badge-item">
            <p style="font-weight: 500;">Cleaning</p>
          </div>
          <div class="col-md-2 badge-item">
            <p style="font-weight: 500;">Cleaning</p>
          </div>
          <div class="col-md-2 badge-item">
            <p style="font-weight: 500;">Cleaning</p>
          </div>
          <div class="col-md-2 badge-item">
            <p style="font-weight: 500;">Cleaning</p>
          </div>
          <div class="col-md-2 badge-item">
            <p style="font-weight: 500;">Cleaning</p>
          </div>
        </div>
        <h5 style="margin-top: 20px">Facilities</h5>
        <div class="row">
            <div class="col-md-4">
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Balcony</span>
                </p>
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Fireplace</span>
                </p>
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Fireplace</span>
                </p>
            </div>
            <div class="col-md-4">
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Broadband Internet</span>
                </p>
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Furnished</span>
                </p>
            </div>
            <div class="col-md-4">
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Elevator</span>
                </p>
                <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
                  <i class="material-icons round-icon" aria-hidden="true">done</i>
                  <span>Modern</span>
                </p>
            </div>
        </div>
      </div>
      <div class="col-md-3 mt-3 font">
        <Contact />
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
            <button
              style="width: 100%"
              class="btn btn-success"
              data-bs-toggle="modal"
              data-bs-target="#exampleModal"
            >Message</button>
            <button style="width: 100%" class="btn btn-dark">Interest</button>
          </div>
        </div>
      </div>
    </div>
    <div>
      <h5 class="pt-6">Location</h5>
      <p class="text-align" style="display:flex; align-items: center; font-weight: 500;">
          <i style="font-size: 1.4rem;" class="material-icons" aria-hidden="true">location_on</i>
          <span>Lamabazar sylhet</span>
      </p>
      <Location />
    </div>
  </div>
  <div style="padding-bottom: 100px;">
  </div>
</template>

<style>
.round-icon {
  font-size: 1.4rem; margin-right: 2px; border-radius: 50%; background-color: white;
  color: green; padding: 2px;
}
.avatar {
  border: 0.3rem solid rgba(#fff, 0.3);
  margin-top: -12rem;
  margin-bottom: 1rem;
  width: 13rem !important;
  height: 13rem !important;
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
