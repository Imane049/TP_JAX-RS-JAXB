# JAX-RS-Jersey


Vidéo de Démonstration

Pour une démonstration complète, veuillez consulter la vidéo suivante : 


[assets/Project 2.mp4
](https://github.com/Imane049/TP_JAX-RS-JAXB/blob/main/assets/Project%202.mp4)

1. Récupérer tous les comptes
curl -X GET "http://localhost:8082/banque/comptes" -H "Accept: application/xml"
2. Récupérer un compte par ID
curl -X GET "http://localhost:8082/banque/comptes/1" -H "Accept: application/xml"

3. Ajouter un compte
curl -X POST "http://localhost:8082/banque/comptes" -H "Content-Type: application/xml" -d '<?xml version="1.0" encoding="UTF-8"?>
<compte>
    <solde>1000.0</solde>
    <dateCreation>2024-01-01</dateCreation>
    <type>EPARGNE</type>
</compte>'

4. Mettre à jour un compte existant
curl -X PUT "http://localhost:8082/banque/comptes/1" -H "Content-Type: application/xml" -d '<?xml version="1.0" encoding="UTF-8"?>
<compte>
    <solde>1500.0</solde>
    <dateCreation>2024-01-01</dateCreation>
    <type>EPARGNE</type>
</compte>'

5. Supprimer un compte
curl -X DELETE "http://localhost:8082/banque/comptes/2"

