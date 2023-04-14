# REDES E ENTREGAS DE CONTEÚDO:

VPC
Seção que agrupam recursos com base nas necessidades operacionais ou de segurança.
![vpc sub-rede com zonas](https://github.com/artillisprado/AWS---Templates/blob/master/images/vpc_sub-rede.png?raw=true)
![Endereços Ip para o bloco CIDR](https://github.com/artillisprado/AWS---Templates/blob/master/images/sub-redes.png?raw=true)
![Endereços VPC](https://github.com/artillisprado/AWS---Templates/blob/master/images/enderecos_vpc.png?raw=true)

Subnet
- public : Contém recursos que precisam ser acessíveis ao público, como o site de uma loja online.
  - EC2
  - Internet Gateway - igw : Adiciona uma rota na Route-Table para enviar tráfego para a internet 0.0.0.0/0
- private : Contém recursos que devem ser acessíveis apenas por meio de sua rede privada, como um Banco de Dados que contém informações pessoais dos clientes e históricos de pedidos.
  - EC2
  - NAT Gateway - nat-igw : permite que instâncias em uma sub-rede privada se conectem à internet ou a outros serviços da aws, mas impede que a internet inicie uma conexão com essas instâncias.

![alt text](https://github.com/artillisprado/AWS---Templates/blob/master/images/sub-redes.png?raw=true)

Route Table - Amazon Route Table
  Uma tabela de rotas contém um conjunto de Regras (ou Rotas) configurável para adicionar o tráfego de rede da sub-rede.
![Tabela de Rotas](https://github.com/artillisprado/AWS---Templates/blob/master/images/tabela_rotas.png?raw=true)
