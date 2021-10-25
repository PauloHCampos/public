# Comandos Uteis.

```

## Service Principal

Criar: az ad sp create
Listar: az ad sp list --filter "displayname like 'aks'"
Mostrar especifico: az ad sp show --id 

az ad app list --query "[?contains(displayName,'aks')] | [].displayName" -o table

az ad app list --query "displayName eq $SPNAME" | [].displayName" -o tsv

az ad sp list --query "[?contains(displayName,'aks')] | [].displayName" -o table

