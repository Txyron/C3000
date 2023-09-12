<template>
    <h4 class="title-text">Récapitulatif
    <p>Nom de l'intervenant : <span id="choix_intervenant"></span></p>
    
<p class="title-text2">Bonjour, M./Mme,<br>
Nous allons intervenir à partir de <span id="dateDebut"></span> jusqu’à <span id="dateFin"></span> pour l’intervention prévue en ce jour.</p>

<br>
<p class="second-text">Vous avez besoin d’informations complémentaires ou vous souhaitez reporter l’intervention ? Contactez-nous dès maintenant en répondant à notre email ou  téléphone.</p>
</h4>

</template>

<script>
export default{
    data(){
        return{
            recap:[
                {title: 'Retour accueil', id:1, details: 'retour'}
            ]
        }
    }
}
</script>

<style>

body{
    color: aliceblue;
    background: #14365b;
}

h2{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 50px;
    border: 1px solid #ffffff;
    border-width: 4px;
    border-radius: 5px;
    background:aliceblue;
    color: black;
    text-align: center;
}

.title-text2{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size:25px;
    background:aliceblue;
    color: black;
}
h2 p{
    font-size: 20px;
    
}
.second-text{
    font-style: italic;
}

</style>