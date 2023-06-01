Agora, vamos pra última etapa.

Vamos criar a infraestrutura que vai receber o Wordpress.

Pra isso, a infraestrutura precisa dos seguintes elementos:

Uma VPC independente na Digital Ocean
Uma máquina virtual Linux com o Ubuntu e IP público para o Wordpress.
Um firewall pra proteger a máquina virtual com o Wordpress.
Um banco de dados MySQL
Segue abaixo o diagrama com a arquitetura:



Os requisitos que devem ser obedecidos são:

A imagem do sistema operacional das máquinas virtuais deve ser parametrizado
O size da máquina deve ser parametrizado
O size do banco de dados deve ser parametrizado
A região de toda a solução deve ser parametrizado
O acesso na máquina virtual vai ser feito utilizando SSH através da chave cadastrada na Digital Ocean (o nome da chave é crm-ssh) e o IP que vai ter acesso à máquina é o 239.13.117.114.
As portas que devem ser liberadas no firewall do Wordpress são apenas as portas HTTP (80), HTTPS (443), DNS (53) e a SSH (22) aceitando apenas o IP que será usado pra acesso.
O banco de dados só deve permitir o acesso da máquina virtual com o Wordpress.
A solução deve ser entregue no repositório “Desafios Terraform” que você criou dentro do diretório /terraform-bronze/02-Wordpress.