# Au delà de TF-IDF

Vous êtes vraiment fier de maîtriser l'algorithme TF-IDF et voulez créer un moteur de recherche pour votre organisation. C'est à ce moment que les responsables du projet vous demandent d'ajouter des tas de nouvelles fonctionnalités, comme par exemple:

- la recherche d'une phrase exacte, permettant de trouver des documents contenant une séquence de mots spécifique (ex: "Les Dents du Midi") dans l'ordre exact et non n'importe où dans le document.
- la possibilité de chercher dans des documents qui ont par exemple un titre et du texte, et donc de chercher soit dans le titre du document, soit dans le texte, soit dans les 2.
- la possibilité de pondérer (rank) différamment les documents selong qu'ils soient récents. C'est pas forcemment intéressant dans notre cas Wikipedia, mais très important par exemple pour un journal ("booster" les articles les plus récents).
- la recherche de documents contenant des mots proches, càd des mots qui ont une similarité sémantique, par exemple si on recherche un "laptop", on devrait aussi trouver des documents contenant des mots comme "ordinateur portable" ou "portable" ou même "ThinkPad".
- pouvoir mettre à jour en continu l'index, sans interrompre les services de recherche
- pouvoir _scaler_ au delà d'une machine, c'est à dire servir votre index à l'aide d'un cluster (ceci afin d'accomoder un trafic élevé, mais aussi d'assurer la résilience de votre système en cas de défaillance d'un noeud du cluster)

Réfléchissez en groupe à comment vous pourriez créer ces nouvelles fonctionaliés (sans les implémenter).
