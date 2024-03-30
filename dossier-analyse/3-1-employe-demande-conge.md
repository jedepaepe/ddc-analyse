# demande congé
En tant qu'employé, je veux pouvoir demander congé, ainsi tout le monde peut s'organiser (je peux organiser sereinement mes congés, mon manager peut organiser son planning, mon entreprise peut vérifier les congés).

## Scénario
### Préconditions
L'employé est authentifié.

(Si l'employé, n'est pas authentifié, il est redirigé vers la page d'authentification).

### Scénario 1 - happy flow
- l'employé complète le formulaire de demande de congé avec:
    - la date de début de congé (obligatoire)
    - la date de fin de congé (obligatoire)
    - le type de congé (obligatoire)
    - une raison (non obligatoire)
- l'application affiche le solde de congé sans et avec la demande
- l'employé envoie la demande (il peut bien entendu annuler sa demande)
- l'application envoie un email de notification à son manager contenant:
    - le matricule de l'employé
    - son prénom
    - son nom de famille
    - la date de début
    - la date de fin
    - le type de congé
    - la raison
    - le solde de congé de l'employé
    - un lien vers la demande
- l'application envoie un email de confirmation à l'employé contenant les mêmes informations

#### Postconditions
- la demande de congé est enregistrée
- l'email de notification est posté dans la mailbox du manager
- l'email de confirmation est posté dans la mailbox de l'employé

#### Règles métier
- la date de fin de congé est plus grande ou égale à la date de début de congé

### Scénario 2 - plus de solde de congé
Comment gérer un tel cas ?



