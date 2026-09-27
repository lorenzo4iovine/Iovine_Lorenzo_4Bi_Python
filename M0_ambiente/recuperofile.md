@lorenzo4iovine ➜ /workspaces/Iovine_Lorenzo_4Bi_Python (main) $ touch M0_ambiente/temporanei/nota.txt M0_ambiente/temporanei/dati.tmp
git add M0_ambiente/temporanei
@lorenzo4iovine ➜ /workspaces/Iovine_Lorenzo_4Bi_Python (main) $ git commit -m "test: aggiunge per errore la cartella temporanei"
[main 10df5f8] test: aggiunge per errore la cartella temporanei
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 M0_ambiente/temporanei/nota.txt
@lorenzo4iovine ➜ /workspaces/Iovine_Lorenzo_4Bi_Python (main) $ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

# Recupero di file versionati per errore

## Sequenza dei comandi eseguiti
```bash
# Creo la cartella e i file di prova
mkdir M0_ambiente/temporanei
touch M0_ambiente/temporanei/nota.txt M0_ambiente/temporanei/dati.tmp

# Li aggiungo a Git per sbaglio
git add M0_ambiente/temporanei
git commit -m "test: aggiunge per errore la cartella temporanei"

# Inserisco la regola nel .gitignore
echo "M0_ambiente/temporanei/" >> .gitignore

# Rimuovo la cartella dall'indice di Git senza cancellarla dal computer
git rm -r --cached M0_ambiente/temporanei

# Salvo la modifica nel commit
git add .gitignore
git commit -m "fix: rimuove la cartella temporanei dal tracciamento di git"