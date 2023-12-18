<template>
   
   <el-container id="header_top_menu" class="container">
      <el-menu :default-active="activeIndex" class="el-menu-demo" style="color:  #414562;
      text-align: right;
      font-size: 16px;
      font-style: normal;
      font-weight: 700;
      line-height: 22px;
      background: transparent;
      margin-bottom: none;
      " mode="horizontal" :ellipsis="false">
         <el-menu-item style="margin-right: 172px;" index="0">
            <img style="width: 169px" src="../images/Logotype Companion.png" alt="Element logo" />
         </el-menu-item>

         <!-- <el-menu-item index="1">Processing Center</el-menu-item> -->
         <el-sub-menu index="1">
            <template #title>Home</template>
            <el-sub-menu style="margin: 15px" index="2-4">
               <template #title>Home</template>
               <el-menu-item style="margin: 15px" index="2-4-1">item one</el-menu-item>
               <el-menu-item style="margin: 15px" index="2-4-2">item two</el-menu-item>
               <el-menu-item style="margin: 15px" index="2-4-3">item three</el-menu-item>
            </el-sub-menu>
         </el-sub-menu>
         <el-sub-menu index="2">
            <template style="margin: 15px" #title>Pages</template>
            <el-menu-item style="margin: 15px" index="2-4-1">About Us</el-menu-item>
            <el-menu-item style="margin: 15px" index="2-4-2">Our Team</el-menu-item>
            <el-sub-menu style="margin: 15px" index="2-4">
               <template #title>Services </template>
               <el-menu-item style="margin: 15px" index="2-4-1">Services Grid</el-menu-item>
               <el-menu-item style="margin: 15px" index="2-4-2">Single Service</el-menu-item>
            </el-sub-menu>
            <el-sub-menu style="margin: 15px" index="2-5">
               <template #title>Cases </template>
               <el-menu-item style="margin: 15px" index="2-4-3">Cases Grid</el-menu-item>
               <el-menu-item style="margin: 15px" index="2-4-4">Single Cases</el-menu-item>
            </el-sub-menu>
            <el-sub-menu style="margin: 15px" index="2-6">
               <template #title>Events </template>
               <el-menu-item style="margin: 15px" index="2-4-1">Events Grid</el-menu-item>
               <el-menu-item style="margin: 15px" index="2-4-2">Single Events</el-menu-item>
            </el-sub-menu>
            <el-menu-item style="margin: 15px" index="2-4-3">Contact Us</el-menu-item>
            <el-menu-item style="margin: 15px" index="2-4-4">Make an Appointment</el-menu-item>
            <el-sub-menu style="margin: 15px" index="2-7">
               <template #title>Meetings </template>
               <el-menu-item style="margin: 15px" index="2-4-4">Meetings Grid</el-menu-item>
               <el-menu-item style="margin: 15px" index="2-4-5">Single Meetings</el-menu-item>
            </el-sub-menu>
            <el-menu-item style="margin: 15px" index="2-4-7">Cost Calculatort</el-menu-item>
            <el-menu-item style="margin: 15px" index="2-4-8">Pricing Plans</el-menu-item>
            <el-menu-item style="margin: 15px" index="2-4-9">FAQ</el-menu-item>
         </el-sub-menu>
         <el-sub-menu index="3">
            <template #title>Blog</template>
            <el-sub-menu style="margin:15px" index="2-4">
               <template #title>Blog</template>
               <el-menu-item style="margin:15px" index="2-4-1">Blog one</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-2">Blog two</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-3">Blog three</el-menu-item>
            </el-sub-menu>
         </el-sub-menu>
         <el-sub-menu index="4">
            <template #title>Shop</template>
            <el-sub-menu style="margin:15px" index="2-4">
               <template #title>Shop</template>
               <el-menu-item style="margin:15px" index="2-4-1">Shop one</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-2">Shop two</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-3">Shop three</el-menu-item>
            </el-sub-menu>
         </el-sub-menu>
         <el-sub-menu index="5">
            <template #title>Elements</template>
            <el-sub-menu style="margin:15px" index="2-4">
               <template #title>Elements</template>
               <el-menu-item style="margin:15px" index="2-4-1">Elements one</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-2">Elements two</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-3">Elements three</el-menu-item>
            </el-sub-menu>
         </el-sub-menu>
         <el-sub-menu index="6">
            <template #title>Suppert</template>
            <el-sub-menu style="margin:15px" index="2-4">
               <template #title>Suppert</template>
               <el-menu-item style="margin:15px" index="2-4-1">Suppert one</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-2">Suppert two</el-menu-item>
               <el-menu-item style="margin:15px" index="2-4-3">Suppert three</el-menu-item>
            </el-sub-menu>
         </el-sub-menu>
      </el-menu>
      <div class="icons">
         <el-icon class="search">
            <Search />
         </el-icon>
         <el-icon class="shopping">
            <ShoppingCart />
         </el-icon>
      </div>
   </el-container>
   <div class="media">
      <nav class="navbar navbar-expand-lg ">
         <div class="container-fluid">
            <img src="../images/Logotype Companion.png" alt="">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
               aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
               <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
               <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                  <li class="nav-item dropdown">
                     <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">
                        Portfolio
                     </a>
                     <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Action</a></li>
                        <li><a class="dropdown-item" href="#">Another action</a></li>
                        <li><a class="dropdown-item" href="#">Something else here</a></li>
                     </ul>
                  </li>
                  <li class="nav-item dropdown">
                     <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">
                        Portfolio
                     </a>
                     <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Action</a></li>
                        <li><a class="dropdown-item" href="#">Another action</a></li>
                        <li><a class="dropdown-item" href="#">Something else here</a></li>
                     </ul>
                  </li>
                  <li class="nav-item dropdown">
                     <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
                        aria-expanded="false">
                        Portfolio
                     </a>
                     <ul class="dropdown-menu">
                        <li><a class="dropdown-item" href="#">Action</a></li>
                        <li><a class="dropdown-item" href="#">Another action</a></li>
                        <li><a class="dropdown-item" href="#">Something else here</a></li>
                     </ul>
                  </li>

               </ul>

            </div>
         </div>
      </nav>
   </div>

   <div class="icons_slider">
      <i class="fa-solid fa-arrow-left " type="button" data-bs-target="#carouselExampleIndicators"
         data-bs-slide="prev"></i>
      <i class="fa-solid fa-arrow-right" type="button" data-bs-target="#carouselExampleIndicators"
         data-bs-slide="next"></i>
   </div>
   
   <div class="slider carousel slide" id="carouselExampleIndicators">
      <div class="slider_top carousel-inner">
         <div class="carousel-item active">
            <img src="../images/slider (1).jpg" alt="img">
            <div class="slider_top_info">
               <div class="container">
                  <p>Helping clients create change</p>
               </div>

            </div>
         </div>
         <div class="carousel-item ">
            <img src="../images/slider (2).jpg" alt="img">
            <div class="slider_top_info">
               <div class="container">
                  <p>The right people for your team</p>
               </div>

            </div>
         </div>
         <div class="carousel-item ">
            <img src="../images/slider (3).jpg" alt="img">
            <div class="slider_top_info">
               <div class="container">
                  <p>Helping clients create change</p>
               </div>
            </div>
         </div>
      </div>
      <div class="slider_bottom">
         <div class="container">
            <div class="slider_bottom_item active" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0"
               aria-current="true" aria-label="Slide 1">
               <h3>Helping clients create change</h3>
               <p>Collaboration once happened while huddled in a conference room.</p>
            </div>
            <div class="slider_bottom_item" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
               aria-current="true" aria-label="Slide 2">
               <h3>The right people for your team</h3>
               <p>With dry-erase markers to unleash ideas onto a whiteboard.</p>
            </div>
            <div class="slider_bottom_item" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
               aria-current="true" aria-label="Slide 3">
               <h3>Helping clients create change</h3>
               <p>Crazy 8 design sprints, dot voting, and journey maps.</p>
            </div>
         </div>
      </div>
   </div>

   <div class="icon">
      <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
         <span class="carousel-control-prev-icon"></span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
         <span class="carousel-control-next-icon"></span>
      </button>
   </div>
  
