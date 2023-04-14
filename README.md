# REDES E ENTREGAS DE CONTEÚDO:

VPC
Seção que agrupam recursos com base nas necessidades operacionais ou de segurança.
<p align="center">
  <image src="https://github.com/artillisprado/AWS---Templates/blob/master/images/vpc_sub-rede.png?raw=true" alt="vpc sub-rede com zonas" height="50%" width="50%" />
</p>
<image src="https://github.com/artillisprado/AWS---Templates/blob/master/images/sub-redes.png?raw=true" alt="Endereços Ip para o bloco CIDR" height="50%" width="50%" />
<image src="https://github.com/artillisprado/AWS---Templates/blob/master/images/enderecos_vpc.png?raw=true" alt="Endereços VPC" height="50%" width="50%" />

Subnet
- public : Contém recursos que precisam ser acessíveis ao público, como o site de uma loja online.
  - EC2
  - Internet Gateway - igw : Adiciona uma rota na Route-Table para enviar tráfego para a internet 0.0.0.0/0
- private : Contém recursos que devem ser acessíveis apenas por meio de sua rede privada, como um Banco de Dados que contém informações pessoais dos clientes e históricos de pedidos.
  - EC2
  - NAT Gateway - nat-igw : permite que instâncias em uma sub-rede privada se conectem à internet ou a outros serviços da aws, mas impede que a internet inicie uma conexão com essas instâncias.

<image src="https://github.com/artillisprado/AWS---Templates/blob/master/images/public_private.png?raw=true" alt="" height="50%" width="50%" />

Route Table - Amazon Route Table
  - Uma tabela de rotas contém um conjunto de Regras (ou Rotas) configurável para adicionar o tráfego de rede da sub-rede.
<image src="https://github.com/artillisprado/AWS---Templates/blob/master/images/tabela_rotas.png?raw=true" alt="" height="50%" width="50%" />
