<template>
  <div>
    <main v-if="!changeView" id="default">
      <img src="./assets/question.png" alt="" />
      <button @click="changeView = false">Start Game</button>
    </main>
    <main v-if="changeView">
      <h1>Quiz Sounds</h1>
      <div id="container">
        <strong>Question</strong>
        <p>Who is this person?</p>
        <b>Answer: Chapulin Colorado</b>

        <section>
          <p>Next Sounds</p>
          <div id="elements">
            <div v-if="checkOne">
              <img src=./assets/img/drackandjosh.png alt="draick" />
              <ul>
                <li>Sound #1</li>
                <li>Answer: Darek y Josh</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/draikyjosh.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/bob y patrick.jpg" alt="draick" />
              <ul>
                <li>Sound #2</li>
                <li>Answer: Bob esponja</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/bob esponja.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download
                      <a href="./assets/music/bob esponja.mp4">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/tortugasdenemo.jpg" alt="draick" />
              <ul>
                <li>Sound #3</li>
                <li>Answer: Tortugas de nemo (Squirt)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/buscando a nemo-tortugas.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download
                      <a href="./assets/music/buscando a nemo-tortugas.mp4"
                        >MP3</a
                      >
                      or <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/donramon.jpg" alt="draick" />
              <ul>
                <li>Sound #4</li>
                <li>Answer: Don Ramon</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/chavo del 8-ramon.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download
                      <a href="./assets/music/chavo del 8-ramon.mp4">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/donde estan las rubias.jpg" alt="draick" />
              <ul>
                <li>Sound #5</li>
                <li>Answer: Marcus y Kevin (Donde estan las rubias)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/donde estan las rubias.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/crud y capitan.jpg" alt="draick" />
              <ul>
                <li>Sound #6</li>
                <li>Answer: Grud y Capitan America (Avengers Endgame)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/grud y capitanamerica.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/gump.jpg" alt="draick" />
              <ul>
                <li>Sound #7</li>
                <li>Answer: Forrest Gump</li>
                <li>
                  <audio controls>
                    <source src="./assets/music/gump.mp4" type="audio/mpeg" />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/ron y hermony.jpg" alt="draick" />
              <ul>
                <li>Sound #8</li>
                <li>Answer: Ron y Hermonie</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/harry potter ron y hermony.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/dombuldor.jpg" alt="draick" />
              <ul>
                <li>Sound #9</li>
                <li>Answer: Dombuldor</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/HarryPotterDombuldor.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/jenji y lord.jpeg" alt="draick" />
              <ul>
                <li>Sound #10</li>
                <li>Answer: Jenjibre y LordFargat (Sherk)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/jenjibre sherk y lord farguat.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/homero y miljaus.jpg" alt="draick" />
              <ul>
                <li>Sound #11</li>
                <li>Answer: Homero y Miljaus</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/los simposon-homero y miljaus.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/tony stark.png" alt="draick" />
              <ul>
                <li>Sound #12</li>
                <li>Answer: Tony Stark (Avengers)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/Los Vengadores-tony.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/lord fargaut.jpg" alt="draick" />
              <ul>
                <li>Sound #13</li>
                <li>Answer: Lord Farguat</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/lord farguat sherk.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/skiper magadascar.jpg" alt="draick" />
              <ul>
                <li>Sound #14</li>
                <li>Answer: Skiper (Madagascar)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/madagascar-skiper.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/mario bross estrella.jpg" alt="draick" />
              <ul>
                <li>Sound #15</li>
                <li>Answer: Lumalee (Mario Bross)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/mariobross- estrella azul.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/monsterinc 1.jpeg" alt="draick" />
              <ul>
                <li>Sound #16</li>
                <li>Answer: Monster Inc</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/monser inc 1.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/burro.jpeg" alt="draick" />
              <ul>
                <li>Sound #17</li>
                <li>Answer: Burro (Sherk)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/sherk burro.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/locutor spider man.jpeg" alt="draick" />
              <ul>
                <li>Sound #18</li>
                <li>Answer: Spiderman</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/spider-man locutor.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img src="./assets/img/thore.jpg" alt="draick" />
              <ul>
                <li>Sound #19</li>
                <li>Answer: Thor</li>
                <li>
                  <audio controls>
                    <source src="./assets/music/thor.mp4" type="audio/mpeg" />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="checkOne">
              <img
                src="./assets/img/monster inc pejelagarto.jpg"
                alt="draick"
              />
              <ul>
                <li>Sound #20</li>
                <li>Answer: Monster Inc.</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/monter inc.mp4"
                      type="audio/mpeg"
                    />
                    <p>
                      Download <a href="myAudio.mp3">MP3</a> or
                      <a href="myAudio.ogg">OGG</a> audio.
                    </p>
                  </audio>
                </li>
              </ul>
              <input
                type="checkbox"
                name=""
                id="check"
                @change="checkOne = !checkOne"
              />
            </div>

            <!-- Aqui empieza otro-->
          </div>
          <!-- 

     
          <span>
            <div id="audio-content">
              <div id="rep">
                <img
                  @click="test = !test"
                  src="./assets/img/drackandjosh.png"
                  alt=""
                />
                <ul>
                  <li>Sound #1</li>
                  <li>Answer: {{ respuesta }}</li>
                </ul>
              </div>
              <audio controls>
                <source src="./assets/music/draikyjosh.mp4" type="audio/mpeg" />
                <p>
                  Download <a href="myAudio.mp3">MP3</a> or
                  <a href="myAudio.ogg">OGG</a> audio.
                </p>
              </audio>
            </div>
          </span>   -->
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
      t: "./assets/img/drackandjosh.png",
      test: false,
      checkOne: true,
      changeView: true,
      music: [
        {
          audio: "draikyjosh.mp4",
          respuesta: "Drack and Josh",
          img: "./assets/logo.png",
        },
      ],
    };
  },
};
</script>

<style scoped>
#check {
}

#default {
  width: 100%;
  height: 100vh;
  background: linear-gradient(
    131deg,
    rgba(136, 170, 255, 1) 0%,
    rgba(6, 9, 205, 1) 100%
  );
}
main {
  padding: 2rem 2rem 0rem 2rem;
  margin: 0rem;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  width: fit-content;
  height: fit-content;
  background: linear-gradient(
    131deg,
    rgba(136, 170, 255, 1) 0%,
    rgba(6, 9, 205, 1) 100%
  );
}
#container {
  background-color: white;
  width: 100%;
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
#audio-content {
  border-radius: 1rem;
  padding: 0.5rem 2rem;
  background: rgba(136, 170, 255, 1);
}
#rep {
  display: flex;
  align-items: center;

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
  align-items: center;
  gap: 0.5rem;
}
#elements div img {
  width: 150px;
  height: auto;
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
  width: 100%;
  /* Ancho personalizado */
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