</template>

<script setup lang="ts">
import { ref } from 'vue'

const activeIndex = ref('1')
const handleSelect = (key: string, keyPath: string[]) => {
   console.log(key, keyPath)
}
</script>

<style lang="scss" scoped>
.flex-grow {
   flex-grow: 1;
}
#header_top_menu{
   position: absolute;
   left: 50%;
   transform: translate(-50%);
   z-index: 5000;
}
.container {
   
   width: 100%;
   max-width: 1170px;
   margin: auto;
   padding-top: 24px;
   background: transparent;

   .el-menu--horizontal.el-menu {
      border-bottom: none;
      background: transparent;
   }

   .el-menu--horizontal.el-menu {
      border-bottom: none;
      color: none;
      background: transparent;
   }

   .el-menu--horizontal>.el-menu-item.is-active {
      border-bottom: 0;
      color: none;
      background: transparent;
   }

   .el-menu--horizontal .el-menu-item:not(.is-disabled):focus,
   .el-menu--horizontal .el-menu-item:not(.is-disabled):hover {
      color: none;
      background: transparent;
   }

   .icons {
      display: flex;
      align-items: center;
      gap: 25px;
      color: #414562;
      font-size: 18px;

      &::before {
         content: '';
         display: block;
         height: 20px;
         width: 1px;
         background: #414562;
         margin-right: 5px;
      }
   }
}
.slider {
   .slider_top {
      .carousel-item {
         img {
            position: absolute;
            z-index: -99999;
            top:0;
            right: 0;
            width: 1345px;
            height: 540px;
            left: 575px;
            object-fit: cover;
         }
      }

      .slider_top_info {
         margin-bottom: 78px;
         display: flex;
         align-items: end;
         position: relative;

         .container {
            display: flex;
            gap: 200px;
            align-items: end;

            p {
               margin-top: 280px;
               color: #0E163D;
               font-size: 96px;
               font-style: normal;
               font-weight: 700;
               line-height: 96px;
               letter-spacing: -4px;
               max-width: 850px;
               width: fit-content;
            }


         }

         
      }
   }

   .slider_bottom {
      .container {
         padding: 89px 0 90px;
         display: flex;
         // justify-content: space-between;
         gap: 90px;

         .slider_bottom_item {
            max-width: 330px;
            width: fit-content;

            &:hover {
               cursor: pointer;
            }

            &.active h3 {
               color: #A6876A;
               border-bottom: 1px solid #A6876A;
            }

            h3 {
               color: #0E163D;
               font-size: 18px;
               font-style: normal;
               font-weight: 700;
               line-height: 24px;
               letter-spacing: -0.09px;
               padding-bottom: 12px;
               border-bottom: 1px solid #BFD4E4;
               margin-bottom: 12px;
            }

            p {
               color: #597393;
               font-size: 16px;
               font-style: normal;
               font-weight: 400;
               line-height: 26px;
            }
         }
      }
   }
}

.icons_slider {
            position: absolute;
            z-index: 99999;
            right: 375px;
            display: flex;
            gap: 10px;
            top: 45%;
            .fa-arrow-left,
            .fa-arrow-right {
               color: #414562;
               padding: 23px;
               background: #fff;
               border-radius: 50%;
               font-size: 24px;
            }
         }
.icon {
   position: fixed;
   z-index: 500;

}

.media {
   display: none;
}

@media (max-width: 576px) {

   .container {
      display: none;
      width: 100px;
   }

   .media {
      display: block;
      padding: 22px 30px;

   }

   .slider_bottom {
      display: none;
   }

   .navbar {
      --bs-navbar-toggler-border-color: none
   }

   .slider {
      .slider_top {
         img {
            

         }
      }
   }

   .slider_top {
      .slider_top_info {
         .icons {
            display: none;
         }

         .container {
            p {
               font-family: DM Sans;
               font-size: 48px;
               font-weight: 700;
               line-height: 54px;
               letter-spacing: -0.0 25em;
               text-align: left;
               width: 315px;
               width: fit-content;
            }
         }
      }
   }
}</style>