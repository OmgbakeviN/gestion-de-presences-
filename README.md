# Gestion des Présences

Un projet Django permettant de gérer les présences des étudiants d'une manière simple et efficace. Il inclut la génération automatique de rapports journaliers et mensuels.

## Fonctionnalités

- **Page sécurisée** : Accès au site via un mot de passe unique.
- **Gestion des filières et étudiants** : Ajout et modification des données via l'interface admin de Django.
- **Enregistrement des présences** : Système de cases à cocher pour marquer les étudiants comme présents ou absents.
- **Génération de PDF** :
  - Liste des présences et absences journalières.
  - Rapport mensuel avec le total des présences et absences par étudiant.
- **Réinitialisation des données de présence**.

## Prérequis

- Python 3.x
- Django 4.x ou supérieur
- Bibliothèque `reportlab` pour la génération des PDF.

## Installation

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/username/gestion-presences.git
   cd gestion-presences
   ```

2. Installez les dépendances :
   ```bash
   pip install -r requirements.txt
   ```

3. Appliquez les migrations :
   ```bash
   python manage.py migrate
   ```

4. Lancez le serveur de développement :
   ```bash
   python manage.py runserver
   ```

5. Accédez au site via [http://127.0.0.1:8000](http://127.0.0.1:8000).

## Utilisation

### Accès à l'interface admin
1. Créez un superutilisateur :
   ```bash
   python manage.py createsuperuser
   ```
2. Connectez-vous à l'interface admin via [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin).
3. Ajoutez les filières et étudiants.

### Enregistrement des présences
1. Sélectionnez une filière sur la page principale.
2. Marquez les étudiants comme présents ou absents.
3. Enregistrez les présences pour générer automatiquement un PDF.

### Rapport mensuel
1. Cliquez sur le bouton **Rapport mensuel** dans la page de gestion d'une filière.
2. Téléchargez le fichier PDF généré.

## Contribuer

Les contributions sont les bienvenues ! Pour signaler un problème ou proposer une amélioration, ouvrez une issue ou soumettez une pull request.

---

## Auteurs

- **Kevin** - Développeur principal

---

## Licence

Ce projet est sous licence MIT. Consultez le fichier [LICENSE](LICENSE) pour plus de détails.
