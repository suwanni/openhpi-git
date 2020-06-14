# Git Beispiele

## Git Lokal/Remote Repository auf einem Rechner
Im folgenden Beispiel werden die beiden Repositories in gleichen Verzeichnis
angelegt.


### Remote Repository anlegen

    git init --bare repoRemote.git

### Lokales Repository anlegen

    git init repoLocal
    cd repoLocal

### Lokales Repository mit dem Remote Repository verknüpfen

    git remote add origin /home/maro/develop/gitrepos/openHPI/repoRemote.git

