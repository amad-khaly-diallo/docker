# Dockerfile pour le backend

# 1 Image de base Node.js
FROM node:20-alpine

# 2 Répertoire de travail
WORKDIR /usr/src/app

# 3 Copie package.json et package-lock.json (à créer)
COPY package*.json ./

# 4 Installation des dépendances
RUN npm install --production

# 5 Copie du code backend
COPY . .

# 6 Expose le port
EXPOSE 3000

# 7 Commande pour lancer le serveur
CMD ["node", "server.js"]
