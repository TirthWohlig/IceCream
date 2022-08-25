<template>
  <div class="ice-cream">
    <div class="flavour">
      <img
        class="cream"
        id="berry"
        src="./assets/images/berry.png"
        alt="berry"
      />
      <br />
      <img
        class="cream"
        id="blueberry"
        src="./assets/images/blueberry.png"
        alt="blueberry"
      />
      <br />
      <img
        class="cream"
        id="butterscoth"
        src="./assets/images/butterscoth.png"
        alt="butterscoth"
      />
      <br />
      <img
        class="cream"
        id="chocolate"
        src="./assets/images/chocolate.png"
        alt="chocolate"
      />
      <br />
      <img class="cream" id="mint" src="./assets/images/mint.png" alt="mint" />
      <br />
      <img
        class="cream"
        id="peach"
        src="./assets/images/peach.png"
        alt="peach"
      />
      <br />
      <img
        class="cream"
        id="strawberry"
        src="./assets/images/strawberry.png"
        alt="strawberry"
      />
      <br />
      <img
        class="cream"
        id="vanilla"
        src="./assets/images/vanilla.png"
        alt="vanilla"
      />
      <br />
      <img id="cone" src="./assets/images/cone.png" alt="cone" />
    </div>
  </div>

  <form>
    <div class="choice">
      <input
        type="checkbox"
        class="check"
        id="white"
        name="Box"
        @click="cream"
      />
      Vanilla
      <br />
      <br />
      <input type="checkbox" id="pink" name="Box" @click="cream" />
      Strawberry
      <br />
      <br />
      <input
        type="checkbox"
        autocomplete="off"
        id="baby_pink"
        name="Box"
        @click="cream"
      />
      Peach
      <br />
      <br />
      <input type="checkbox" id="green" name="Box" @click="cream" /> Mint
      <br />
      <br />
      <input type="checkbox" id="brown" name="Box" @click="cream" />
      Chocolate
      <br />
      <br />
      <input type="checkbox" id="yellow" name="Box" @click="cream" />
      Butterscoth
      <br />
      <br />
      <input type="checkbox" id="blue" name="Box" @click="cream" />
      Blueberry
      <br />
      <br />
      <input type="checkbox" id="purple" name="Box" @click="cream" /> Berry
    </div>
  </form>
</template>

<script>
export default {
  methods: {
    cream() {
      // Vanilla
      if (document.getElementById("white").checked) {
        document.getElementById("vanilla").style.visibility = "visible";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("vanilla").style.visibility = "hidden";
      }

      // Strawberry
      if (document.getElementById("pink").checked) {
        document.getElementById("strawberry").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("strawberry").style.visibility = "hidden";
      }

      // Peach
      if (document.getElementById("baby_pink").checked) {
        document.getElementById("peach").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("peach").style.visibility = "hidden";
      }

      // Mint
      if (document.getElementById("green").checked) {
        document.getElementById("mint").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("mint").style.visibility = "hidden";
      }

      // Chocolate
      if (document.getElementById("brown").checked) {
        document.getElementById("chocolate").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("chocolate").style.visibility = "hidden";
      }

      // Butterscoth
      if (document.getElementById("yellow").checked) {
        document.getElementById("butterscoth").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("butterscoth").style.visibility = "hidden";
      }

      // BlueBerry
      if (document.getElementById("blue").checked) {
        document.getElementById("blueberry").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("berry").style.visibility = "hidden";
      } else {
        document.getElementById("blueberry").style.visibility = "hidden";
      }

      // Berry
      if (document.getElementById("purple").checked) {
        document.getElementById("berry").style.visibility = "visible";
        document.getElementById("vanilla").style.visibility = "hidden";
        document.getElementById("strawberry").style.visibility = "hidden";
        document.getElementById("peach").style.visibility = "hidden";
        document.getElementById("mint").style.visibility = "hidden";
        document.getElementById("butterscoth").style.visibility = "hidden";
        document.getElementById("chocolate").style.visibility = "hidden";
        document.getElementById("blueberry").style.visibility = "hidden";
      } else {
        document.getElementById("berry").style.visibility = "hidden";
      }
    },
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background-color: #ac9aad;
}

.flavour {
}

.cream {
  text-align: center;
  position: absolute;
  left: 49%;
  top: 45%;
  transform: translate(-50%, -50%);
  font-size: 30px;
  font-size: 30px;
  z-index: 999;
  height: 19%;
  visibility: hidden;
}

#cone {
  text-align: center;
  position: absolute;
  left: 49.7%;
  top: 59%;
  transform: translate(-50%, -50%);
  font-size: 30px;
  font-size: 30px;
}

.choice {
  background-color: #fbdbde;
  width: 19%;
  height: 100%;
  display: block;
  position: absolute;
  top: 0%;
  padding-top: 60px;
  border-right: 1.5px solid #2f4858;
  box-shadow: 10px -3px 20px 8px rgb(28 28 28 / 17%);
  text-align: center;
  line-height: 33px;
}
</style>
