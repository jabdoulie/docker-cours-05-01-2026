# Image Node.js officielle
FROM node:20-alpine

# Dossier de travail
WORKDIR /app

# Copier les fichiers de dépendances
COPY package.json package-lock.json ./

# Installer les dépendances
RUN npm install

# Copier le reste du code
COPY . .

# Exposer le port Angular
EXPOSE 4200

# Lancer le serveur Angular
CMD ["npx", "ng", "serve", "--host", "0.0.0.0", "--port", "4200"]
