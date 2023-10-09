<template>
  <div class="about">
    <main class="content">
      <div class="box">
        <h3>Fiche d'intervention</h3>
        <div class="box-1">
          <h4>Date et heure de début</h4>
          <input type="datetime-local" v-model="dateDebut">
          <h4>Date et heure de fin :</h4>
          <input type="datetime-local" v-model="dateFin">
          <h4>Intervenant :</h4>
          <select v-model="choix_intervenant">
            <option value="Hugo">Hugo</option>
            <option value="Louis">Louis</option>
            <option value="Lucas">Lucas</option>
            <option value="David">David</option>
          </select>
        </div>
        <div class="box-2">
          <h4>Nom du client :</h4>
          <input type="text" v-model="nomClient" placeholder="Nom du client...">
          <h4>Observations</h4>
          <textarea v-model="Observations" cols="30" rows="10" placeholder="Saisissez vos observations ici..."></textarea>
          <router-link :to="{ path: '/Recap', query: { dateDebut, dateFin, choix_intervenant, nomClient, Observations } }">
            <button class="button">ENVOYER</button>
          </router-link>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dateDebut: '',
      dateFin: '',
      choix_intervenant: '',
      nomClient: '',
      Observations: '',
    };
  },
};
</script>


<style>

h3 {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  text-align: center;
  padding: 20px;
  color: #ffffff;
  font-size: 20px;
}

.button {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  color: #ffffff;
  background-color: #55ab41;
  margin: 5px;
  padding: 10px;
  width: 50%;
  border-style: none;
  border-radius: 10px;
  transition: background-color 0.3s ease, color 0.3s ease;
}

.button:hover {
  background-color: #14365b; /* Changez cette couleur selon vos préférences */
  color: #fff; /* Changez cette couleur selon vos préférences */
}


.content {
  background-repeat: no-repeat;
  background-size: cover;
  margin: 10px;
  padding: 0;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.box {
  text-align: center;
  background-color: #000000;
  padding: 5%;
  margin: 10%; /* Augmentation des marges */
  width: 100%; 
  height: 100%;
  border: 2px solid #ffffff;
  border-radius: 10px;
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}


.box-1, .box-2 {
  width: 100%; 
  box-sizing: border-box;
  padding: 2px;
  
}

textarea {
  width: 100%;
  height: 60px;
  padding: 10px;
  border: 2px solid #3d3d33;
  border-radius: 5px;
}
@media (max-width: 768px) {
  .box-container {
    margin: 20px;
    padding: 10px;
  }

  .button {
  width: 100%;

}
}
</style>
