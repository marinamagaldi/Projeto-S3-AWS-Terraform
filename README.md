# Criação de um bucket S3 usando o Terraform

# Configuração inicial para esse laboratório:
    - Conta na AWS: https://aws.amazon.com/pt
        - Em Gerenciamento de Acesso, criar novo usuário com permissões de administrador.
        - Em Credenciais de Segurança, criar as senhas de acesso e guardá-las bem.
        - Importante: Logar na console da AWS com o usuário criado para iniciar o lab.
    - Para esse projeto utilizei o terminal WSL Ubuntu no VSCode em máquina Windows.


1- Criação de diretório para o projeto.

2- Iniciar um novo projeto Terraform.
        executar o comando no terminal: terraform init
        
3- Criar um novo arquivo de configuração
        arquivo: main.tf
Nesse arquivo consta a definição do provedor AWS e recurso do bucket S3.

4-  No terminal executar os comandos:
        terraform fmt: utilizado para formatar automaticamente os arquivos de configuração do Terraform.

        terraform validate: utilizado para validar a sintaxe e a semântica dos arquivos de confirguração do Terraform.

        export AWS_ACCESS_KEY_ID="chave de acesso"

        export AWS_SECRET_ACCESS_KEY="chave secreta"

        terraform plan: utilizado para criar um plano de execução no Terraform.
            -> mostrará uma mensagem com as configurações a serem aplicadas: terraform apply -> yes

As configurações serão criadas e aplicadas automaticamente no console da AWS.

5- Para excluir, executar o comando:
        terraform destroy.
