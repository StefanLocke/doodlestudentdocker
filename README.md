# doodlestudentdocker
TP de TLC.
Je suis arriver a la tache 6.
Normalement, le grafana est automatiquement connecte au prometheus grace au provisionning.
Mais je n'ai pas reussit a faire marcher l'import automatique de dashboard

### Notes :

Normalement, le lien pour acceder au server est 
```
slocketlc.(doodle | pad | monitor | phpmyadmin ).diverse-team.fr:(PORT)
```
Ou 
```
Port =  3000 - grafana (admin - changeme)
        8000 - front
        8081 - back
```
le fichier ect/host est changer pour cree un mini DNS qui redirige les addresses ci dessu en localhost (127.0.0.1)

Ce qui a ete implementer : 
        le back quarkus
        le front, utilisant bunkerized NGINX
        la BDD + PHPMyAdmin
        le Etherpad
        Service de Mail
        Monitoring avec Prometheus + granfana
        
Tout cela est lancer avec un simple docker-compose up, qui est dans le fichier Compose
        
        
