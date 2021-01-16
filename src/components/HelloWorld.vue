<template>
  <div class="hello">

    <div class="nes-container is-dark with-title nes-pointer tournament" @click="goToTournament()">
      <p class="title">Multigaming Level One - Du 11 au 31 Janvier</p>
      <div>
        <div class="lists">
          <ul class="nes-list is-circle">
            <li>Age of Empire II</li>
            <li>Trackmania</li>
            <li>Warsow</li>
            <li>Golf with friends</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import {Options, Vue} from "vue-class-component";

@Options({
  props: {},
  methods: {
    goToTournament() {
      this.$router.push("/tournament/1");
    }
  }
})
export default class HelloWorld extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.tournament {
  margin-top: 80px;
  width: 1200px;
}

.hello {
  display: flex;
  flex-direction: column;
  align-items: center;
}

ul {
  text-align: left;
}

ul li::before {
  color: white;
}

.nes-list.is-circle li::before {
  color: white;
}
</style>
