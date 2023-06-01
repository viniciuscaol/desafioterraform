Criar uma infraestrutura simples para a aplicação de monitoramento dos assuntos no Twitter. 
Essa infraestrutura tem os seguintes requisitos:

Uma VPC independente na Digital Ocean
Uma máquina virtual Linux com o Ubuntu e IP público
Um firewall pra proteger a máquina virtual
Segue abaixo o diagrama com a arquitetura:



Alguns requisitos que devem ser obedecidos:

A imagem do sistema operacional da máquina virtual deve ser parametrizado
O size da máquina deve ser parametrizado
A região de toda a solução deve ser parametrizado
O acesso na máquina virtual vai ser feito utilizando SSH através da chave cadastrada na Digital Ocean 
(o nome da chave é twitter-ssh) e o IP que vai ter acesso à máquina é o 239.13.117.114.
As portas que devem ser liberadas no firewall são apenas as portas HTTP (80), HTTPS (443), DNS (53) e a SSH (22) 
aceitando apenas o IP que será usado pra acesso.
A solução deve ser entregue no repositório “Desafios Terraform” que você criou dentro do diretório 
/terraform-bronze/01-Twitter_Trends_Scan.