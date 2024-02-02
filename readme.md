1. ¿Qué comando utilizaste en el paso 11? ¿Por qué? 
Git reset --hard HEAD^ . Git reset sería la operación, hard el modo, es decir, que se borre todo incluidos los cambios en la working area y HEAD^, que indica el commit al que volver, es decir, el inmediatamente anterior al que borramos.
2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 
Utilizo git reflog para ir a historial, copio el hash y con git reset - - hard + el hash vuelvo a ese commit y lo recupero.
3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 
No causa ningún conflicto, aunque al hacer git checkout me indica que hay diferencias entre ambas ramas.
4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
Si hay conflicto. Porque cada archivo está formateado de manera diferente.
5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
No causó ningún conflicto. Porque no había archivos en conflicto.
6. ¿Qué comando o comandos utilizaste en el paso 25? 
git log --graph
7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
Si, porque solo tiene que avanzar para absorber a title
8. ¿Qué comando o comandos utilizaste en el paso 27? 
git reset - - soft HEAD^ para mantener los cambios del working copy
9. ¿Qué comando o comandos utilizaste en el paso 28? 
git checkout - - .
10. ¿Qué comando o comandos utilizaste en el paso 29? 
git branch -D title
11. ¿Qué comando o comandos utilizaste en el paso 30? 
git reflog, copio el hash, git reset, git checkout + hash
12. ¿Qué comando o comandos usaste en el paso 32? 
git reflog, copio el hash, git reset + hash
13. ¿Qué comando o comandos usaste en el punto 33? 
copio el hash (que lo tenia arriba de haber hecho reflog antes), git reset + hash