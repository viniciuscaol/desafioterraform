A implantação do CRM foi um sucesso !!! Mas como se trata de uma aplicação crítica, foi definido que a infraestrutura precisaria suportar alta disponibilidade. Então faremos uma alteração na arquitetura do CRM adicionando redundância na solução e incluindo um load balancer na frente das máquinas de front end.

Segue abaixo o diagrama atualizado:



Todos os requisitos anteriores devem ser seguidos nessa solução também.

A solução deve ser entregue no repositório “Desafios Terraform” que você criou dentro do diretório /terraform-bronze/04-CRM-HA.