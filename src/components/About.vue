<template>
   <div class="tokyo_tm_about">
      <div class="about_image">
         <img src="../assets/img/slider/1.jpg" alt="about" />
      </div>
      <!-- End .about_image -->

      <div class="description">
         <h3 class="name">Moses Wescombe</h3>
         <div class="description_inner">
            <div class="left">
               <p>
                  Hi! I am a passionate Software Engineer striving to design
                  simple code, for simple solutions, to difficult problems. In
                  my spare time I love to get out on my motorbike, go
                  bouldering, snowboarding or hiking. On a slow day I prefer to
                  spend my time learning new skills.
               </p>
               <div class="tokyo_tm_button">
                  <button class="ib-button" @click="showModal">
                     My Skills
                  </button>
               </div>
            </div>
            <!-- End .left -->

            <div class="right">
               <ul>
                  <li>
                     <p><span>Birthday:</span>16.11.2001</p>
                  </li>
                  <li>
                     <p><span>Age:</span>19</p>
                  </li>
                  <li>
                     <p><span>Location:</span>Christchurch, New Zealand</p>
                  </li>
                  <li>
                     <p>
                        <span>Email:</span
                        ><a href="mailto:moseswescombe@gmail.com"
                           >moseswescombe@gmail.com</a
                        >
                     </p>
                  </li>
                  <li>
                     <p>
                        <span>Phone:</span
                        ><a href="tel:+64210376223">021 037 6223</a>
                     </p>
                  </li>
                  <li>
                     <p><span>Study:</span>The University of Canterbury</p>
                  </li>
               </ul>
               <!-- End ul -->
            </div>
            <!-- End .right -->
         </div>
      </div>

      <!-- Start Modalbox -->
      <transition name="fade">
         <!-- Modal -->
         <div
            :class="{ 'modal-mask': isActive }"
            id="modal"
            @click="closeModal"
            v-if="isVisible"
         >
            <div
               class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-user"
               @click.stop
            >
               <div class="modal-content">
                  <div class="tokyo_tm_modalbox_about">
                     <div class="close" @click="closeModal">
                        <img
                           class="svg"
                           src="../assets/img/svg/cancel.svg"
                           alt="cancel-img"
                        />
                     </div>
                     <!-- End .close -->
                     <div class="my_box">
                        <div class="left">
                           <div class="about_title">
                              <h3>Tools</h3>
                           </div>
                           <!-- End .abut_title -->
                           <div class="tokyo_progress">
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">Vue.js</span
                                    ><span class="number">80%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:80%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <!-- End progress_inner -->
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">MySQL</span
                                    ><span class="number">70%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:70%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <!-- End progress_inner -->
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">AWS</span
                                    ><span class="number">50%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:50%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">WAMP</span
                                    ><span class="number">50%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:50%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">GitLab CI/CD</span
                                    ><span class="number">40%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:40%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">Maven</span
                                    ><span class="number">50%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:50%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <!-- End progress_inner -->
                           </div>
                           <!-- End .tokyo_progress -->
                        </div>
                        <!-- End .left -->
                        <div class="right">
                           <div class="about_title">
                              <h3>Languages</h3>
                           </div>
                           <div class="tokyo_progress">
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">C/C++</span
                                    ><span class="number">80%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:80%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">Python</span
                                    ><span class="number">90%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:90%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">Java</span
                                    ><span class="number">90%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:90%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">PHP</span
                                    ><span class="number">90%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:90%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">SQL</span
                                    ><span class="number">80%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:80%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">HTML</span
                                    ><span class="number">90%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:90%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">JavaScript</span
                                    ><span class="number">70%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:70%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">CSS</span
                                    ><span class="number">60%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:60%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                              <div class="progress_inner">
                                 <span
                                    ><span class="label">Matlab</span
                                    ><span class="number">70%</span></span
                                 >
                                 <div class="background">
                                    <div class="bar">
                                       <div
                                          class="bar_in"
                                          style="width:70%"
                                       ></div>
                                    </div>
                                 </div>
                              </div>
                           </div>
                        </div>
                        <!-- End .right -->
                     </div>
                  </div>
                  <!-- End .tokyo_tm_modalbox_about -->
               </div>
            </div>
         </div>
      </transition>
      <!-- End Modalbox -->
   </div>
</template>

<script>
//import Brand from './Brand';
export default {
   components: {},
   data() {
      return {
         isActive: false,
         isVisible: false,
      };
   },
   methods: {
      showModal: function() {
         this.isActive = true;
         this.isVisible = true;
      },
      closeModal: function() {
         this.isActive = false;
         this.isVisible = false;
      },
   },
};
</script>

<style lang="scss"></style>
