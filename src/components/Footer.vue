<template>
       <div class="boxes">
              <div class="item">
                     <h3>Sales blueprint puts Company's growth back on track</h3>
                     <p>We build machines that set the industry standard for precision and durability.</p>
                     <div class="information">
                            <span>-></span>
                            <span>Learn more -></span>
                     </div>
              </div>
              <div class="item">
                     <h3>Sales blueprint puts Company's growth back on track</h3>
                     <p>We build machines that set the industry standard for precision and durability.</p>
                     <div class="information">
                            <span>-></span>
                            <span>Learn more -></span>
                     </div>
              </div>
              <div class="item">
                     <h3>Sales blueprint puts Company's growth back on track</h3>
                     <p>We build machines that set the industry standard for precision and durability.</p>
                     <div class="information">
                            <span>-></span>
                            <span>Learn more -></span>
                     </div>
              </div>
              <div class="item">
                     <h3>Sales blueprint puts Company's growth back on track</h3>
                     <p>We build machines that set the industry standard for precision and durability.</p>
                     <div class="information">
                            <span>-></span>
                            <span>Learn more -></span>
                     </div>
              </div>
              <div class="item">
                     <h3>Sales blueprint puts Company's growth back on track</h3>
                     <p>We build machines that set the industry standard for precision and durability.</p>
                     <div class="information">
                            <span>-></span>
                            <span>Learn more -></span>
                     </div>
              </div>
       </div>
</template>

<script setup lang="ts">
import {ref} from 'vue'


// interface Props {
//        img: string,
//        h3: string,
//        p:string,
      
// }


// const lists = ref<Props[]>([
//        {
//               img: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASMA…1dFpVS4ngmGc+Ypk3igv8v6cx9Hn8Hk4ZAAAAAElFTkSuQmCC',
//               h3:"Sales blueprint puts Company's growth back on track",
//               p:"We build machines that set the industry standard for precision and durability.",
//        },
//        {
//               img: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASMA…1dFpVS4ngmGc+Ypk3igv8v6cx9Hn8Hk4ZAAAAAElFTkSuQmCC',
//               h3:"Sales blueprint puts Company's growth back on track",
//               p:"We build machines that set the industry standard for precision and durability.",
//        },
//        {
//               img: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASMA…1dFpVS4ngmGc+Ypk3igv8v6cx9Hn8Hk4ZAAAAAElFTkSuQmCC',
//               h3:"Sales blueprint puts Company's growth back on track",
//               p:"We build machines that set the industry standard for precision and durability.",
//        },
//        {
//               img: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASMA…1dFpVS4ngmGc+Ypk3igv8v6cx9Hn8Hk4ZAAAAAElFTkSuQmCC',
//               h3:"Sales blueprint puts Company's growth back on track",
//               p:"We build machines that set the industry standard for precision and durability.",
//        },
//        {
//               img: 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASMA…1dFpVS4ngmGc+Ypk3igv8v6cx9Hn8Hk4ZAAAAAElFTkSuQmCC',
//               h3:"Sales blueprint puts Company's growth back on track",
//               p:"We build machines that set the industry standard for precision and durability.",
//        },

// ])

</script>

<style lang="scss" scoped>
.boxes {
       width: 100%;
       display: grid;
       grid-template-columns: repeat(5, 1fr);
       min-height: 780px;
       background: url('../images/portrait_1\ \(1\).png');

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
                     bottom: 85px;
                     display: none;
              }

              &:hover {
                     background: rgba(0, 0, 0, 0.20);
              }
              &:hover h3{
                     bottom: 155px;
              }
              &:hover p{
                     display: block;
              }
              .information {
                     position: relative;
                     
                     span {
                            color:  #A6876A;
                            font-size: 16px;
                            font-style: normal;
                            font-weight: 700;
                            line-height: 22px;
                            transition: 500ms;
                            &:nth-child(2){
                                   position: absolute;
                                   display: none;
                            }
                            
                     }
                     
              }
              &:hover .information span:nth-child(2){
                     display: block;
              }
              &:hover .information span:nth-child(1){
                     display: none;
              }
       }

       .item:last-child {
              border-right: none;
       }
}</style>