# SHARED VIEW MODEL
La principale différence dans l'implémentation d'un [shared view model]  est la façon dont nous y 
accédons à partir des contrôleurs UI.
Vous utiliserez [activity instance]  au lieu de [fragment instance] 

# activityViewModels()
[viewModels()] vous donne le ViewModel instance étendue au fragment . 

[activityViewModels()] vous donne le ViewModel instance étendue à activity .

# delegation 
La delegation de propriété dans Kotlin vous aide à transférer la responsabilité du getter-setter à une autre classe.

Une propriété déléguée est définie à l'aide de la [by] clause et d'une instance de classe déléguée :

# Date formatter
Le framework Android fournit une classe appelée SimpleDateFormat, qui est une classe pour le 
formatage et l'analyse des dates d'une manière sensible aux paramètres régionaux. I
Vous pouvez créer une instance de[SimpleDateFormat()] en transmettant une chaîne de modèle et un paramètre régional 
[SimpleDateFormat("E MMM d", Locale.getDefault())]
la chaîne de modèle est ["EEE, MMM d"] analysée en ["Wed, Jul 4"]

# Operator Elvis ( ?: )
[quantity.value ?: 0]
signifie que si l'expression de gauche n'est pas nulle, alors utilisez-la. Sinon, si l'expression à
gauche est nulle, utilisez l'expression à droite de l'opérateur elvis

# Set Lifecycle owner to observe LiveData
[LifecycleOwner] est une classe qui a un lifecycle Android, comme une activité ou un fragment.
[LiveData]observer observe les modifications apportées aux data de l'app uniquement si le owner du lifecycle est dans des états actifs ( STARTED ou RESUMED).
[LiveData]observers sont les  binding expressions in layout files avec les data observable comme  price
Avec [Data Binding], lorsqu'une valeur observable change, les éléments UI  auxquels elle est liée sont automatiquement mis à jour.
For the UI elements to automatically update, you have to associate [binding.lifecycleOwner]
 
#LiveData transformation
La LiveData ou les méthodes de transformation permettent d'effectuer des manipulations de données sur
la source LiveData et de renvoyer un LiveData objet résultant. 
En termes simples, il transforme la valeur de LiveData en une autre valeur. 

[Transformations.map()]est l'une des fonctions de transformation, cette méthode prend la source LiveData et une fonction comme paramètres
Quelques exemples en temps réel où vous pouvez utiliser une transformation LiveData :
1. Formater les chaînes de date et d'heure pour l'affichage
2. Trier une liste d'éléments
3. Filtrer ou regrouper les éléments
4. Calculez le résultat à partir d'une liste telle que la somme de tous les éléments, le nombre d'éléments, renvoyez le dernier élément, etc.

#Setup click listeners using listener binding

#Implement Up button behavior

# tasks and back stack:
[Task] Les activités dans Android existent dans les task
Lorsque vous ouvrez une application pour la première fois à partir de l'icône du lanceur, Android crée une nouvelle task avec votre activité principale.
Une task est un ensemble d'activités avec lesquelles l'utilisateur interagit lors de l'exécution d'un certain travail

[back stack]
Les activités sont organisées dans une back, appelée  , back stack où chaque nouvelle activité visitée par l'utilisateur est poussée sur la back stack pour la task.
Les activités en dessous sur la pile ont été mises en arrière-plan et ont été arrêtées.
La back stack est utile lorsque l'utilisateur veut naviguer vers l'arrière. Android peut supprimer l'activité en cours du haut de la pile, la détruire et recommencer l'activité en dessous.
Lorsqu'il n'y a plus d'activités dans le backstack, l'utilisateur est ramené à l'écran de lancement de l'appareil