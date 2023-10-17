<template>
    <div class="recap">
      <h3>Récapitulatif de l'intervention</h3>
      <p>Date et heure de début : {{ $route.query.dateDebut }}</p>
      <p>Date et heure de fin : {{ $route.query.dateFin }}</p>
      <p>Intervenant : {{ $route.query.choix_intervenant }}</p>
      <p>Nom du client : {{ $route.query.nomClient }}</p>
      <p>Observations :</p>
      <p>{{ $route.query.Observations }}</p>
    </div>
  </template>
  
  <script>
  export default {
  };
  
  </script>
  

<style>

body{
    color: aliceblue;
    background: #14365b;
}

h3{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 30px;
    text-transform: uppercase;
    background:#14365b;
    color: white;
    text-align: center;
}

.title-text2{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size:25px;
    background:aliceblue;
    color: black;
    border-radius: 6px;
}
h3 p{
    font-size: 20px;
    color: black;
    
}
.second-text{
    font-style: italic;
}

.recap{
  background: white;
  color: black;   border: 1px solid #ffffff;
    border-width: 4px;
    border-radius: 5px;
    width: 100%;
    height: 300px;
}

</style>