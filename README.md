`sudo apt install python3-venv`
`python3 -m venv venv` 
`source venv/bin/activate`

`ansible-galaxy collection install -r requirements.yml`

## export DB_PASSWORD=$(kubectl get secret --namespace default postgres-db-2-postgresql -o jsonpath="{.data.postgres-password}" | base64 -d) ## if you are using K8 postrgres

export DB_PASSWORD=<your DB password>

