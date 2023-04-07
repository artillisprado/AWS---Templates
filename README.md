# AWS---Templates

REDES E ENTREGAS DE CONTEÚDO:

VPC
Seção que agrupam recursos com base nas necessidades operacionais ou de segurança.

Subnet
- public : Contém recursos que precisam ser acessíveis ao público, como o site de uma loja online.
- private : Contém recursos que devem ser acessíveis apenas por meio de sua rede privada, como um Banco de Dados que contém informações pessoais dos clientes e históricos de pedidos.

Route Table - Amazon Route Table
  Uma tabela de rotas contém um conjunto de Regras (ou Rotas) configurável para adicionar o tráfego de rede da sub-rede.
- Public : 
Internet Gateway - igw
 - Usada por Public-Subnet, adiciona uma rota na Route-Table para enviar tráfego para a internet 0.0.0.0/0
- private : 
NAT Gateway - nat-igw
 - Um Gateway de Conversão de Endereços de Rede (NAT) permite que instâncias em uma sub-rede privada se conectem à internet ou a outros serviços da aws, mas impede que a internet inicie uma conexão com essas instâncias.
