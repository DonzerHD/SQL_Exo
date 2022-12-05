## 1:Sélectionner toutes les colonnes de la table SERV.
SELECT noserv FROM serv;
SELECT service FROM serv;
SELECT ville FROM serv;

## 2:Sélectionner d’une autre manière ces colonnes.
SELECT * FROM serv;

## 3:Sélectionner les colonnes SERVICE et NOSERV de la table SERV.
SELECT SERVICE, NOSERV FROM SERV;

## 4:Sélectionner toutes les colonnes de la table EMP.
SELECT * FROM EMP;

## 5:Sélectionner les emplois de la table EMP.
SELECT  emploi FROM EMP;

## 6:Sélectionner les différents emplois de la table EMP.
SELECT DISTINCT emplois FROM EMP;

## 7 : Sélectionner les employés du service N°3.
SELECT * FROM emp WHERE noserv = 3;

## 8 : Sélectionner les noms, prénoms, numéro d’employé, numéro de service de tous les techniciens.
SELECT nom, prenom, noemp, noserv FROM emp WHERE emploi = 'TECHNICIEN';

## 9 : Sélectionner les noms, numéros de service de tous les services dont le numéro est supérieur à 2.
SELECT nom, noserv FROM emp WHERE noserv > 2;

## 10 : Sélectionner les noms, numéros de service de tous les services dont le numéro est inférieur ou égal à 2.

