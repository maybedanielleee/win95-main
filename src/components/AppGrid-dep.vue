<template>
  <div class="app-grid">
    <button class="app" v-touch:tap="openBio" v-on:dblclick="openBio">
      <img class="icon app-bio" src="../assets/win95Icons/bio.png" />
      <div class="border">
        <div class="icon-text">Biography</div>
      </div>
    </button>
    <button class="app" v-touch:tap="openPhotos" v-on:dblclick="openPhotos">
      <img class="icon app-photos" src="../assets/win95Icons/photos.png" />
      <div class="border">
        <div class="icon-text">Photos</div>
      </div>
    </button>
    <button class="app" v-touch:tap="openMail" v-on:dblclick="openMail">
      <img class="icon app-mail" src="../assets/win95Icons/mail.png" />
      <div class="border">
        <div class="icon-text">Electronic Mail</div>
      </div>
    </button>
  </div>
</template>
<style scoped>
.app-grid {
  display: grid;
  grid-gap: 20px;
  margin-left: 10px;
  justify-items: center;
  align-items: center;
  margin-top: 10px;
}
.app {
  width: 60px;
  height: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  font-size: 12px;
  color: white;
  padding: 10px;
}
button {
  background: none;
  color: inherit;
  border: none;
  font: inherit;
  outline: inherit;
}
a {
  color: white;
  text-decoration: none;
}
.app:focus .border {
  border: rgb(255, 255, 148) dotted 1px;
}
.app:focus .icon {
  filter: grayscale(100%) brightness(30%) sepia(100%) hue-rotate(-180deg)
    saturate(400%) contrast(0.9);
}
.app:focus .icon-text {
  background: rgb(0, 0, 118);
}
.icon {
  width: 30px;
  height: 30px;
  margin-bottom: 5px;
}
</style>
<script>
export default {
  data() {
    return {
      activeIcon: "",
    };
  },
  methods: {
    openBio(e) {
      e.stopPropagation();
      this.$store.commit("toggleCloseBio", true);
      this.$store.commit("toggleShownBio", true);
      this.$store.commit("changeActiveWindow", "Bio");
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "bio");
      }, 1);
    },
    openMail(e) {
      e.stopPropagation();
      this.$store.commit("toggleCloseMail", true);
      this.$store.commit("toggleShownMail", true);
      this.$store.commit("changeActiveWindow", "Mail");
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "mail");
      }, 1);
    },
    openPhotos(e) {
      e.stopPropagation();
      this.$store.commit("toggleClosePhotos", true);
      this.$store.commit("toggleShownPhotos", true);
      this.$store.commit("changeActiveWindow", "Photos");
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "photos");
      }, 1);
    },
    openNoss(e) {
      e.stopPropagation();
      this.$store.commit("toggleCloseNossaflex", true);
      this.$store.commit("toggleShownNossaflex", true);
      this.$store.commit("changeActiveWindow", "NOSSAFLEX");
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "noss");
      }, 1);
    },
    openResume(e) {
      e.stopPropagation();
      this.$store.commit("toggleCloseResume", true);
      this.$store.commit("toggleShownResume", true);
      this.$store.commit("changeActiveWindow", "Resume");
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "resume");
      }, 1);
    },
  },
};
</script>
