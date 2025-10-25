# Utiliser une image de base pytorch
FROM pytorch/pytorch

# Créer un répertoire de travail
WORKDIR /app

# Copier tous les fichiers dans le workdir
COPY requirements.txt /app 

# Installer wget et unzip
RUN apt-get update && apt-get install -y wget unzip

# Installer les dépendances manquantes
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Exposer le port pour le notebook
EXPOSE 8888
