#Docker y terraform

Instalacion de Terraform


```
wget -O- https://apt.releases.hashicorp.com/gpg | gpg --dearmor | sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform

```{{execute}}

Inicializando Terraform

` cd /root && terraform init `{{execute}}

Plan Terraform

`terraform plan`{{execute}}`

Apply Terraform

`terraform apply --auto-approve`{{execute}}



