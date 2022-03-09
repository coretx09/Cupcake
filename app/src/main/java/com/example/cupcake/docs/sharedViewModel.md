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
