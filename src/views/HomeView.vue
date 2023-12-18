<template>
  <!-- Header-Section-Start -->
  <Header />
  <!-- Header-Section-Finish -->

  <!-- Main-Section-Start -->
  <main>
    <div class="container">
      <div class="row">
        <div class="main_text">
          <h2>About Us</h2>
        </div>
        <div class="main_info">
          <h3>We champion <br> the bold to achieve the extraordinary</h3>
          <div class="main_info_details">
            <p class="main_p">We put aside ego and be in our client’s sides to create the design that will perfectly fits
              in all aspects
              of our clients.</p>
            <div class="main_info_detail">
              <p>120<sup>%</sup></p>
              <p>of recurring business value under management</p>
            </div>
            <div class="main_info_detail">
              <p>350<sup>+</sup></p>
              <p>technology-transformation leaders using Business</p>
            </div>
            <div class="main_info_detail">
              <p><sup>$</sup>2 bn</p>
              <p>of IT investment under management</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
  <!-- Main-Section-Finish -->

  <!-- Article-Section-Start -->
  <article>
    <img class="round" src="../images/arc.png" alt="round">
    <img class="back" src="../images/Img.jpg" alt="round">
    <div class="offer">
      <div class="container">
        <h2>What We Offer</h2>
        <h1>We provide brilliant ideas & adding success to your business</h1>
        <div class="article_details">
          <p>Enable employees to quickly, proactively, and transparently meet and exceed expectations.</p>
          <router-link to="#">All Services</router-link>
        </div>
      </div>
    </div>
    <div class="article_lists">
      <div class="container">
        <div class="list">
          <ul>
            <li><sup>01</sup> Consulting</li>
            <li><sup>02</sup> Digital Business Models</li>
            <li><sup>03</sup> Enterprise Customer Experience</li>
            <li><sup>04</sup> Audit & Assurance</li>
          </ul>
        </div>
        <div class="list">
          <ul>
            <li><sup>05</sup> Bonds & Commodities</li>
            <li><sup>06</sup> Trades & Stocks</li>
            <li><sup>07</sup> Business Opportunities</li>
            <li><sup>08</sup> Strategic Planning</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="brands">
      <div class="container">
        <div class="logos">
          <img src="../images/logo Apple.png" alt="logo">
          <img src="../images/logo Disney.png" alt="logo">
          <img src="../images/logo Google.png" alt="logo">
          <img src="../images/logo Meta.png" alt="logo">
          <img src="../images/logo Nike.png" alt="logo">
        </div>
      </div>
    </div>
  </article>
  <!-- Article-Section-Finish -->

  <!-- Footer-Start -->
  <Footer />
  <!-- Footer-Finish -->
</template>

<script setup>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'


</script>

<style lang="scss" scoped>
// ==== Main-Start ====
main {
  background: #0E163D;
  padding: 140px 0 177px;

  .container {
    width: 100%;
    max-width: 1170px;
    margin: auto;
    padding: 0 12px;

    .row {
      width: 100%;
      display: flex;
      flex-wrap: wrap;
      // gap: 121px;
      margin: 0 -15px;

      .main_text {
        width: 20%;

        h2 {
          color: #A6876A;
          font-size: 16px;
          font-style: normal;
          font-weight: 700;
          line-height: 22px;
          text-transform: uppercase;
          margin-top: 20px;
        }
      }

      .main_info {
        width: 80%;

        h3 {
          max-width: 770px;
          width: fit-content;
          color: #FFF;
          font-size: 78px;
          font-style: normal;
          font-weight: 700;
          line-height: 84px;
          letter-spacing: -2.73px;
          margin-bottom: 60px;
        }

        .main_info_details {
          width: 100%;
          display: flex;


          .main_p {
            color: #FFF;
            font-family: DM Sans;
            font-size: 24px;
            font-style: normal;
            font-weight: 700;
            line-height: 30px;
            letter-spacing: -0.24px;
            max-width: 320px;
            width: fit-content;
            margin-right: 80px;
          }

          .main_info_detail {
            max-width: 170px;
            width: fit-content;
            margin-right: 30px;

            p:nth-child(1) {
              position: relative;
              color: #A6876A;
              font-family: DM Sans;
              font-size: 48px;
              font-style: normal;
              font-weight: 700;
              line-height: 54px;
              letter-spacing: -1.2px;
              margin-bottom: 26px;

              sup {
                color: #FFF;
                font-family: DM Sans;
                font-size: 24px;
                font-style: normal;
                font-weight: 700;
                line-height: 30px;
                letter-spacing: -0.24px;
                margin-left: 6px;
                margin-right: 6px;
              }

            }

            p:nth-child(2) {
              color: #BFD4E4;
              font-family: Merriweather;
              font-size: 14px;
              font-style: normal;
              font-weight: 400;
              line-height: 24px;
              max-width: 170px;
              width: fit-content;
            }
          }

          .main_info_detail:last-child {
            margin-right: 0;
          }
        }
      }
    }
  }
}

