# Récupération de l'image
FROM node:8.11-alpine

# Copie du code dans le container
COPY . /app

# Installation du Node Package Manager à la création
RUN cd /app && npm install

# Précision du chemin de l'application
WORKDIR /app

# On expose un port pour la communication
EXPOSE 3000

# Commande à lancer au lancement du container
CMD ["npm", "start"]
