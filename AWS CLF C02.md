
#### Conceitos

O que e **Cloud Computing?** - Vários Data Centers conectados, sendo uma opção mais vantajosa a ter um servidor físico(que pode render problemas para possíveis upgrades, refrigera mento, quebra de componentes)

Vantagens: 
- Custos reduzidos;
- Escala global (alta escalabilidade);
- Performance;
- Velocidade (serviços iniciados rapidamente);
- Produtividade (por consequência de todos);
- Segurança;
- Flexibilidade/remoto (permiti o trabalho a distancia).

##### Tipos de Cloud

Infraestrutura como serviço(IAAS) -> Permite que um cliente alugue uma infraestrutura de TI, como:
- Servidores;
- VM;
- Storage.

Plataforma como serviço(PAAS) -> Focado na área do software, como:
- SO;
- Banco de dados;
- Hospedagem.

Software como serviço(SAS) -> Adquirir uma aplicação, como:
- E-mail;
- Dropbox.

Nuvem pública -> AWS, Azure, GCP. (Quer dizer que os servidores são 'públicos, apesar de outras pessoas usarem o mesmo servidor que você, e garantido pelo host que eles não vão acessar seus dados');
Nuvem privada -> Bancos, governos, empresas financeiras;
Nuvem Híbrida  -> Público/Privado, e o meio ponto entre os dois, alguns dados estão no público e os dados mais sigilosos no privado.

##### AWS Support

(Não vou descrever tudo)
Vários graus de suporte:

1. Developer - Numero limitado de contato com o suporte e horários não vantajosos, demora na resposta, resposta genéricas.
2. Business - Consideravelmente melhor que o Developer em questão de resposta mas não tem os benefícios dos Enterprise que conseguem resolver problemas em menos de meia hora. 
3. Enterprise-on-Ramp - Muito melhor que o Business mas não chega próximo ao Enterprise.
4. Enterprise - Praticamente um consultor para te ajudar.

#### IAM

Controle de usuários, grupos, permitir grupos ou um usuário especifico a fazer determinada ação baseada em uma politica que foi cedida por um Admin ou pelo ROOT.  Além disso, tem o Roles, alguma máquina tem acesso a outra máquina que foi habilitado por uma função.

##### IAM Identity Center 
Permite também associar aplicações, acessar provedores de e-mail ou software da empresa.  Adicionar usuários para usar uma aplicação que dentro da AWS.

##### MFA
E verificação de duas etapas, serve para aumentar a segurança da conta. 

##### AWS Organization
Usado para criação de subcontas (organizações), para gerenciar outros tipos de projetos.
Permite: 
- **Gerenciamento Centralizado de Contas**
- **Controle de Acesso Hierárquico**
- **Políticas de Controle de Serviço**
- **Junção da cobrança em um lugar**
- **Automação**

##### Políticas de Senha
E possível alterar a política de criação de senha.

##### Outras maneiras de acessar: CloudShell e CLI
CLI - Facilita a utilização de Scripts. Feito usando um software usando suas credenciais da AWS.
Requer:
- Acess Key;
- Private Key.
SDK - Quando uma aplicação precisa se comunicar com a AWS, tambem precisa de Acess key e Private key.
CloudShell - Maquina Linux qual a AWS oferece, permitindo uso do console pelo site da AWS.

##### IAM Credential Report e Acess Advisor

Credential Report - Mostra quando os usuários foram criados, ultimo login, ultima senha trocada, MFA ativado ou não.
Acess Advisor - Mostra quais serviços permitidos para devido usuário. 
AWS CloudTrail - Permite registrar todas as ações de um usuário para auditoria.  

#### Estrutura da AWS

##### Infraestrutura global 

Uma região contem data centers, que são divididos em zonas de disponibilidade.

Zonas locais(AZs) - E uma zona menor que conecta a um Data Center, para regiões que estão longe de um data center.

Wavelength - Usado normalmente por desenvolvedores, tem uma latência muito menor e por consequência vai ter uma conexão mais rápida. 

Outposts - E como se fosse um mini data center, colocado em um lugar especifico que não tem interesse em colocar uma zona local.

##### AWS Share Responsibility Model 

Você tem uma parte da responsabilidade sobre a sua cloud, nem tudo vai ser culpa da AWS.

Customer - Dados inseridos, aplicação, cuidar dos usuarios, conexões e configurações de firewall, trafego de rede, encriptação de dados no client-side.

AWS - Software e Hardware.

#### EC2 (IAAS)

Elastic coumput cloud. E um Cluster de servidores que funciona para criarmos instancia de determinado sistemas operacional.

##### Tipos de EC2

##### Modelos de preço

Cobrança baseada em segundos, transferência de arquivos para fora da AWS, determinado hardware com maior qualidade, IP estático.

AWS Calculator - Usado para calcular quanto pagara por uma instancia. 

Modelos de aquisição:
- Sob demanda - Caro, começa instantaneamente;
- Saving plans - Barato, contrato de longo prazo (1 a 3 anos);
- Spot - Barato, mas pode ser encerrado sem a sua permissão, pois caso a AWS precisar ela vai usar o que você esta ocupando;
- Host dedicado - Muito caro, privado;
- Capacidade por demanda - Médio, especifica todo o hardware necessário a partir de tal dia ate outro determinado dia.