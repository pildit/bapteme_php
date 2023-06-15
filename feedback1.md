
1. On peut utiliser le meme template pour student add / update 
2. En checkAuthorization() on n'a pas besoin d'appeler exit()
3. les methodes qui interrogent la BD sont declarees static mais sont apellees sur un objet, comme par exemple :
```
   $newteacher = new Teacher();
   $teacherFromDb = $newteacher->find($teacherid);
```
Ca pourrait etre ecrit comme ca: 

```
  $teacherFromDb = Teacher::find($teacherid);
```    

4. On devrait utiliser camelCase pour variables, comme par exemple : 
    $teacherid => $teacherId 
5. On pourrait utiliser une couleur differente pour les profs/eleves desactives

7. Definir une fonction pour l'affichage d'un \<select> en template afin de ne pas repeter code , comme par exemple :
```
    function display_select(array $options, string $selected = null) 
```

J'ai rajoute un patch avec les modifs necessaires pour un fonctionnement correct du code, il y avait des anomalies au niveau de Student update et Teacher update 
