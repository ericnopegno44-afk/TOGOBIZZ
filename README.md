# TOGO BUSINESS — structure prête pour Mixx by Yas

Cette version contient un frontend, un backend PHP, un schéma MySQL et un endpoint webhook.

Yas indique officiellement proposer le paiement en ligne Mixx by Yas via une API sécurisée. Les URLs, paramètres, signatures et champs exacts ne sont pas inventés ici : ils doivent venir de la documentation et du compte marchand Yas.

## Installation
1. Héberger avec HTTPS et PHP.
2. Créer une base MySQL et importer `backend/database.sql`.
3. Copier `backend/config.example.php` vers `backend/config.php`.
4. Renseigner uniquement les paramètres officiels fournis par Yas.
5. Configurer le webhook/callback sur le serveur.
6. Tester en sandbox si Yas en fournit un.
7. Vérifier les signatures et statuts avant la production.

## Limite actuelle
`backend/payment.php` ne déclenche aucun paiement réel tant que le connecteur API officiel Yas n'est pas intégré.
