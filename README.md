# TypeGraphQL + TypeORM + TypeScript

## Installation & Run

1- Créer la base de données dans MYSQL

CREATE SCHEMA trainingdb ;

2- Configuration du fichier .env

Voir fichier ".env.example"

3- Commande pour générer une migration :

(après avoir créer le script suivant dans le package.json : "typeorm:cli": "ts-node ./node_modules/typeorm/cli")

```sh
npm run typeorm:cli -- migration:generate -n +"nom de votre migration"
```

(ex : "npm run typeorm:cli -- migration:generate -n InitDataBase" => création de la migration nommée InitDataBase)

4- Commande pour lancer la migration :

```sh
npm run typeorm:cli -- migration:run
```

5- Lancement du serveur :

```sh
npm start
```

## Use it as a starter

Just create your own models in the `src/models` folder and your resolvers in `src/resolvers` to create your API!
