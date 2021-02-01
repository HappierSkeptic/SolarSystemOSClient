<template>
  <div>
    <!-- main content -->
    <v-container>
    <div>
      <h1 id="header" color="white">SolarSystemOS</h1>
<br>
      <section class="glass">
        <div class="dashboard">
          <div class="user">
            <img src="../public/images/avatar.png" alt="" />
            <h3>Ian Floyd</h3>
            <p>Admin</p>
          </div>
          <br>
          <div class="links">
          
            <div class="link">
                <v-btn text>
              <img src="../public/images/tools.png" alt="" />
              <h2>Tools</h2>
                 </v-btn>
            </div>
         
            <div class="link">
              <v-btn text>
              <img src="../public/images/upcoming.png" alt="" />
              <h2>Games</h2>
              </v-btn>
            </div>
            <div class="link">
              <v-btn text>
              <img src="../public/images/library.png" alt="" />
              <h2>Library</h2>
              </v-btn>
            </div>
            <div class="link">
              <v-btn text>
              <img src="../public/images/chat.png" alt="" />
              <h2>Chat</h2>
              </v-btn>
            </div>
          </div>
          <!-- <div class="pro">
            <h2>Join pro for free games.</h2>
            <img src="../public/images/controller.png" alt="" />
          </div> -->
        </div>
        <div class="games">
          <div class="cards">
            <div class="card">
              <img src="../public/images/tools.png" alt="" />
              <div class="card-info">
                <h2>File Uploader</h2>
                <p>v1.0.0</p>
                <div class="progress"></div>
              </div>
              <h2 class="percentage"></h2>
            </div>
            <div class="card">
              <img src="../public/images/tools.png" alt="" />
              <div class="card-info">
                <h2>Tool 2</h2>
                <p>v1.0.0</p>
                <div class="progress"></div>
              </div>
              <h2 class="percentage"></h2>
            </div>
            <div class="card">
              <img src="../public/images/tools.png" alt="" />
              <div class="card-info">
                <h2>Tool 3</h2>
                <p>v1.0.0</p>
                <div class="progress"></div>
              </div>
              <h2 class="percentage"></h2>
            </div>
          </div>
        </div>
      </section>
    </div>
    <!-- background gradient -->
    <figure class="fullheight" id="night-day">
      <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="120%">
        <linearGradient id="skyGradient" x1="0%" y1="0%" x2="0%" y2="100%">
          <stop stop-color="rgb(0,0,12)" offset="0%" id="zenith">
            <animate
              attributeName="stop-color"
              dur="240s"
              values="rgba(0,0,12,0);rgba(2,1,17,0);rgba(2,1,17,0);rgba(2,1,17,0);rgba(32,32,44,0.5);rgba(64,64,92,.8);rgb(74,73,105);rgb(117,122,191);rgb(130,173,219);rgb(148,197,248);rgb(183,234,255);rgb(144,223,254);rgb(87,193,235);rgb(45,145,194);rgb(36,115,171);rgb(30,82,142);rgb(30,82,142);rgb(21,66,119);rgba(22,60,82,0.8);rgba(7,27,38,.5);rgba(1,10,16,.3);rgba(9,4,1,0);rgba(0,0,12,0);rgba(0,0,12,0)"
              repeatCount="indefinite"
            />

            <animate
              attributeName="offset"
              dur="240s"
              values="0;.85;.6;.1;0;0;0;0;0;.01;0;0;0;0;0;0;0;0;0;0;.3,.5,.8,0"
              repeatCount="indefinite"
            />
          </stop>

          <stop stop-color="rgb(0,0,12)" offset="100%" id="horizon">
            <animate
              attributeName="stop-color"
              dur="240s"
              values="rgba(0,0,12,0);rgba(25,22,33,.3);rgba(32,32,44,.8);rgb(58,58,82);rgb(81,81,117);rgb(138,118,171);rgb(205,130,160);rgb(234,176,209);rgb(235,178,177);rgb(177,181,234);rgb(148,223,255);rgb(103,209,251);rgb(56,163,209);rgb(36,111,168);rgb(30,82,142);rgb(91,121,131);rgb(157,166,113);rgb(233,206,93);rgb(178,99,57);rgb(47,17,7);rgb(36,14,3);rgb(47,17,7);rgba(75,29,6,.4);rgba(21,8,0,0);rgba(0,0,12,0)"
              repeatCount="indefinite"
            />
          </stop>
        </linearGradient>
        <rect
          id="sky"
          x="0"
          y="0"
          width="100%"
          height="100%"
          style="fill: url(#skyGradient)"
        />
      </svg>

      <!-- <div class="sun"></div>
  <div class="moon"></div> -->
    </figure>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap");

h2,
p {
  color: #658ec6;
  font-weight: 500;
  opacity: 0.8;
}

h3 {
  color: #426696;
  font-weight: 600;
  opacity: 0.8;
}

