### Créer un projet vue js nommé vue-router
### Créer les composants : 
* ListPays.vue
* PageConnexion.vue
* TodoList.vue

### Mettre en place le route à l'aide d'un objet et de "meta composant" de VueJs
lien : https://vue3-fr.netlify.app/api/built-in-components.html#component

déclaration d'une variable réactive pour stocker le composant à afficher par défaut : 

Dans le mesure où un composant n'est pas une variable ordinaire, il se produit une surchage de performance. La surcharge de performance survient lorsque Vue essaie de rendre réactif quelque chose qui n'en a pas besoin, comme un composant. Dans ce cas, on peut utiliser `shallowRef` : Contrairement à ref, `shallowRef` crée une référence réactive, mais seulement pour la valeur principale elle-même, sans surveiller les changements à l'intérieur de cette valeur. Par exemple, si tu utilises `shallowRef` pour un objet, Vue détectera uniquement quand l'objet entier change, mais pas si des détails à l'intérieur de l'objet changent. Cela signifie que si l'objet est un composant Vue, Vue ne suivra pas les changements à l'intérieur du composant, ce qui empêche une surcharge de performance.

* const componentName = ref(markRaw(TodoList));



### Révision pour tous : 
* Mise en place de la TodoList avec les fonctionnalités suivantes : 
1. Ajout
2. Suppression
3. Marquer comme terminé
4. Modifier 

* Composant ListPays : 
Récupération des données et affichage sur la vue dans des vignettes avec des informations simples

* Composant PageConnexion :
Mettre en place un formulaire de connexion