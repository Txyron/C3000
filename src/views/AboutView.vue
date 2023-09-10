<template>
  <div class="about">
    <div id="app">
    <main class="content">
      <div class="box">
        <h3>Fiche d'intervention</h3>

        <div class="box-1">
          <h4>Date et heure de début</h4>
          <input type="datetime-local" name="dateDebut" id="dateDebut" value="2023-09-06T08:00">
          <h4>Date et heure de fin :</h4>
          <input type="datetime-local" name="dateFin" id="dateFin" value="2023-09-06T10:00">
          <h4>Intervenant :</h4>
          <input type="text" name="intervenant" id="intervenant" placeholder="Nom de l'intervenant...">
          <h4>Nature de l’intervention</h4>
          <textarea
            name="Nature d'intervention"
            id=""
            cols="30"
            rows="10"
            placeholder="Saisissez votre message ici..."
          ></textarea>
        </div>

        <div class="box-2">
          <h4>Nom du client :</h4>
          <input type="text" name="nomClient" id="nomClient" placeholder="Nom du client...">
          <h4>Adresse :</h4>
          <input type="text" name="adresseClient" id="adresseClient" placeholder="Adresse...">
          
          <h4>Observations</h4>
          <textarea
            name="Observations"
            cols="30"
            rows="10"
            placeholder="Saisissez vos observations ici..."
          ></textarea>
          <router-link to="/Recap"><button class="button">ENVOYER</button></router-link>
        </div>
      </div>
    </main>
  </div>
  </div>
</template>

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
  margin: 5%; 
  border: 2px solid #ffffff;
  border-radius: 10px;
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.box-1, .box-2 {
  width: 100%; 
  box-sizing: border-box;
  padding: 5px;
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
