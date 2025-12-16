FROM cosminbilga/welcome-to-docker:latest

# Copier ton code modifié
COPY ./src ./src
COPY ./public ./public
COPY package*.json ./

# Installer, build et nettoyer
RUN npm install \
    && npm install -g serve@latest \
    && npm run build \
    && rm -fr node_modules

EXPOSE 3000
CMD ["serve", "-s", "build"]
