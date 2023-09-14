# Algorithme DAB

Conception d'un algorithme de DAB , sous forme de pseudo-code.

  
---

```text 
Le client insére sa cb ds le DAB
Le process de vérification est lancé
    SI la cb n'est pas conforme
        ALORS le DAB rejette la carte 
        Le programme s'arrete
    SINON SI la carte est bloquée
        ALORS le DAB avale la cb
         Le programme s'arrete
    SINON la cb est valide 
        la carte est valide 
        Lancer la dmde du code de la carte 
Le DAB affiche un msg"demandant le code de la carte"
Le client tape un code
    SI le code est incorrect
        ALORS le DAB affiche un msg "code incorrect"
        ET le compteur de tentative est incrémenté de 1 
        SI le compteur de tentative est égal à 3
            ALORS  le distributeur avale la carte
            le programme s'arrete
        Lancer la dmde du code de la carte 
    SINON
        Le code est correct
        Lancer la dmde 
Le distributeur affiche un msg "demanadant de choisir un montant à retirer"
Le client choisit un montant
Le processus de vérification de solde du client est lancé 
    SI le montant choisi > le solde || le montant > plafond 
        Le retrait est refusé 
        Le distributeur affiche un message   
        Le DAB relance la dmde du montant à retirer      
    SINON
        Le retrait est autorisé 
        Le processus de vérification de solde DAB est lancé
            SI  le montant > le solde
                Le retrait est refusé
                Le distributeur affiche un message  
                Le DAB relance la dmde du montant à retirer  
            SINON
                Le retrait est autorisé
                Le DAB remet le montant choisi
Le client recupere sa CB 
Le client recupère l'argent du DAB
Fin du programme
```

                 