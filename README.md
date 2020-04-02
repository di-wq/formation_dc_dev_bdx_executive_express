Instructions d'installation
======================

#Windows
1. Installer Git https://gitforwindows.org/
2. Installer NodeJS https://nodejs.org/en/download/
3. Cloner le projet :
    1. Se rendre sur github.com
        1. Se connecter
        2. Fork le projet `Dylfaen/formation_dc_dev_bdx_executive_express`
    2. Cloner le projet forké sur votre compte depuis github
4. lancer la commande `npm install` dans le répertoire du projet dans `node_src/`
5. Installer mongoDB https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/
6. Lancer la commande en mode administrateur `"C:\Program Files\MongoDB\Server\4.2\bin\mongo.exe"`
7. Lancer MongoDB compass et se connecter au server mongoDB avec `mongodb://127.0.0.1:27017/?compressors=zlib&gssapiServiceName=mongodb`
8. Créer un ficher dans `node_src` nommé `config.js` contenant le code suivant 
```
module.exports = {
    mongodb: {
        url: "mongodb://127.0.0.1:27017",
    },
    port: "3001"
}
```
8. lancer `npm start` dans `node_src/`


#Linux et MacOS
1. Installer docker et docker-compose
2. Se rendre sur github.com
    1. Se connecter
    2. Fork le projet `Dylfaen/formation_dc_dev_react_node`
3. Installer git
4. Cloner votre projet
5. Créer un ficher dans `node_src` nommé `config.js` contenant le code suivant 
```
module.exports = {
    mongodb: {
        url: "mongodb://mongo:27017",
    },
    port: "3001"
}
```
6. Dans le répertoire du projet lancer `sudo docker-compose up`
7. Le server node sur `localhost:3001`





