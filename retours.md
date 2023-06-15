1. 🟡 Des Choses à Travailler 
2.  🟠 Insuffisant pour Valider
3. 🟠 Insuffisant pour Valider
4. 🔴 Non Rendu ou Très Insuffisant

Quelques remarques valables pour toutes les solutions : 

- Quand on utilise PDO il faut passer par des "prepared statements" afin  d'etre sure que les parametres soient bien escapes. je vois qu'il y a quand meme une exception a ca, 
quand on supprime un etudiant (Student->delete())

- Les definitions de routes peuvent etre mises dans un fichier separe.



