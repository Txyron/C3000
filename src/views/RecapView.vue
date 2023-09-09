<template>
<h1>RECAP 
    
    
<p>Bonjour, M./Mme,<br>
Nous allons intervenir aujourd’hui à partir de *DATE ET HEURE* jusqu’à *DATE ET HEURE* au *RUE/ADRESSE* pour l’intervention prévue en ce jour.</p>
</h1>


<p class="msgaide">Vous avez besoin d’informations complémentaires ou vous souhaitez reporter l’intervention ? Contactez-nous dès maintenant en répondant à notre email ou  téléphone.</p>



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
}

h1{
    color: aliceblue;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 40px;
}
h1 p{
    font-size: 20px;
}
.msgaide{
    font-style: italic;
}

</style>