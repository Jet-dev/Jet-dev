<template>
  <div class="tournament-view">
    <h1>
      <i class="nes-icon trophy is-large"></i>
      Multigaming Level One
      <i class="nes-icon trophy is-large"></i>
    </h1>
    <h2>Du 11 Janvier au 5 Février</h2>

    <div class="participants" style="margin-top: 50px;">
      <h2>Participants</h2>
      <div class="lists">
        <ul class="nes-list is-circle" style="text-align: left">
          <li>
            THEO
            <i
              class="nes-icon coin is-small"
              v-for="_ in [1, 2, 3, 4, 5, 6, 7]"
              v-bind:key="_"
            ></i>
          </li>
          <li>
            WILL
            <i
              class="nes-icon coin is-small"
              v-for="_ in [1, 2, 3, 4, 5, 6]"
              v-bind:key="_"
            ></i>
          </li>
          <li>
            HUGO
            <i
              class="nes-icon coin is-small"
              v-for="_ in [1, 2, 3, 4, 5]"
              v-bind:key="_"
            ></i>
          </li>
          <li>
            JAJA
            <i
              class="nes-icon coin is-small"
              v-for="_ in [1]"
              v-bind:key="_"
            ></i>
          </li>
          <li>RORO</li>
        </ul>
      </div>
    </div>

    <div class="results">
      <h2 style="margin-top: 50px;">Resultats</h2>

      <h3 style="margin-top: 20px;">Golf With Your Friends</h3>

      <div
        class="nes-table-responsive"
        style="margin-top: 50px;display:flex;flex-direction:column;align-items:center;"
      >
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

      <h3 style="margin-top:20px;">
        Age of Empire II : Definitive Edition
      </h3>

      <div
        class="nes-table-responsive"
        style="margin-top:50px;display:flex;flex-direction:column;align-items:center;"
      >
        <table class="nes-table is-bordered is-dark">
          <thead>
            <tr>
              <th>Le Gamer</th>
              <th>Score</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Jaja</td>
              <td>2077</td>
            </tr>
            <tr>
              <td>Roro</td>
              <td>1386</td>
            </tr>
            <tr>
              <td><i class="nes-icon trophy is-small"></i> Will</td>
              <td>20142</td>
            </tr>
            <tr>
              <td>Hugo</td>
              <td>1900</td>
            </tr>
            <tr>
              <td>Theo</td>
              <td>2130</td>
            </tr>
            <tr>
              <td>Thomas (guest)</td>
              <td>3938</td>
            </tr>
          </tbody>
        </table>
      </div>

      <h3 style="margin-top: 20px;">Trackmania Stadium</h3>
      <div class="nes-table-responsive" style="margin-top: 50px;">
        <table class="nes-table is-bordered is-dark">
          <thead>
            <tr>
              <th>Le Gamer</th>
              <th>Map 1</th>
              <th>Map 2</th>
              <th>Map 3</th>
              <th>Map 4</th>
              <th>Map 5</th>
              <th>Classement final</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Jaja</td>
              <td>1.03.82</td>
              <td>0.49.414</td>
              <td>0.40.890</td>
              <td>0.47.582</td>
              <td>1.02.494</td>
              <td>4</td>
            </tr>
            <tr>
              <td>Roro</td>
              <td>Forfait</td>
              <td>Forfait</td>
              <td>Forfait</td>
              <td>Forfait</td>
              <td>Forfait</td>
              <td>5</td>
            </tr>
            <tr>
              <td>Will</td>
              <td>0.57.208</td>
              <td>0.46.205</td>
              <td>0.39.964</td>
              <td>0.42.628</td>
              <td>1.00.436</td>
              <td>3</td>
            </tr>
            <tr>
              <td><i class="nes-icon trophy is-small"></i> Hugo</td>
              <td>0.57.379</td>
              <td>0.45.423</td>
              <td>0.38.324</td>
              <td>0.42.165</td>
              <td>0.57.558</td>
              <td>1</td>
            </tr>
            <tr>
              <td>Theo</td>
              <td>0.55.838</td>
              <td>0.46.328</td>
              <td>0.37.118</td>
              <td>0.44.108</td>
              <td>0.59.305</td>
              <td>2</td>
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
