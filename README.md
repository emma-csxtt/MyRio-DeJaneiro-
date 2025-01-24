Exo1 : LED : 
L'objectif est de faire clignoter la LED0 en fonction d'un bouton d'activation. 
De ce fait, nous avons voulu procéder de la manière suivante : 
    La boucle While nous permet de recuperer l'index temps évoluant de un en un, nous le divisons par 2 pour determiner un pair ou un impaire.
    Ensuite en fonction du reste (dans le cas d'un reste = 0 alors on essaye d'activer la led) et de l'activation du bouton soumis a un "AND" logique nous activons ou desactivons la LED0.
    Le bouton stop permet d'arreter le programme.
    Le Wait time permet de "ralentir" le programme ce qui nous permet de visualiser le clignotement de la led.
    Une gestion d'erreur a été faite.

Exo 2 : Gyroscope :
L'objectif est de recuperer les valeurs d'accéléromètre suivant les axes X,Y et Z. 
Nous avons donc :
    Une boucle While pour assurer la continuité de la lecture des données.
    Une fois récuperer nous devons appliquer un filtre Passe-Bas pour lisser les données.
    Pour finalement les afficher sur un oscilloscope.
    Un bouton Stop permet d'arreter le programme.
    Une gestion d'erreur a été faite.

Exo 3 : "Bulleur"
L'objectif est de creer un Bulleur Numérique en fonction de l'axe Z.
Voici comment nous avons imaginé le systeme : 
    Une boucle deterministe permettant la continuité de lecture des données avec l'activation des leds en fonction de l'angle détecté.
    La boucle non déterministe est utilisée pour mettre à jour la valeur référence de l'angle lorsque l'on appui sur le bouton de la MyRio.
    La communication entre les 2 boucles se fait via des variables partagées.
    
      
