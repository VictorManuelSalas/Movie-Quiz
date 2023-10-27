<template>
  <div>
    <main v-if="!changeView">
      <img src="./assets/question.png" alt="" />
      <button @click="changeView = false">Start Game</button>
    </main>
    <main v-if="changeView">
      <h1>Sound #1</h1>
      <div id="container">
        <strong>Question</strong>
        <p>Who is this person?</p>
        <b>Answer: Chapulin Colorado</b>

        <section>
          <p>Next Sounds</p>
          <div id="elements">
            <div>
              <img src="./assets/logo.png" alt="" />
              <ul>
                <li>Sound #1</li>
                <li>Answer: Buscando a nemo</li>
              </ul>
            </div>
            <div>
              <img src="./assets/logo.png" alt="" />
              <ul>
                <li>Sound #1</li>
                <li>Answer: Buscando a nemo</li>
              </ul>
            </div>
            <div>
              <img src="./assets/logo.png" alt="" />
              <ul>
                <li>Sound #1</li>
                <li>Answer: Buscando a nemo</li>
              </ul>
            </div>
          </div>
          <span>
            <div id="rep">
              <img src="./assets/logo.png" alt="" />
              <ul>
                <li>Sound #1</li>
                <li>Answer: Buscando a nemo</li>
              </ul>
              <audio controls>
                <source src="myAudio.mp3" type="audio/mpeg" />
                <p>
                  Download <a href="myAudio.mp3">MP3</a> or
                  <a href="myAudio.ogg">OGG</a> audio.
                </p>
              </audio>
            </div>
          </span>
        </section>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      changeView: true,
    };
  },
};
</script>

<style scoped>
main {
  padding: 0%;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  width: 100vw;
  height: 100vh;
  background: linear-gradient(
    131deg,
    rgba(136, 170, 255, 1) 0%,
    rgba(6, 9, 205, 1) 100%
  );
}
#container {
  background-color: white;
  width: 100vh;
  height: 70%;
  padding: 2rem 2rem;
  font-size: 1.4rem;
  border-radius: 2rem 2rem 0rem 0rem;
}
h1 {
  color: white;
}
strong {
  font-size: 1.7rem;
}
p {
  text-align: center;
}
p:first-child {
  text-align: left;
  color: black;
  font-weight: bolder;
}
b {
  color: blue;
}
section {
  display: flex;
  flex-direction: column;
  gap: 1rem; 
}
#rep {
  position: relative;
  border-radius: 1rem;
  display: flex;
  align-items: center;
  padding: 0.5rem 2rem;
  background: rgba(136, 170, 255, 1);
  color: white;
}
#rep img {
  width: 15%;
  border-radius: 1rem;
  margin: 0%;
}
#elements {
  height: 250px;
  overflow-y: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
#elements div {
  padding: 1rem 1rem;
  display: flex;
  gap: 1rem;
}
#elements div img {
  width: 15%;
  border-radius: 1rem;
  margin: 0%;
}
#elements div ul,
#rep ul {
  list-style: none;
}
#elements div ul li:first-of-type,
#rep ul li:first-of-type {
  font-weight: bolder;
}
audio {
  position: absolute;
  right: 3%;
  width: 20%; /* Ancho personalizado */
  
}
audio::-webkit-media-controls-play-button,
audio::-webkit-media-controls-pause-button,
audio::-webkit-media-controls-mute-button {
   
}
img {
  width: 40%;
  margin: 0rem auto;
}
button {
  border-radius: 1rem;
  width: 80%;
  height: 7%;
  font-size: 2rem;
}
</style>
