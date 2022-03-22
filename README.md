# doodlestudentdocker
TP de TLC.
Je suis arriver a la tache 6.
Normalement, le grafana est automatiquement connecter au prometheus grace au provisionning.
Mais je n'ai pas reussit a faire marcher l'import automatique de dashboard

### Notes :

Normalement, le lien pour acceder au server est 

slocketlc.(doodle | pad | monitor | phpmyadmin ).diverse-team.fr:(PORT)

Ou 
```
Port =  3000 - grafana (admin - changeme)
        8000 - front
        8081 - back
```
le fichier ect/host est changer pour cree un mini DNS qui redirige les addresses ci dessu en localhost (127.0.0.1)
