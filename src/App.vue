<template>
  <div>
    <main v-if="!changeView" id="default">
      <img src="./assets/question.png" alt="" />
      <button @click="changeView = false">Start Game</button>
    </main>
    <main v-if="changeView">
      <h1>Quiz Sounds</h1>
      <div id="container">
        <strong>Question ({{ length }})</strong>
        <p>Who is this person or movie?</p>
        <b>Answer: {{ answer }}</b>

        <section>
          <p>Next Sounds</p>
          <div id="elements">
            <div v-if="check1" @click="answer = 'Darek y Josh'">
              <img src=./assets/img/drackandjosh.png alt="draick" />
              <ul>
                <li>Sound #1</li>
                <li>Answer: Darek y Josh</li>
                <li>
                  <audio controls >
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
                @change="check1 = !check1"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check2" @click="answer = 'Bob esponja'">
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
                @change="check2 = !check2"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check3" @click="answer = 'Tortugas de nemo (Squirt)'">
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
                @change="check3 = !check3"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check4">
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
                @change="check4 = !check4"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check5">
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
                @change="check5 = !check5"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check6">
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
                @change="check6 = !check6"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check7">
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
                @change="check7 = !check7"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check8">
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
                @change="check8 = !check8"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check9">
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
                @change="check9 = !check9"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check10">
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
                @change="check10 = !check10"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check11">
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
                @change="check11 = !check11"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check12">
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
                @change="check12 = !check12"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check13">
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
                @change="check13 = !check13"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check14">
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
                @change="check14 = !check14"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check15">
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
                @change="check15 = !check15"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check16">
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
                @change="check16 = !check16"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check17">
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
                @change="check17 = !check17"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check18">
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
                @change="check18 = !check18"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check19">
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
                @change="check19 = !check19"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check20">
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
                @change="check20 = !check20"
              />
            </div>

            <!-- Aqui empieza otro-->
            <div v-if="check21">
              <img src="./assets/img/perikles y merlina.jpg" alt="draick" />
              <ul>
                <li>Sound #22</li>
                <li>Answer: Merlina y Perikles</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/locos adams.mp4"
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
                @change="check21 = !check21"
              />
            </div>
            <!-- Aqui empieza otro-->

            <div v-if="check22">
              <img src="./assets/img/wasaaaa.jpg" alt="draick" />
              <ul>
                <li>Sound #23</li>
                <li>Answer: Scary Movie</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/scarymovie.mp4"
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
                @change="check22 = !check22"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check23">
              <img src="./assets/img/merlina.png" alt="draick" />
              <ul>
                <li>Sound #24</li>
                <li>Answer: Merlina</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/merlina.mp4"
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
                @change="check23 = !check23"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check24">
              <img src="./assets/img/oogie boogie2.jpg" alt="draick" />
              <ul>
                <li>Sound #25</li>
                <li>Answer: El extraño mundo de Jack (Oogie bugi)</li>
                <li>
                  <audio controls>
                    <source src="./assets/music/oogie.mp4" type="audio/mpeg" />
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
                @change="check24 = !check24"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check25">
              <img src="./assets/img/coco.jpeg" alt="draick" />
              <ul>
                <li>Sound #26</li>
                <li>Answer: Coco</li>
                <li>
                  <audio controls>
                    <source src="./assets/music/coco.mp4" type="audio/mpeg" />
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
                @change="check25 = !check25"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check26">
              <img src="./assets/img/abracadabra.jpeg" alt="draick" />
              <ul>
                <li>Sound #27</li>
                <li>Answer: Okus pocus (abacadraba)</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/abacadraba.mp4"
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
                @change="check26 = !check26"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check27">
              <img src="./assets/img/cadaverdelanovia.jpg" alt="draick" />
              <ul>
                <li>Sound #28</li>
                <li>Answer: El cadaver de la novia</li>
                <li>
                  <audio controls>
                    <source
                      src="./assets/music/cadaverdelanovia.mp4"
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
                @change="check27 = !check27"
              />
            </div>
            <!-- Aqui empieza otro-->
            <div v-if="check28">
              <img src="./assets/img/chucky.jpg" alt="draick" />
              <ul>
                <li>Sound #29</li>
                <li>Answer: Chucky</li>
                <li>
                  <audio controls>
                    <source src="./assets/music/chuky.mp4" type="audio/mpeg" />
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
                @change="check28 = !check28"
              />
            </div>
          </div>

          <span>
            <div id="audio-content">
              <div id="rep">
                <img src="./assets/question.png" alt="text" />
                <ul>
                  <li>Sound #1</li>
                  <li>Answer: Try to get a lot of corrects answers</li>
                </ul>
              </div>
              <audio controls>
                <source src="./assets/music/background.mp4" type="audio/mpeg" />
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
      answer: "",
      test: false,
      check21: true,
      check22: true,
      check23: true,
      check24: true,
      check25: true,
      check26: true,
      check27: true,
      check28: true,
      check1: true,
      check2: true,
      check3: true,
      check4: true,
      check5: true,
      check6: true,
      check7: true,
      check8: true,
      check9: true,
      check10: true,
      check11: true,
      check12: true,
      check13: true,
      check14: true,
      check15: true,
      check16: true,
      check17: true,
      check18: true,
      check19: true,
      check20: true,
      length: 0,
      changeView: true,
      music: [
        {
          audio: "draikyjosh.mp4",
          respuesta: "Drack and Josh",
          img: "./assets/img/chucky.jpg",
        },
      ],
    };
  },
  mounted() {
    let d = document.querySelectorAll('input[type="checkbox"]');
    this.length = d.length;
  },
};
</script>

<style scoped>
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
  height: 60vh;
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
  width: 100%;
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
