# Utilisation d'une image Python de base
FROM python:3.9-slim

# Définir le répertoire de travail
WORKDIR /app

# Copier le fichier requirements.txt
COPY requirements.txt .

# Installer les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Copier tous les fichiers du frontend dans le conteneur
COPY . /app/

# Exposer le port sur lequel ton app frontend va tourner
EXPOSE 5000

# Commande pour démarrer l'application
CMD ["python", "app.py"]
