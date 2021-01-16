<template>
  <div class="tournament-view">
    <h1>
      <i class="nes-icon trophy is-large"></i>
      Multigaming Level One
      <i class="nes-icon trophy is-large"></i>
    </h1>
    <h2>Du 11 au 31 Janvier</h2>

    <div class="participants" style="margin-top: 50px;">
      <h2>Participants</h2>
      <div class="lists">
        <ul class="nes-list is-circle">
          <li>THEO <i class="nes-icon coin is-small" v-for="_ in [1,2,3]" v-bind:key="_"></i></li>
          <li>HUGO <i class="nes-icon coin is-small" v-for="_ in [1,2]" v-bind:key="_"></i></li>
          <li>WILL <i class="nes-icon coin is-small" v-for="_ in [1,2]" v-bind:key="_"></i></li>
          <li>RORO</li>
          <li>JAJA</li>
        </ul>
      </div>
    </div>

    <div class="results">
      <h2 style="margin-top: 50px;">Resultats</h2>

      <h3 style="margin-top: 20px;">Golf With Your Friends</h3>
      <div class="nes-table-responsive" style="margin-top: 50px;">
        <table class="nes-table is-bordered is-dark">
          <thead>
            <tr>
              <th>Le Gamer</th>
              <th>Forest</th>
              <th>Haunted (bug)</th>
              <th>Pirate Cove</th>
              <th>Total</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Jaja</td>
              <td>57</td>
              <td>/</td>
              <td>90</td>
              <td>147</td>
            </tr>
            <tr>
              <td>Roro</td>
              <td>45</td>
              <td>/</td>
              <td>83</td>
              <td>115</td>
            </tr>
            <tr>
              <td>Will</td>
              <td>32</td>
              <td>/</td>
              <td>83</td>
              <td>115</td>
            </tr>
            <tr>
              <td>Hugo</td>
              <td>44</td>
              <td>/</td>
              <td>71</td>
              <td>115</td>
            </tr>
            <tr>
              <td><i class="nes-icon trophy is-small"></i>Theo</td>
              <td>34</td>
              <td>/</td>
              <td>72</td>
              <td>106</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tournament"
};
</script>

<style scoped>
.tournament-view {
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
}


ul li::before {
  color: white;
}

.nes-list.is-circle li::before {
  color: white;
}
</style>
