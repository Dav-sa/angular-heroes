# Angular Tour Of Heroes

TL:DR Ce projet est recommandé par la documentation d'Angular pour apprendre les bases de ce framework.
L'application permet de :

- consommer une liste de héros et l'afficher à l'utilisateur
- afficher / modifier les détails d'un héros
- permettre la navigation entre deux vues grâce au module de routing

## Les trucs que j'ai bien compris

- utiliser la CLI pour créer des composants / la structure des composants avec un fichier ts qui définit la classe, un fichier html qui définit le template, un fichier de style et un fichier de test
- les décorateurs qui permettent de spécifier de la metadata pour un composant/service.
- les directives qui permettent de dynamiser le templating (ngIf, ngFor, ngModel).
- la directive ngModel et son two-way binding pour lier une variable stateful à un input.
- le hook onInit qui permet d'initialiser le composant après sa création.
- l'utilisation de module dans le fichier AppModule, plus globalement, le découpage rigoureux de l'application.
- La séparation des préoccupations entre les composants et les services : les composants sont responsables de l'affichage et de la logique de l'UI, les services sont responsables de la logique métier et de la communication avec les API.
- Venant de l'univers de React, c'est un très grand changement de séparer les composants et les services. Avec React il faut connaître une librairie de création de formulaire, un client http, un router... Avec Angular tout immédiatement disponible sous forme de module.
- Par exemple le data fetching semble bien plus cadré sur Angular : avec React on utilise un hook useEffect directement dans le composant, ensuite il faut connaitre un client http comme Axios, puis gérer les erreurs, ou bien apprendre une librairie qui fait tout ca comme react-query.
- Avec Angular, on crée un service qui va gérer le data fetching, puis on injecte ce service dans le composant qui va l'utiliser.

## Les trucs que j'ai moins bien compris

- Il y a une grande utilisation qui est faite de certains design pattern : le singleton, l'observable, le décorateur.
- La notion d'injection de dépendance.
- L'idée d'injecter un service dans un service puis dans un composant.
- la libraire RxJS et la gestion des observables.
