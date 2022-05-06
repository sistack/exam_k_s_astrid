# exam_k_s_astrid

Cours de K8S avec Arthur Escriou (examen du 6 mai 2022)
Les fichiers de déploiement utilisés pour l'examen:
astnoderedis.yaml
astriddeployredis.yaml
astridservice.yaml
astridnodeservice.yaml
Pour déployer le serveur node-redis sur un pod on va utiliser le fichier : astnoderedis.yaml grâce à la commande: 
$ kubectl apply -f astnoderedis.yaml
Pour déployer redis sur 3 pods différents de l'application redis. 
$ kubectl apply -f astriddeployredis.yaml
On déploie le service astridservice afin que les applications redis puissent communiquer avec le cluster
$ kubectl apply -f astridservice.yaml
On déploie le service astridnodeservice afin que le serveur puisse parler avec les autres pods du cluster
$ kubectl apply -f astridnodeservice.yaml
