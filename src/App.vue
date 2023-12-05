<template>
  <div id="app">
    <div class="name-bar">
      <div class="name-text"><h1>Group Giftly</h1></div>
    </div>
    <div class="big-box">
      <div class="lane-spacer"></div>
      <div class="lane">
        <div class="box">
          <div class="box-title">
            <h1>Goals of the Project</h1>
          </div>
          <div class="box-body">
            <p>- Provide a platform for sharing wish lists with other people</p>
            <p>- Provide a secret santa feature</p>
          </div>
        </div>
        <div class="spacing-box"></div>
        <div class="box">
          <div class="box-title">
            <h1>Links to Software</h1>
          </div>
          <div class="box-body">
            <p>Link 1:</p>
          </div>
        </div>
      </div>
      <div class="lane-spacer"></div>
      <div class="lane">
        <div class="box">
          <div class="box-title">
            <h1>Progress Report</h1>
          </div>
          <div class="box-body">
            <p>
              Back-end almost complete, some front-end components are complete.
              No finished views as of yet though. Most endpoints are in place.
            </p>
          </div>
        </div>
        <div class="spacing-box"></div>
        <div class="box">
          <div class="box-title">
            <h1>Links to Websites</h1>
          </div>
          <div class="box-body">
            <p>Link 1:</p>
          </div>
        </div>
      </div>
      <div class="lane-spacer"></div>
      <div class="lane">
        <div class="box-long-team">
          <div class="box-title">
            <h1>The Team</h1>
          </div>
          <div class="box-name">
            <div class="box-name-name">
              <p>Aishwarya Gupta</p>
            </div>
            <div class="box-name-title">
              <p>Group Manager</p>
            </div>
            <img class="profile-pic" :src="require('./Asheproj.jpg')" />
          </div>
          <div class="box-name">
            <div class="box-name-name">
              <p>Kimiya Ata</p>
            </div>
            <div class="box-name-title">
              <p>Responsible for Testing</p>
            </div>
            <img class="profile-pic" :src="require('./Kimproj.png')" />
          </div>
          <div class="box-name">
            <div class="box-name-name">
              <p>Gustav Nolgren</p>
            </div>
            <div class="box-name-title">
              <p>Responsible for Integration</p>
            </div>
            <img class="profile-pic" :src="require('./GNproj.jpg')" />
          </div>
          <div class="box-name">
            <div class="box-name-name">
              <p>Jonas Teglund</p>
            </div>
            <div class="box-name-title">
              <p>Responsible for Backend</p>
            </div>
            <img class="profile-pic" :src="require('./JTproj.png')" />
          </div>
          <div class="box-name">
            <div class="box-name-name">
              <p>Oscar Wadestig</p>
            </div>
            <div class="box-name-title">
              <p>Responsible for UI</p>
            </div>
            <img class="profile-pic" :src="require('./OWproj.jpg')" />
          </div>
        </div>
      </div>
      <div class="lane-spacer"></div>
    </div>
    <div class="bottom-bar"></div>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #1a1d28;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #1a1d28;
}

.name-bar {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 18%;
  text-align: start;
  color: #fca311;
  background-color: #1a1d28;
}

.name-text {
  margin-left: 6.5%;
  font-size: 170%;
  color: #fca311;
}

.bottom-bar {
  position: absolute;
  width: 100%;
  height: 18%;
  top: 82%;
  left: 0;
  text-align: start;
  background-color: #1a1d28;
}

.profile-pic {
  position: relative;
  top: -75%;
  left: 77%;
  width: 15%; /* Set the desired width */
  height: 70%; /* Set the desired height */
  border-radius: 50%; /* Make it round */
  object-fit: cover; /* Maintain aspect ratio */
}

.big-box {
  position: absolute;
  display: flex;
  top: 18%;
  left: 0;
  width: 100%;
  height: 64%;
  background-color: #2d3139;
}

.spacing-box {
  width: 100%;
  height: 10%;
  background-color: #1a1d28;
}

.box {
  text-align: center;
  top: 0;
  left: 0;
  width: 100%;
  height: 40%;
  background-color: #2d3139;
}

.box-long {
  text-align: center;
  width: 100%;
  height: 93%;
  background-color: #2d3139;
}

.box-long-team {
  text-align: center;
  width: 90%;
  height: 93%;
  background-color: #2d3139;
}

.box-long-team-profile-pic {
  text-align: left;
  width: 10%;
  height: 80%;
  background-color: #fff;
}

.box-title {
  top: 0;
  left: 10%;
  text-align: left;
  width: 90%;
  height: 10%;
  margin-top: -2%;
  margin-left: 7%;
  color: #fca311;
  background-color: #2d3139;
}

.box-body {
  text-align: left;
  width: 86%;
  height: 90%;
  margin-top: 7%;
  margin-left: 8%;
  background-color: #2d3139;
  color: #e5e5e5;
  font-size: 120%;
}

.box-name {
  text-align: left;
  width: 100%;
  height: 14%;
  margin-left: 10%;
  font-size: 120%;
}

.box-name-name {
  text-align: left;
  width: 70%;
  height: 50%;
  color: #e5e5e5;
  font-weight: bold;
}

.box-name-title {
  width: 70%;
  height: 50%;
  color: #e5e5e5;
  margin-top: -10%;
}

.lane {
  text-align: center;
  width: 25%;
  height: 100%;
  background-color: #2d3139;
}

.lane-spacer {
  text-align: center;
  width: 6.25%;
  height: 100%;
  background-color: #1a1d28;
}
</style>