main {
  font-family: "Poppins", sans-serif;
  height: 100vh;
  background: linear-gradient(to right top, #65dfc9, #6cdbeb);
  display: flex;
  align-items: center;
  justify-content: center;
}

.glass {
  background: white;
  height: 90vh;
  width: 100%;
  background: linear-gradient(
    to right bottom,
    rgba(255, 255, 255, 0.7),
    rgba(255, 255, 255, 0.3)
  );
  border-radius: 2rem;
  z-index: 2;
  backdrop-filter: blur(2rem);
  display: flex;
}
.circle1,
.circle2 {
  background: white;
  background: linear-gradient(
    to right bottom,
    rgba(255, 255, 255, 0.8),
    rgba(255, 255, 255, 0.3)
  );
  height: 20rem;
  width: 20rem;
  position: absolute;
  border-radius: 50%;
}

.circle1 {
  top: 5%;
  right: 15%;
}
.circle2 {
  bottom: 5%;
  left: 10%;
}
.dashboard {
  align-items: center;
  justify-content: space-evenly;
  text-align: center;
  background: linear-gradient(
    to right bottom,
    rgba(255, 255, 255, 0.7),
    rgba(255, 255, 255, 0.3)
  );
  border-radius: 2rem;
}
.link {
  display: flex;
  margin: 2rem 0rem;
  padding: 1rem 5rem;
  align-items: center;
}
.link h2 {
  padding: 0rem 2rem;
}

.games {
  flex: 2;
}

.pro {
  background: linear-gradient(to right top, #65dfc9, #6cdbeb);
  border-radius: 2rem;
  color: white;
  padding: 1rem;
  position: relative;
}

.pro img {
  position: absolute;
  top: -10%;
  right: 10%;
}
.pro h2 {
  width: 40%;
  color: white;
  font-weight: 600;
}

/* GAMES */
.status {
  margin-bottom: 3rem;
}

.status input {
  background: linear-gradient(
    to right bottom,
    rgba(255, 255, 255, 0.7),
    rgba(255, 255, 255, 0.3)
  );
  border: none;
  width: 50%;
  padding: 0.5rem;
  border-radius: 2rem;
}

.games {
  margin: 5rem;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
}

.card {
  display: flex;
  background: linear-gradient(
    to left top,
    rgba(255, 255, 255, 0.8),
    rgba(255, 255, 255, 0.5)
  );
  border-radius: 1rem;
  margin: 2rem 0rem;
  padding: 2rem;
  box-shadow: 6px 6px 20px rgba(122, 122, 122, 0.212);
  justify-content: space-between;
}

.progress {
  background: linear-gradient(to right top, #65dfc9, #6cdbeb);
  width: 100%;
  height: 25%;
  border-radius: 1rem;
  position: relative;
  overflow: hidden;
}
.progress::after {
  content: "";
  width: 100%;
  height: 100%;
  background: rgb(236, 236, 236);
  position: absolute;
  left: 60%;
}
.card-info {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.percentage {
  font-weight: bold;
  background: linear-gradient(to right top, #65dfc9, #6cdbeb);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.user {
  margin-top: 25px;
}
/* other styles */

body {
  margin: 0 !important;
  margin: 0;
  overflow: hidden;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  padding: 0;
  margin: 0;
  overflow: hidden;
}

.daynightcycle {
  background-color: black;
}
.fullheight {
  overflow: hidden;
  height: 100vh;
}
#header {
  font-family: "Press Start 2P", cursive;
  color: white;
}

figure#night-day {
  z-index: -1;
  margin: 0 auto;
  font-size: 0;
  max-width: 100vw;
  height: 110vh;
  min-height: 100vh;
  background-color: #000;
  overflow-y: hidden;
  background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/starfield_stock_1.jpg);
  position: fixed;
  position: fixed;
  bottom: 0;
  right: 0;
  top: 0;
  left: 0;
}
@keyframes suntrack {
  from {
    transform: rotate(0.15turn);
  }
  to {
    transform: rotate(-0.85turn);
  }
}

@keyframes moontrack {
  from {
    transform: rotate(0.15turn);
  }
  to {
    transform: rotate(-0.85turn);
  }
}

@keyframes sunpulse {
  from {
    box-shadow: 0 0 100px rgba(255, 255, 0, 0.4),
      0 0 100px rgba(255, 255, 0, 0.4);
  }
  to {
    box-shadow: 0 0 50px rgba(241, 245, 9, 0.911),
      0 0 75px rgba(255, 255, 0, 0.8);
  }
}

body {
  margin: 0;
  background-color: #000;
  background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/starfield_stock_1.jpg);
  position: relative;
}

.sun {
  width: 15vw;
  height: 15vw;
  background: #ff0;
  background: radial-gradient(ellipse at center, #f90 0%, #fc0 60%, #ff0 100%);
  border-radius: 100%;
  position: absolute;
  bottom: -7vw;
  right: 7vw;
  transform-origin: -28vw 7vw;
  animation: suntrack 24s infinite forwards linear,
    sunpulse 2s alternate infinite;
}

.moon {
  background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/moon8.png);
  width: 15vw;
  height: 15vw;
  position: absolute;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 90% 90%;
  border-radius: 100%;
  bottom: -7vw;
  right: 7vw;
  transform-origin: -28vw 7vw;
  animation: moontrack 24s infinite backwards linear;
  animation-delay: 12s;
  opacity: 0.8;
}
</style>
