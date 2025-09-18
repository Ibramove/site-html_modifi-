# Déploiement sur OpenShift

# 1.Relancer un build avec le nouveau code :

oc start-build site-html --from-dir=. --follow


# 2. Vérifier le déploiement :

oc get pods
oc get route


# 3. Tester dans le navigateur ou avec curl :

curl http://<URL_de_route>


La page mise à jour s’affiche avec :

<img width="3483" height="1532" alt="image" src="https://github.com/user-attachments/assets/b6d56a84-b20a-4a3e-bb54-02c70cefedf7" />
