# 5th Module on the labs order, 301-T03A Mod3 Exercise Outputs and fixes. 

# Cleanup command after the Lab 5 down below
az group list --query "[?starts_with(name,'AADesignLab05')]".name --output tsv | xargs -L1 bash -c 'az group delete --name $0 --no-wait --yes'

