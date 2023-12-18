<template>
       <div id="footerCarousel" class="carousel slide">
              <div class="boxes">
                     <div class="item active" data-bs-target="#footerCarousel" data-bs-slide-to="0" aria-current="true"
                            aria-label="Slide 1">
                            <h3>Sales blueprint puts Company's growth back on track</h3>
                            <p>We build machines that set the industry standard for precision and durability.</p>
                            <div class="information">
                                   <span>-></span>
                                   <span>Learn more -></span>
                            </div>
                     </div>
                     <div class="item " data-bs-target="#footerCarousel" data-bs-slide-to="1" aria-current="true"
                            aria-label="Slide 2">
                            <h3>Sales blueprint puts Company's growth back on track</h3>
                            <p>We build machines that set the industry standard for precision and durability.</p>
                            <div class="information">
                                   <span>-></span>
                                   <span>Learn more -></span>
                            </div>
                     </div>
                     <div class="item " data-bs-target="#footerCarousel" data-bs-slide-to="2" aria-current="true"
                            aria-label="Slide 3">
                            <h3>Sales blueprint puts Company's growth back on track</h3>
                            <p>We build machines that set the industry standard for precision and durability.</p>
                            <div class="information">
                                   <span>-></span>
                                   <span>Learn more -></span>
                            </div>
                     </div>
                     <div class="item " data-bs-target="#footerCarousel" data-bs-slide-to="3" aria-current="true"
                            aria-label="Slide 4">
                            <h3>Sales blueprint puts Company's growth back on track</h3>
                            <p>We build machines that set the industry standard for precision and durability.</p>
                            <div class="information">
                                   <span>-></span>
                                   <span>Learn more -></span>
                            </div>
                     </div>
                     <div class="item " data-bs-target="#footerCarousel" data-bs-slide-to="4" aria-current="true"
                            aria-label="Slide 5">
                            <h3>Sales blueprint puts Company's growth back on track</h3>
                            <p>We build machines that set the industry standard for precision and durability.</p>
                            <div class="information">
                                   <span>-></span>
                                   <span>Learn more -></span>
                            </div>
                     </div>
              </div>
              <div class="carousel-inner">
                     <div class="carousel-item active">
                            <img src="../images/portrait_4.jpg" alt="img">
                     </div>
                     <div class="carousel-item">
                            <img src="../images/portrait_1.jpg" alt="img">
                     </div>
                     <div class="carousel-item">
                            <img src="../images/portrait_2.jpg" alt="img">
                     </div>
                     <div class="carousel-item">
                            <img src="../images/portrait_3.jpg" alt="img">
                     </div>
                     <div class="carousel-item">
                            <img src="../images/portrait.jpg" alt="img">
                     </div>
              </div>
       </div>
</template>

<script setup>


</script>

<style lang="scss" scoped>
.carousel {
       overflow: hidden;
       .boxes {
              width: 100%;
              display: grid;
              grid-template-columns: repeat(5, 1fr);
              min-height: 780px;
              position: absolute;
              z-index: 50;

              .item {
                     padding: 40px;
                     border-right: 1px solid rgba(255, 255, 255, 0.25);
                     display: flex;
                     gap: 20px;
                     flex-direction: column;
                     justify-content: end;
                     transition: 500ms;
                     position: relative;

                     h3 {
                            color: #FFF;
                            font-size: 24px;
                            font-style: normal;
                            font-weight: 700;
                            line-height: 30px;
                            letter-spacing: -0.24px;
                            position: absolute;
                            display: block;
                            bottom: 85px;
                            transition: 500ms;
                     }

                     p {
                            color: #FFF;
                            font-size: 18px;
                            font-style: normal;
                            font-weight: 400;
                            line-height: 30px;
                            position: absolute;
                            bottom: 55px;
                            display: none;
                     }

                     &:hover {
                            background: rgba(0, 0, 0, 0.20);
                     }

                     &:hover h3 {
                            bottom: 165px;
                     }

                     &:hover p {
                            display: block;
                     }

                     .information {
                            position: relative;

                            span {
                                   color: #A6876A;
                                   font-size: 16px;
                                   font-style: normal;
                                   font-weight: 700;
                                   line-height: 22px;
                                   transition: 500ms;

                                   &:nth-child(2) {
                                          position: absolute;
                                          display: none;
                                   }

                            }

                     }

                     &:hover .information span:nth-child(2) {
                            display: block;
                     }

                     &:hover .information span:nth-child(1) {
                            display: none;
                     }
              }

              .item:last-child {
                     border-right: none;
              }
       }
}

@media(max-width:376px) {
       .carousel {
              .boxes {
                     display: grid;
                     grid-template-columns: 1fr;
                     grid-template-rows: repeat(5, 1fr);
                     .item {
                            display: flex;
                            flex-direction: column;
                            gap: 20px;
                            padding: 40px;
                            border-right: 1px solid rgba(255, 255, 255, 0.25);
                            h3 {   
                                   bottom: 0;
                                   font-size: 18px;
                                   font-weight: 700;
                                   line-height: 24px;
                                   letter-spacing: -0.005em;
                                   text-align: left;    
                            }

                            p {
                                   display: block;
                                   font-family: Merriweather;
                                   font-size: 16px;
                                   font-weight: 400;
                                   line-height: 26px;
                                   letter-spacing: 0em;
                                   text-align: left;

                            }

                            &:hover h3 {
                                   bottom: 0;
                            }

                            &:hover p {
                                   display: block;
                            }

                            .information {

                                  
                                   &.information span:nth-child(2) {
                                          display: none;
                                   }

                                   &.information span:nth-child(1) {
                                          display: none;
                                   }
                            }

                     }


              }
       }
}
</style>