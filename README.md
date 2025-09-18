# Exercice 3 – Modification du site HTML

Cet exercice montre comment mettre à jour un site statique déjà déployé sur OpenShift.

## Contenu modifié

Le fichier `index.html` devient :

```html
<!DOCTYPE html>
<html>
  <head><title>Site OpenShift Modifié</title></head>
  <body>
    <h1 style="color:blue;">Bienvenue sur mon site HTML modifié</h1>
    <p style="color:green;">Ajout d’un paragraphe</p>
  </body>
</html>
-----------------------------------

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
