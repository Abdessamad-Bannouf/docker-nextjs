# NextJS (node lts alpine) Docker

# Installation du projet :

    ● Cloner le projet : git clone https://github.com/Abdessamad-Bannouf/docker-nextjs.git

    ● Lancer la commande : docker-compose build

    ● Lancer la commande : docker-compose up -d


# Connexion à l'application web :

    ● Aller sur l'adresse : http://localhost:3500


# Persistance de données :

    Pour la persistance de données j'ai mis en place l'ORM Prisma.

    Pour écrire vos scripts de migrations ça se passe dans le dossier prisma, plus précisément sur le fichier schema.prisma
    
    ● Lancer la commande : docker exec -it job-board-api bash

    ● Se rendre dans le dossier prisma (cd prisma)

    ● Editer le fichier schema.prisma et lancer la commande pour migrer les données en bdd : npx prisma migrate dev --name test

