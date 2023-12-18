# Configuration Variables

##PANELTRANSPARENCY## -> Ce n'est plus utilisable.

##PAGEBACKGROUNDCOLOR## -> Couleur du fond du panneau -> (en RGBA)  : La couleur doit être en rgba afin que les utilisateurs puissent choisir la transparence.

##PANELBLUR## -> (en px) 

##MAINBUTTONCOLOR## -> Couleur du fond des boutons principaux -> (en Hexa) / (en RGBA)

##SECONDARYBUTTONCOLOR## -> Couleur du fond des boutons secondaires -> (en Hexa) / (en RGBA) 

##MAINBUTTONTEXTCOLOR## -> Couleur du text des boutons principaux -> (en Hexa) / (en RGBA) : Calculer par le logiciel par rapport à ##MAINBUTTONCOLOR## 

##SECONDARYBUTTONTEXTCOLOR## ->  Couleur du text des boutons secondaires -> (en Hexa) / (en RGBA) : Calculer par le logiciel par rapport à ##SECONDARYBUTTONCOLOR## 


##SECONDARYCOLOR## -> Couleur du texte secondaire (champs input ...) + le trait en dessous des inputs + le trait séparateur du pied de page -> (en Hexa)  / (en RGBA)

##PAGECOLOR## -> Couleur du texte principale + la couleur du trait qui s'étend lorsqu'on focus sur les champs "input" -> (en Hexa) 

##PANELPOSITION## -> left-blur / right-blur / center-blur

##PHOTONAME## -> Lien de l'image de fond sans les guillemets -> ex : BG/default.jpg

##LOGO## -> Lien du logo sans les guillemets -> ex : img/default.jpg

##TITLE## -> Une chaîne de caractères

##CUSTOMTEXT## -> Une chaîne de caractères : text du footer 

##CUSTOMTEXTCOLOR## -> (en HEX ) / en (RGBA) : couleur text du footer  


##LABELUSERNAME##

##LABELPASSWORD##

##LABELDOMAIN##

##LABELTWOFACTOR##

##LABELLOGON##

##TR-FOOTER## -> pour Cacher le footer -> valeurs attendues :   block / none 


# Détail des calculs : 

A consulter : https://github.com/Amine210/TSplus-variables/blob/main/index.js 


## La fonction computeLuminence calcule la luminance d'une couleur d'arrière-plan 

### Paramètres : 
                backgroundcolor (String) : La couleur d'arrière-plan  en RGB  pour laquelle la luminance doit être calculée. Cela doit être un code couleur RGB valide

### Valeur de retour
                luminence (Number) : La valeur de luminance calculée pour la couleur d'arrière-plan fournie.


 
## La fonction shouldTextBeBlack détermine si le texte doit être affiché en noir en se basant sur la luminance de la couleur d'arrière-plan. Si la luminance est supérieure à 0,5, la fonction renvoie true

### Paramètres :
                backgroundcolor (String) : La couleur d'arrière-plan à évaluer.

### Valeur de retour :   
                 true si le texte doit être en noir, false sinon.

  # Web-Portal
