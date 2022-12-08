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
  <div class="container py-7">
    <div class="row mt-5">
      <div class="col-sm-3 col-6 mx-auto">

        <!-- Modal -->
        <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
          <div class="modal-dialog">
            <div class="modal-content">
              <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLabel">
                  Your modal title
                </h5>
                <MaterialButton color="none" class="btn-close" data-bs-dismiss="modal" aria-label="Close">
                </MaterialButton>
              </div>
              <div class="modal-body">
                <div class="row">
                  <div class="col-lg-10 mx-auto d-flex justify-content-center flex-column">
                    <!-- <h3 class="text-center">Contact us</h3> -->
                    <form role="form" id="contact-form" method="post" autocomplete="off">
                      <div class="card-body">
                        <h6 for="name">Furnished</h6>
                        <div class="row border-bottom">
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished" >
                              Unfurnished
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Furnished
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Partly Furnished
                            </MaterialCheckbox>
                          </div>
                        </div>
                        <h6 for="name">Area</h6>
                        <div class="row border-bottom">
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished" >
                              Lamabazar
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Subidbazar
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Bagbari
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Modina market
                            </MaterialCheckbox>
                          </div>
                        </div>
                        <h6 for="name">Number of bedrooms</h6>
                        <div class="row border-bottom">
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished" >
                              1
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              2
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              3
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              4
                            </MaterialCheckbox>
                          </div>
                        </div>
                        <h6 for="name">Available from</h6>
                        <div class="row border-bottom">
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="unfurnished" label="Furnished" >
                              January
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              February
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              March
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
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
                            <MaterialCheckbox id="unfurnished" label="Furnished" >
                              Cable TV
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Common Room Cleaning
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Electricity
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Gas
                            </MaterialCheckbox>
                          </div>
                          <div class="form-check col-md-4">
                            <MaterialCheckbox id="furnished" label="Furnished" >
                              Water
                            </MaterialCheckbox>
                          </div>
                        </div>
                      </div>
                      <div class="row">
                        <div class="col-md-12">
                          <!-- <MaterialSwitch class="mb-4 d-flex align-items-center" id="flexSwitchCheckDefault" checked
                            labelClass="ms-3 mb-0">
                            I agree to the
                            <a href="javascript:;" class="text-dark"><u>Terms and Conditions</u></a>.
                          </MaterialSwitch> -->
                        </div>
                      </div>
                    </form>
                  </div>
                </div>
              </div>
              <div class="modal-footer justify-content-between">
                <MaterialButton variant="gradient" color="dark" data-bs-dismiss="modal">
                  Close
                </MaterialButton>
                <MaterialButton variant="gradient" color="success" class="mb-0">
                  Save changes
                </MaterialButton>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
