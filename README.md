# Terraform com Ansible na AWS
<div>
    <a href="https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ansible/ansible-original.svg" width="30" height="30" align="center"/>
    </a>
    <a href="https://www.terraform.io/">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/terraform/terraform-original.svg" width="30" height="30" align="center"/>
    </a>
    <a href="https://aws.amazon.com/pt/?nc2=h_lg">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-plain-wordmark.svg" width="30" height="30" align="center" />
    </a>
</div>


## Neste projeto foi utilizado:
- Terraform para criação de instância EC2 na AWS;
- Ansible para criação do ambiente em python com django;
- AWS para a criação da conta e autenticação com o provider via aws configure.

## Fundamentos de Infraestrutura como Código (IaC) 
### O que podemos resolver com IaC?

- Versionamento de sistemas
- Uso de virtualização 
- Automatização de processos manuais podendo ter um menor erro na montagem de ambiente
- Ambientes idênticos evitando o famoso "Na minha máquina funciona!"
- Deploy Automatizado
- Melhor implementação de CI/CD
- Velocidade e segurança
- Reuso
- Idempotência
- Escrita e execução de código para: Definir, Implantar, atualizar e Gerenciar nossa infra.
### Principais Ferramentas

- Terraform 
- Crossplane
- Puppet
- Ansible
- Chef
- Kubernetes

## Instalação das ferramentas no Ubuntu

### Ansible


 - `sudo apt update`
 - `sudo apt install software-properties-common`
 - `sudo add-apt-repository --yes --update ppa:ansible/ansible`
 - `sudo apt-get install ansible`


### Terraform
`
wget -O- https://apt.releases.hashicorp.com/gpg | \
gpg --dearmor | \
sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg
`
### AWS Configure

Use o site da AWS para executar esse passo:
https://docs.aws.amazon.com/pt_br/cli/latest/userguide/getting-started-install.html

## Principais Comandos utilziados nas ferramentas:
### Terraform:
- `terraform init `
- `terraform plan `
- `terraform apply `

### Ansible:
`ansible-playbook playbook.yaml -u ubuntu --private-key <secret.pem> -i hosts.yaml`
