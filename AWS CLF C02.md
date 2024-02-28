
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
Permite também associar aplicações, acessar provedores de e-mail ou software da empresa. 

##### MFA
E verificação de duas etapas, serve para aumentar a segurança da conta. 