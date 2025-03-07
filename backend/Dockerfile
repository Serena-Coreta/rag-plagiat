# Utilisation de l'image python:3.9-slim comme image de base
FROM python:3.9-slim

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le fichier requirements.txt dans le conteneur
COPY requirements.txt .

# Installer les dépendances à partir du fichier requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copier le reste de l'application dans le conteneur
COPY . .

# Définir le port que le conteneur va exposer
EXPOSE 8000

# Commande pour démarrer l'application
CMD ["python", "app.py"]