/*11 : Sélectionner les employés dont la commission est inférieure au salaire. Vérifiez le résultat jusqu’à obtenir la bonne réponse.*/
/*12 : Sélectionner les employés qui ne touchent jamais de commission.*/
/*13 : Sélectionner les employés qui touchent éventuellement une commission et dans l’ordre croissant des commissions.*/
/*14 : Sélectionner les employés qui ont un chef.*/
/*15 : Sélectionner les employés qui n’ont pas de chef.*/
/*16 : Sélectionner les noms, emploi, salaire, numéro de service de tous les employés du service 5 qui gagnent plus de 20000 €.*/
/*17 : Sélectionner les vendeurs du service 6 qui ont un revenu mensuel supérieur ou égal à 9500 €.*/
/*18 : Sélectionner dans les employés tous les présidents et directeurs. Attention, le français et la logique sont parfois contradictoires.*/
/*19 : Sélectionner les directeurs qui ne sont pas dans le service 3.*/
/*20 : Sélectionner les directeurs et « les techniciens du service 1 ».*/
/*21 : Sélectionner les « directeurs et les techniciens » du service 1.*/
/*22 : Sélectionner les employés du service 1 qui sont directeurs ou techniciens.*/
/*23 : Sélectionner les employés qui ne sont ni directeur, ni technicien et travaillant dans le service 1.*/
/*24 : Sélectionner les employés qui sont techniciens, comptables ou vendeurs.*/
/*25 : Sélectionner les employés qui ne sont ni technicien, ni comptable, ni vendeur.*/
/*26 : Sélectionner les directeurs des services 2, 4 et 5.*/
/*27 : Sélectionner les subalternes qui ne sont pas dans les services 1, 3, 5.*/
/*28 : Sélectionner les employés qui gagnent entre 20000 et 40000 euros, bornes comprises.*/
/*29 : Sélectionner les employés qui gagnent moins de 20000 et plus de 40000 euros.*/
/*30 : Sélectionner les employés qui ne sont pas directeur et qui ont été embauchés en 88.*/
/*30 : Sélectionner les employés qui ne sont pas directeur et qui ont été embauchés en 88.*/
/*31 : Sélectionner les directeurs des services 2 ,3 , 4, 5 sans le IN.*/
/*32 :Sélectionner les employés dont le nom commence par la lettre M.*/
/*33 : Sélectionner les employés dont le nom se termine par T.*/
/*34 : Sélectionner les employés ayant au moins deux E dans leur nom.*/
/*35 : Sélectionner les employés ayant exactement un E dans leur nom.*/
/*36 : Sélectionner les employés ayant au moins un N et un O dans leur nom.*/
/*37 : Sélectionner les employés dont le nom s'écrit avec 6 caractères et qui se termine par N.*/
/*38 : Sélectionner les employés dont la troisième lettre du nom est un R.*/
/*39 : Sélectionner les employés dont le nom ne s'écrit pas avec 5 caractères.*/
/*40 : Trier les employés (nom, prénom, n° de service, salaire) du service 3 par ordre de salaire croissant.*/
/*41 : Trier les employés (nom, prénom, n° de service , salaire) du service 3 par ordre de salaire décroissant.*/
/*42 : Idem en indiquant le numéro de colonne à la place du nom colonne.*/
/*43 : Trier les employés (nom, prénom, n° de service, salaire, emploi) par emploi, et pour chaque emploi par ordre décroissant de salaire.*/
/*44 : Idem en indiquant les numéros de colonnes.*/
/*45 : Trier les employés (nom, prénom, n° de service, commission) du service3 par ordre croissant de commission.*/
/*46 : Trier les employés (nom, prénom, n° de service, commission) du service 3 par ordre décroissant de commission, en considérant que celui dont la commission est nulle ne touche pas de commission.*/
/*47 : Sélectionner le nom, le prénom, l'emploi, le nom du service de l'employé pour tous les employés.*/
/*48 : Sélectionner le nom, l'emploi, le numéro de service, le nom du service pour tous les employés.*/
/*49 : Idem en utilisant des alias pour les noms de tables.*
/*50 : Sélectionner le nom, l'emploi, suivis de toutes les colonnes de la table SERV pour tous les employés.*/
/*51 : Sélectionner les nom et date d'embauche des employés suivi des nom et date d'embauche de leur supérieur pour les employés plus ancien que leur supérieur, dans l'ordre nom employés, noms supérieurs.*/
/*52 : Sélectionner sans doublon les prénoms des directeurs et « les prénoms des techniciens du service 1 » avec un UNION.*/
/*53 : Sélectionner les numéros de services n’ayant pas d’employés sans une jointure externe.*/
/*54 : Sélectionner les services ayant au moins un employé.*/
/*54 bis : Sélectionner les numéros de services ayant des employés sans une jointure externe*/
/*56 : Sélectionner les employés qui ont le même chef que DUBOIS, DUBOIS exclu.*/
/*57 : Sélectionner les employés embauchés le même jour que DUMONT.*
/*58 : Sélectionner les nom et date d'embauche des employés plus anciens que MINET, dans l’ordre des embauches.*/
/*59 : Sélectionner le nom, le prénom, la date d’embauche des employés plus anciens que tous les employés du service N°6. (Attention MIN)*/
/*60 : Sélectionner le nom, le prénom, le revenu mensuel des employés qui gagnent plus qu'au moins un employé du service N°3, trier le résultat dans l'ordre croissant des revenus mensuels.*/
/*61 : Sélectionner les noms, le numéro de service, l’emplois et le salaires des personnes travaillant dans la même ville que HAVET.*/
/*62 : Sélectionner les employés du service 1, ayant le même emploi qu'un employé du service N°3.*/
/*63 : Sélectionner les employés du service 1 dont l'emploi n'existe pas dans le service 3.*/
/*64 : Sélectionner nom, prénom, emploi, salaire pour les employés ayant même emploi et un salaire supérieur à celui de CARON.*/
/*65 : Sélectionner les employés du service N°1 ayant le même emploi qu'un employé du service des VENTES.*/
/*66 : Sélectionner les employés de LILLE ayant le même emploi que RICHARD, trier le résultat dans l'ordre alphabétique des noms.*/
/*67 : Sélectionner les employés dont le salaire est plus élevé que le salaire moyen de leur service (moyenne des salaires = avg(sal)), résultats triés par numéros de service.*/
/*68 : Sélectionner les employés du service INFORMATIQUE embauchés la même année qu'un employé du service VENTES.( année : to_char(embauche,’YYYY’) )*/
/*69 : Sélectionner le nom, l’emploi, la ville pour les employés qui ne travaillent pas dans le même service que leur supérieur hiérarchique direct.*/
/*70 : Sélectionner le nom, le prénom, le service, le revenu des employés qui ont des subalternes, trier le résultat suivant le revenu décroissant.*/
/*71 :Sélectionner le nom, l’emploi, le revenu mensuel (nommé Revenu) avec deux décimales pour tous les employés, dans l’ordre des revenus décroissants.*/
/*72 : Sélectionner le nom, le salaire, commission des employés dont la commission représente plus que le double du salaire.*/
/*73 : Sélectionner nom, prénom, emploi, le pourcentage de commission (deux décimales) par rapport au revenu mensuel ( renommé "% Commissions") , pour tous les vendeurs dans l'ordre décroissant de ce pourcentage.*/
/*74 : Sélectionner le nom, l’emploi, le service et le revenu annuel ( à l’euro près) de tous les vendeurs.*/
/*75 : Sélectionner nom, prénom, emploi, salaire, commissions, revenu mensuel pour les employés des services 3,5,6.*/
/*76 : Idem pour les employés des services 3,5,6 en remplaçant les noms des colonnes : SAL par SALAIRE, COMM par COMMISSIONS, SAL+IFNULL(COMM,0) par GAIN_MENSUEL.*/
/*77 : Idem pour les employés des services 3,5,6 en remplaçant GAIN_ MENSUEL par GAINMENSUEL.*/
/*78 : Afficher le nom, l'emploi, les salaires journalier et horaire pour les employés des services 3,5,6 (22 jours/mois et 8 heures/jour), sans arrondi, arrondi au centime près.*/
/*79 : Idem sans arrondir mais en tronquant.

/*80 : Concaténer les colonnes Service et Ville en les reliant par " ----> ", les premières lettres des noms de villes doivent se trouver sur une même verticale.
/*81 : Sélectionner nom, emploi pour les employés en ajoutant une colonne "CODE EMPLOI", trier le résultat sur ce code. 0 signifie que le code emploi n’existe pas.
/*82 : Sélectionner les employés en remplaçant les noms par '*****' dans le service n°1, trier le résultat suivant le N° de service.
/*83 : Sélectionner les noms des services en affichant que les 5 premiers caractères.
/*84 : Sélectionner les employés embauchés en 1988.
/*85 : Sélectionner les noms des employés sur 3 colonnes la première en majuscules, la seconde avec l'initiale en majuscule et le reste en minuscules, la troisième en minuscules.
/*86 : Sélectionner les positions des premiers M et E dans les noms des employés
/*87 : Afficher le nombre de lettres qui sert à écrire le nom de chaque service.
/*88 : Tracer un Histogramme des salaires avec nom, emploi, salaire triés dans l'ordre décroissant (max de l’histogramme avec 30 caractères).
/*89 : Sélectionner nom, emploi, date d'embauche des employés du service 6.
/*90 : Même chose en écrivant la colonne embauche sous la forme ‘dd-mm-yy’, renommée embauche.
/*91 : Même chose en écrivant la colonne embauche sous la forme ‘day dd month yyyy'
/*92 : Même chose en écrivant la colonne embauche sous la forme ‘day dd month(abv) yy'
/*93 : Même chose en écrivant la colonne embauche sous la forme ‘yy month(abv) dd'
/*94 : Même chose en écrivant la colonne embauche sous la forme ‘Day-dd-Month-yyyy'
/*95 : Sélectionner les employés avec leur ancienneté en jours dans l'entreprise.
/*96 : Sélectionner les employés avec leur ancienneté en mois dans l'entreprise.
/*97 : Sélectionner toutes les dates d’embauche majorées de 12 ans.
/*98 : Sélectionner les employés ayant plus de 12 ans d’ancienneté.

Plus amusant …
/*99 : Depuis combien de jours êtes-vous nés ?
/*00 : Depuis combien de mois êtes-vous nés ?