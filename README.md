# Projet de visualisation de donn�es 

WhereWasI? - Comment me suis-je d�plac� ?

Projet r�alis� par Th�o PONTON, Julien GRENIER et Martin CHAUVIN dans le cadre du MOS 5.5 de l'Ecole Centrale Lyon

*La question � laquelle nous voulons r�pondre* 
Nous voulons savoir quels d�placements ont �t� effectu�s par une personne :
Dans quelles villes / pays (localisation sur une carte) cette personne a �t�
Comment se sont r�partis ses d�placements (entre 0 et 24 heures) pour chaque jour de la semaine
La distance moyenne parcourue et avec quels moyens de transport pour chaque jour de la semaine
Nous voulons �galement pouvoir s�lectionner la p�riode temporelle sur laquelle visualiser ces donn�es.

*De quel donn�es avons nous besoin ?*
Nous avons besoin de positions GPS d�une personne avec une fr�quence de plusieurs fois par jour. Soit au minimum un triplet de type : latitude, longitude, temps du relev� de position.
Pour chacune de ces positions, nous avons �galement besoin d�une estimation du mode de d�placement : statique, marche, course, v�lo, voiture, ...

*Comment nous allons collecter les donn�es*
Nous allons utiliser les donn�es li�es aux comptes Google. Google permet de t�l�charger ses donn�es personnelles dont les donn�es de localisation. L�historique de position � disposition est tr�s complet et fournit notamment les informations de positions et d�activit� avec un interval de 2 minutes.

*Quels sont les principaux risques de collection et visualisation de ces donn�es ?*
Pour la collection, il est possible que la personne ait d�sactiv� l�historique des localisations. Dans ce cas, les donn�es google ne sont pas disponibles et il faut se rabattre sur d�autres moyens comme les donn�es de localisation Facebook ou Waze. Le probl�mes c�est que les donn�es de ces derni�res application sont moins compl�tes que celles de google.
Pour la visualisation, si les donn�es sont interrompus (points de localisation manquant) cela peut poser probl�me. On peut mal interpr�ter un trajet qui comporte des segments manquants. Il y a aussi un risque que l�estimation de l�activit� de d�placement faite par google soit fausse.

*Quels sont les possibles probl�mes �thiques/donn�es priv�es ?*
Un probl�me pourrait se poser si la personne dont laquelle les donn�es sont trait�es ne donne pas son consentement ou le retire. Afin de contourner ce probl�me, nous allons prendre les donn�es d�une personne du groupe. Nous garantissons ainsi le consentement.
Dans un but d�exposition du travail au un public plus large (comme Linkedin voir m�me pour le cours) nous allons anonymiser ces donn�es. 

Test

