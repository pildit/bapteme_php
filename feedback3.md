
- erreur dans les templates : il faut les "decouper" en header, footer comme les autres apprenants l'ont fait 
- le URL racine "/" n'etait pas bien renseigne 
- les liens dans le header ne fonctionnent pas, il faudrait utiliser `$router->generate('teacher_list')` au lieu d'avoir des liens hardcodes
- en student_add_tpl.php : faut pas mettre des valeurs hard-codes, mais une liste de la DB 
- Student model : il manque les get/set TeacherId()  methods

