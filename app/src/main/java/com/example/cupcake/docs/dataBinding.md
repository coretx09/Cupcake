# DATA BINDING
La bibliothèque [Data Binding] est une bibliothèque de support qui vous permet de lier des
[composants UI]  dans [layouts] à des [Data sourcse] dans votre application à l'aide d'un format déclaratif plutôt que par programmation.

# Layouts and binding expression:
Le langage d'expression vous permet d'écrire des expressions qui gèrent les événements distribués par les [views].

[Data binding layout] sont légèrement différents et commencent par une balise racine [layout] suivie 
d'un [data] élément et d'un [view] élément racine
Cet [view] est ce que serait votre racine dans un fichier de mise en page non contraignant.

[Expressions bindings] dans la mise en page sont écrites dans les propriétés d'attribut à l'aide de la [ @{}syntaxe " "]


# Listener bindings:
Ce sont des [Expressions bindings] qui s'exécutent lorsqu'un événement se produit. 


# Work with observable data objects
observable signifie que lorsque les données changent, l'interface utilisateur sera automatiquement mise à jour.
Il existe plusieurs façons de mettre en œuvre l'observabilité. Vous pouvez utiliser [observable classes, observable fields,]
ou, de préférence, [LiveData] .
LiveData est un observable sensible au [lifeCycle], vous devez donc spécifier le propriétaire du lifeCycle à utiliser:
  [ binding.lifecycleOwner = viewLifecycleOwner ]
