Utilisateurs
============

Rôles des utilisateurs
----------------------

Rôles au niveau de l’application
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Chaque utilisateur possède un de ces rôles :

+----------+-----------------------------------------------------------+
| Rôle     | Description                                               |
+==========+===========================================================+
| Administ | Accès à tout                                              |
| rateur   |                                                           |
+----------+-----------------------------------------------------------+
| Gestionn | Peut créer des projets d’équipe mais ne peut pas changer  |
| aire     | les réglages de l’application                             |
+----------+-----------------------------------------------------------+
| Utilisat | Peut créer des projets privés                             |
| eur      |                                                           |
+----------+-----------------------------------------------------------+

Rôles au niveau des projets
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Chaque membre d’un projet peut avoir un rôle différent :

+-----------------+----------------------------------------------------+
| Rôle            | Description                                        |
+=================+====================================================+
| Chef de projet  | Peut changer les paramètres du projet, accéder aux |
|                 | rapports                                           |
+-----------------+----------------------------------------------------+
| Membre du       | Peut créer des tâches et utiliser le tableau       |
| projet          | Kanban                                             |
+-----------------+----------------------------------------------------+
| Visualiseur de  | Accès en lecture seule au projet                   |
| projet          |                                                    |
+-----------------+----------------------------------------------------+

Il est également possible de créer des rôles personnalisés pour
appliquer des restrictions supplémentaires sur les utilisateurs.

Ajouter un nouvel utilisateur
-----------------------------

Pour ajouter un nouvel utilisateur, vous devez être administrateur.

1. Depuis le menu déroulant situé en haut à droite, cliquez sur
   **Gestion des utilisateurs**
2. Dans la partie haute vous avez un lien **Créer un utilisateur local**
   ou **Créer un utilisateur distant**
3. Informez les champs de saisie et enregistrez

.. figure:: /_static/new-user.png
   :alt: Nouvel utilisateur

Quand vous créez un **utilisateur local**, vous devez préciser au moins
deux valeurs :

-  **nom d’utilisateur** : c’est l’identifiant unique de votre
   utilisateur (login)
-  **mot de passe** : le mot de passe de votre utilisateur doit
   comporter au moins 6 caractères

Pour les **utilisateurs distants**, seul le nom d’utilisateur est
obligatoire.

Modifier des utilisateurs
-------------------------

Quand vous allez au menu **utilisateurs**, vous disposez d’une liste
d’utilisateurs. Pour modifier un utilisateur cliquez sur le lien
**Modifier**.

-  si vous êtes un utilisateur ordinaire, vous ne pouvez modifier que
   votre propre profil
-  vous devez être administrateur pour pouvoir modifier n’importe quel
   utilisateur

Supprimer des utilisateurs
--------------------------

Depuis le menu **utilisateurs**, cliquez sur le lien **supprimer**. Ce
lien n’est visible que si vous êtes administrateur.

Si vous supprimez un utilisateur particulier, **les tâches assignées à
cette personne ne lui seront plus assignées** après cette opération.

Authentification à deux facteurs
--------------------------------

Chaque utilisateur peut activer `l’authentification à deux
facteurs <http://en.wikipedia.org/wiki/Two_factor_authentication>`__.
Après s’être connecté, un code à usage unique (6 caractères) est demandé
à l’utilisateur pour lui autoriser l’accès à Kanboard.

Ce code doit être fourni par un logiciel compatible, généralement
installé sur votre smartphone.

Kanboard utilise le `Time-based One-time Password
Algorithm <http://en.wikipedia.org/wiki/Time-based_One-time_Password_Algorithm>`__
défini dans la `RFC 6238 <http://tools.ietf.org/html/rfc6238>`__.

Il existe de nombreux logiciels compatibles avec le standard TOTP
system. Par exemple, vous pouvez utilisez ces applications libres et
open source :

-  `Google
   Authenticator <https://github.com/google/google-authenticator/>`__
   (Android, iOS, Blackberry)
-  `FreeOTP <https://freeotp.github.io/>`__ (Android, iOS)
-  `OATH Toolkit <http://www.nongnu.org/oath-toolkit/>`__ (utilitaire en
   ligne de commande sur Unix/Linux)

Ce système peut fonctionner hors ligne et vous n’avez pas l’obligation
d’avoir un téléphone portable.

Paramétrage
~~~~~~~~~~~

1. Allez dans le profil utilisateur.
2. Sur la gauche, cliquez sur **Authentification à deux facteurs** et
   cochez la case.
3. Une clef secrète est générée pour vous.

.. figure:: /_static/2fa.png
   :alt: 2FA

-  Vous devez sauvegarder votre clef dans votre logiciel TOTP. Si vous
   utilisez un smartphone, la solution la plus simple est de scanner le
   QR code avec FreeOTP ou Google Authenticator
-  À chaque ouverture de session, un nouveau code sera demandé
-  N’oubliez pas de tester votre appareil avant de quitter votre session

Une nouvelle clef est générée à chaque fois que vous activez/désactivez
cette fonction
