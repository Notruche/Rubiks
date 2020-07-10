<template>
  <div class="body">
    <div class="container m-auto" v-if="intro">
      <img src="./assets/img/page-infinie.jpg" alt="image">
      <div style="position:relative">
        <img src="./assets/img/page-infinie-rubik-gif.gif" alt="image">
        <div class="lien" v-on:click="page1"></div>
      </div>
    </div>
    <div class="story" v-if="pageun" style="position:relative">
      <img src="./assets/img/1-01.gif" class="rubiks" v-if="i==1||i==2">
      <img src="./assets/img/1-02.png" class="modele">
      <img src="./assets/img/1-02.png" class="rubiks" v-if="i==2||i==3">
      <img src="./assets/img/1-03.png" class="rubiks" v-if="i==3||i==4">
      <img src="./assets/img/1-04.png" class="rubiks" v-if="i==4||i==5">
      <img src="./assets/img/1-05.png" class="rubiks" v-if="i==5||i==6">
      <img src="./assets/img/1-06.png" class="rubiks" v-if="i==6||i==7">
      <img src="./assets/img/1-07.png" class="rubiks" v-if="i==7||i==8">
      <img src="./assets/img/1-08.png" class="rubiks" v-if="i==8||i==9">
      <img src="./assets/img/1-09.png" class="rubiks" v-if="i==9||i==10">
      <img src="./assets/img/1-10.png" class="rubiks" v-if="i==10||i==11">
      <img src="./assets/img/1-11.png" class="rubiks" v-if="i==11||i==12">
      <img src="./assets/img/1-12.png" class="rubiks" v-if="i==12||i==13">
      <img src="./assets/img/1-13.png" class="rubiks" v-if="i==13||i==14">
      <img src="./assets/img/1-14.png" class="rubiks" v-if="i==14||i==15">
      <img src="./assets/img/1-15.png" class="rubiks" v-if="i==15||i==16">
      <img src="./assets/img/1-16.png" class="rubiks" v-if="i==16||i==17">
      <img src="./assets/img/1-17.png" class="rubiks" v-if="i==17||i==18">
      <img src="./assets/img/1-18.png" class="rubiks" v-if="i==18||i==19">
      <img src="./assets/img/1-19.png" class="rubiks" v-if="i==19||i==20">
      <img src="./assets/img/1-20.png" class="rubiks" v-if="i==20||i==21">
      <img src="./assets/img/1-21.png" class="rubiks" v-if="i==21||i==22">
      <img src="./assets/img/1-22.png" class="rubiks" v-if="i==22||i==23">
      <img src="./assets/img/1-23.png" class="rubiks" v-if="i==23||i==24">
      <img src="./assets/img/1-24.png" class="rubiks" v-if="i==24||i==25">
      <img src="./assets/img/1-25.png" class="rubiks" v-if="i==25||i==26">
      <img src="./assets/img/1-26.png" class="rubiks" v-if="i==26||i==27">
      <img src="./assets/img/1-27.png" class="rubiks" v-if="i==27||i==28">
      <img src="./assets/img/1-28.png" class="rubiks" v-if="i==28||i==29">
      <img src="./assets/img/1-29.png" class="rubiks" v-if="i==29||i==30">
      <img src="./assets/img/1-30.png" class="rubiks" v-if="i==30||i==31">
      <img src="./assets/img/1-31.png" class="rubiks" v-if="i==31||i==32">
      <img src="./assets/img/1-32.png" class="rubiks" v-if="i==32||i==33">
      <img src="./assets/img/1-33.png" class="rubiks" v-if="i==33||i==34">
      <img src="./assets/img/1-34.png" class="rubiks" v-if="i==34||i==35">
      <img src="./assets/img/1-35.png" class="rubiks" v-if="i==35||i==36">
      <img src="./assets/img/1-36.png" class="rubiks" v-if="i==36||i==37">
      <img src="./assets/img/1-37.png" class="rubiks" v-if="i==37||i==38">
      <img src="./assets/img/1-38.gif" class="rubiks" v-if="i==38||i==40">
      <div class="pg2" v-on:click="page2" v-if="i==38"></div>
      <img src="./assets/img/2-00.gif" class="rubiks" v-if="i>=39&&i<=41">
      <img src="./assets/img/2-40.jpg" class="rubiks" v-if="i==41||i==42">
      <img src="./assets/img/2-41.jpg" class="rubiks" v-if="i==42||i==43">
      <img src="./assets/img/2-42.jpg" class="rubiks" v-if="i==43||i==44">
      <img src="./assets/img/2-43.jpg" class="rubiks" v-if="i==44||i==45">
      <img src="./assets/img/2-44.jpg" class="rubiks" v-if="i==45||i==46">
      <img src="./assets/img/2-45.jpg" class="rubiks" v-if="i==46||i==47">
      <img src="./assets/img/2-46.jpg" class="rubiks" v-if="i==47||i==48">
      <img src="./assets/img/2-47.jpg" class="rubiks" v-if="i==48||i==49">
      <img src="./assets/img/2-48.jpg" class="rubiks" v-if="i==49||i==50">
      <img src="./assets/img/2-49.jpg" class="rubiks" v-if="i==50||i==51">
      <img src="./assets/img/2-50.jpg" class="rubiks" v-if="i==51||i==52">
      <img src="./assets/img/2-51.jpg" class="rubiks" v-if="i==52||i==53">
      <img src="./assets/img/2-52.jpg" class="rubiks" v-if="i==53||i==54">
      <img src="./assets/img/2-53.jpg" class="rubiks" v-if="i==54||i==55">
      <img src="./assets/img/2-54.jpg" class="rubiks" v-if="i==55||i==56">
      <img src="./assets/img/2-55.jpg" class="rubiks" v-if="i==56||i==57">
      <img src="./assets/img/2-56.jpg" class="rubiks" v-if="i==57||i==58">
      <img src="./assets/img/2-57.gif" class="rubiks" v-if="i==58||i==59">
      <div class="pg3" v-on:click="page2" v-if="i==58"></div>
      <img src="./assets/img/3-00.gif" class="rubiks" v-if="i>=59&&i<=60">
      <img src="./assets/img/3-54.jpg" class="rubiks" v-if="i==60||i==61">
      <img src="./assets/img/3-55.jpg" class="rubiks" v-if="i==61||i==62">
      <img src="./assets/img/3-56.jpg" class="rubiks" v-if="i==62||i==63">
      <img src="./assets/img/3-57.jpg" class="rubiks" v-if="i==63||i==64">
      <img src="./assets/img/3-58.jpg" class="rubiks" v-if="i==64||i==65">
      <img src="./assets/img/3-59.jpg" class="rubiks" v-if="i==65||i==66">
      <img src="./assets/img/3-60.jpg" class="rubiks" v-if="i==66||i==67">
      <img src="./assets/img/3-61.jpg" class="rubiks" v-if="i==67||i==68">
      <img src="./assets/img/3-62.jpg" class="rubiks" v-if="i==68||i==69">
      <img src="./assets/img/3-63.jpg" class="rubiks" v-if="i==69||i==70">
      <img src="./assets/img/3-64.jpg" class="rubiks" v-if="i==70||i==71">
      <img src="./assets/img/3-65.jpg" class="rubiks" v-if="i==71||i==72">
      <img src="./assets/img/3-66.jpg" class="rubiks" v-if="i==72||i==73">
      <img src="./assets/img/3-67.jpg" class="rubiks" v-if="i==73||i==74">
      <img src="./assets/img/3-68.jpg" class="rubiks" v-if="i==74||i==75">
      <img src="./assets/img/3-69.jpg" class="rubiks" v-if="i==75||i==76">
      <img src="./assets/img/3-70.jpg" class="rubiks" v-if="i==76||i==77">
      <img src="./assets/img/3-71.jpg" class="rubiks" v-if="i==77||i==78">
      <img src="./assets/img/3-72.gif" class="rubiks" v-if="i==78||i==79">
      <div class="pg4" v-on:click="page2" v-if="i==78"></div>
      <img src="./assets/img/Gif.gif" class="rubiks" v-if="i==79||i==80">
      <img src="./assets/img/4-75.jpg" class="rubiks" v-if="i==80||i==81">
      <img src="./assets/img/4-76.jpg" class="rubiks" v-if="i==81||i==82">
      <img src="./assets/img/4-77.jpg" class="rubiks" v-if="i==82||i==83">
      <img src="./assets/img/4-78.jpg" class="rubiks" v-if="i==83||i==84">
      <img src="./assets/img/4-79.jpg" class="rubiks" v-if="i==84||i==85">
      <img src="./assets/img/4-80.jpg" class="rubiks" v-if="i==85||i==86">
      <img src="./assets/img/4-81.jpg" class="rubiks" v-if="i==86||i==87">
      <img src="./assets/img/4-82.jpg" class="rubiks" v-if="i==87||i==88">
      <img src="./assets/img/4-83.jpg" class="rubiks" v-if="i==88||i==89">
      <img src="./assets/img/4-84.jpg" class="rubiks" v-if="i==89||i==90">
      <img src="./assets/img/4-85.jpg" class="rubiks" v-if="i==90||i==91">
      <img src="./assets/img/4-86.jpg" class="rubiks" v-if="i==91||i==92">
      <img src="./assets/img/4-87.gif" class="rubiks" v-if="i==92||i==93">
      <div class="pg5" v-on:click="page2" v-if="i==92"></div>
      <img src="./assets/img/fin-trauma.gif" class="rubiks" v-if="i==93||i==94">
      <div class="pg6" v-on:click="page2" v-if="i==93"></div>
      <img src="./assets/img/ecran-crédits.gif" class="rubiks" v-if="i==94">
      <div class="pg7" v-on:click="again" v-if="i==94"></div>
      <a
        href="https://www.instagram.com/pekolio/"
        class="insta"
        v-if="i==94"
        target="blank"
      ></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "body",
  data() {
    return {
      intro: true,
      pageun: false,
      i: 0
    };
  },
  methods: {
    again() {
      this.i = 1;
    },
    page1() {
      let self = this;
      this.i = 1;
      this.intro = false;
      this.pageun = true;
      window.addEventListener("keydown", function(e) {
        var keyCode = e.keyCode;
        if (keyCode == 37) {
          //left
          if (self.i > 2)
            if (self.i < 39) {
              self.i -= 1;
              console.log(self.i);
            } else if (self.i > 41 && self.i < 59) {
              self.i -= 1;
              console.log(self.i);
            } else if (self.i > 60 && self.i < 79) {
              self.i -= 1;
              console.log(self.i);
            } else if (self.i > 80 && self.i < 93) {
              self.i -= 1;
              console.log(self.i);
            }
        } else if (keyCode == 39) {
          //right
          if (self.i < 38) {
            self.i += 1;
            console.log(self.i);
          } else if (self.i >= 39 && self.i < 58) {
            self.i += 1;
            console.log(self.i);
          } else if (self.i >= 59 && self.i < 78) {
            self.i += 1;
            console.log(self.i);
          } else if (self.i >= 79 && self.i < 92) {
            self.i += 1;
            console.log(self.i);
          }
        }
      });
    },
    page2() {
      this.i += 1;
    },
    comment() {
      alert(
        "ATTENTION : Vous devez lire cette BD avec Google Chrome ! (désolée)\n Appuyez sur F 11 pour activer le plein écran !"
      );
    }
  },
  created: function() {
    this.comment();
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
