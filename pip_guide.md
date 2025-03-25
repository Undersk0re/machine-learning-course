# come usare pip (linux version)

- pulire la cache dei pacchetti pip
`pip cache purge`


- creare un virtual environment per i pacchetti necessari al progetto (verrà creata una cartella)
`python3 -m venv .venv` 


- abilitare il virtual environment
`source .venv/bin/activate`

- disabilitare il virtual environment (att.ne pip onstallerà tutto nel sistema host)
`deactivate`


- installare i requirement per un progetto, nel venv che si vuole (sistema o dedicato)
`pip install -r requirements.txt`

- salvare i requirements se modificati
`pip freeze > requirements.txt`

- forzare installazione dei pacchetti nei requirements
`pip install --force-reinstall --no-deps --no-cache-dir -r requirements.txt`


## nota requirements.txt

nel file `requirements.txt` abbiamo requirements compatibili con google-colab, dovrebbe essere possibile portare quasi tutti i files in questo archivio su collab installando solo poche dipendenze.