@media(max-width:376px) {
  main {
    .container {
      .row {
        padding-inline: 30px;
        display: flex;
        flex-direction: column;
        width: 100%;
      }
    }

    .main_info,
    .main_text {
      width: 100%;
    }

    .main_info {

      .main_info_details {
        display: flex;
        flex-direction: column;
      }
    }
  }


}

// ==== Main-Finish ====

// ==== Article-Start ====
article {
  position: relative;

  .back {
    position: absolute;
    right: 0;
    top: 0;
    z-index: 10;
  }

  .round {
    position: absolute;
    z-index: 20;
    right: 23%;
    top: 50%;
    animation: round ease 400s infinite;
  }

  @keyframes round {
    0% {
      transform: rotateZ(0deg)deg;
    }

    50% {
      transform: rotateZ(3600deg);
    }

    100% {
      transform: rotateZ(0deg);
    }
  }

  .offer {
    padding: 133px 0 43px;

    .container {
      width: 100%;
      max-width: 1170px;
      padding: 0 12px;
      margin: auto;

      h2 {
        color: #A6876A;
        font-size: 16px;
        font-style: normal;
        font-weight: 700;
        line-height: 22px;
        text-transform: uppercase;
        margin-bottom: 30px;
      }

      h1 {
        color: #0E163D;
        font-family: DM Sans;
        font-size: 48px;
        font-style: normal;
        font-weight: 700;
        line-height: 54px;
        letter-spacing: -1.2px;
        width: fit-content;
        max-width: 870px;
        margin-bottom: 50px;
      }

      .article_details {
        display: flex;
        gap: 30px;
        align-items: center;

        p {
          width: fit-content;
          max-width: 670px;
          color: #878995;
          font-size: 18px;
          font-style: normal;
          font-weight: 400;
          line-height: 30px;
        }

        a {
          border: 2px solid #A6876A;
          padding: 14px 15px;
          text-decoration: none;
          color: #0E163D;
          text-align: center;
          font-size: 16px;
          font-style: normal;
          font-weight: 700;
          line-height: 22px;
        }
      }
    }
  }

  .article_lists {
    padding: 70px 0 67px;
    background: #F2F7F9;

    .container {
      width: 100%;
      max-width: 1170px;
      margin: auto;
      padding: 0 12px;
      display: flex;
      gap: 70px;

      .list {
        ul {
          list-style: none;

          li {
            color: #0E163D;
            font-size: 24px;
            font-style: normal;
            font-weight: 700;
            line-height: 40px;
            letter-spacing: -0.24px;
            margin-bottom: 40px;

            sup {
              max-width: 30px;
              color: #A6876A;
              font-size: 12px;
              font-style: normal;
              font-weight: 500;
              line-height: 16px;
            }
          }

          li:last-child() {
            margin-bottom: 0;
          }
        }
      }
    }
  }

  .brands {
    padding: 99px 0 98px;

    .container {
      width: 100%;
      max-width: 1170px;
      margin: auto;
      padding: 0 12px;

      .logos {
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
    }
  }
}

@media(max-width:376px) {
  article {
    padding-inline: 30px;

    .round,
    .back {
      display: none;
    }

    .offer {
      .article_details {
        display: flex;
        flex-direction: column;
      }
    }

    .article_lists {
      .container{
        display: flex;
      flex-direction: column;
      }
    }
    .brands .container .logos{
      display: flex;
      gap: 50px;
      align-items: center;
      animation: brandsImage ease 100s infinite;
    }

    @keyframes brandsImage {
      0%{
        transform: translateX(0);
      }
      25%{
        transform: translateX(-600px);
      }
      50%{
        transform: translateX(0);
      }
      75%{
        transform: translateX(600px);
      }
      100%{
        transform: translateX(0);
      }
    }
  }
}</style>