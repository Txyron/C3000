<template>
<h1 class="title-text">RECAP 
    
    
<p class="title-text2">Bonjour, M./Mme,<br>
Nous allons intervenir aujourd’hui à partir de *DATE ET HEURE* jusqu’à *DATE ET HEURE* au *RUE/ADRESSE* pour l’intervention prévue en ce jour.</p>


<p class="second-text">Vous avez besoin d’informations complémentaires ou vous souhaitez reporter l’intervention ? Contactez-nous dès maintenant en répondant à notre email ou  téléphone.</p>
</h1>



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

h1{
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
    border: 1px solid #000000;
    border-width: 4px;
    border-radius: 5px;
    background:aliceblue;
    color: black;
}
h1 p{
    font-size: 20px;
    
}
.second-text{
    font-style: italic;
}

</style>