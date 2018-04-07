Suivi du temps
==============

Les informations de la feuille de suivi du temps peuvent être définies
au niveau des tâches ou des sous-tâches

Suivi de temps des tâches
-------------------------

.. figure:: /_static/task-time-tracking.png
   :alt: Suivi de temps des tâches

Les tâches ont deux champs:

-  Temps estimé
-  Temps passé

Ces valeurs représentent des heures de travail et doivent être entrées
manuellement.

Suivi de temps des sous-tâches
------------------------------

.. figure:: /_static/subtask-time-tracking.png
   :alt: Suivi de temps des sous-tâches

Les sous-tâches ont aussi les champs “temps passé” et “temps estimé”

Lorsque vous changez la valeur de ces champs, **le suivi des tâches est
mis à jour automatiquement et devient la somme des sous-tâches**.

Kanboard enregistre le temps entre chaque changement de statut des
sous-tâches dans une table séparée

-  Changer le statut de la sous-tâche de **à faire** à **en cours**
   marque le temps de début
-  Changer le statut de la sous-tâche de **en cours** à **à faire**
   marque le temps de fin mais aussi met à jour le temps passé sur la
   sous-tâche et la tâche

La répartition de tous les enregistrements est visible sur la page de la
tâche

.. figure:: /_static/task-timesheet.png
   :alt: Feuille de suivi du temps pour les tâches

Pour chaque sous-tâche, le chrono peut être à tout moment arrêté/démarré

.. figure:: /_static/subtask-timer.png
   :alt: Chrono des sous-tâches

-  Le chrono ne dépend pas du statut de la sous-tâche
-  Chaque fois que vous démarrez le chrono, un nouvel enregistrement est
   créé dans la table de suivi des temps
-  Chaque fois que vous arrêtez l’horloge, la date de fin est
   enregistrée dans la table de suivi des temps
-  Le temps passé est arrondi au quart d’heure le plus proche (seulement
   pour Kanboard < 1.0.32)
