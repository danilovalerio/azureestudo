Computação do Azure é um serviço sob demanda, ou seja, quando um recurso precisa ser usado, ele faz a alocação e o desaloca conforme a necessidade
Tipos de computação
- instancias de containers (Serviço de Kubernetes do Azure AKS):
  - Os containers fornecem um ambiente leve e virtualizado que não exige o gerencimanto do sistema operacional e pode responder a alterações sob demanda. 
  - Instâncias de Coneteiner do Azure: uma oferta de PaaS que executa um conteiner ou pod de containers no Azure
  - Aplicativos de conteiner do Azure: uma oferta de PaaS, como instâncias de conteineres, que pode balancear a carga e escalar.
  - Serviço de Kubernetes do Azure: serviço de orquestração para conteineres com arquiteturas distribuídas e grandes volumes de conteineres
- maquinas virtuais 
  - lift-and-shift para numvem (levar como está numa migração) com azure migrate por exemplo 
  - são emulações de computadores físicos
    - inclui processador virtual, memória, armazenamento e rede
    - oferta de IaaS que oferece personalização e controle total
  - conjunto de dimensionamentos, quase igual o load balancer
  - conjunto de disponibilidade de VM: dentro do datacenter temos alguns hacks se todas as máquinas estiverem no mesmo hack e aquele cair teremos a aplicaçao fora do ar.
  - A SEGUIR CONFIGURAÇÃO DE 3 DOMÍNIOS DE FALHAs com os Domain Update
    - hack1 - DOMÍNIO DE FALHA 0
      - VM#1 | UD#1
      - VM#4 | UD#4
    - hack2 - DOMÍNIO DE FALHA 1
      - VM#2 | UD#2
      - VM#5 | UD#5
    - hack3 - DOMÍNIO DE FALHA 2
      - VM#3 | UD#3
      - VM#6 | UD#1  
  - recursos exigidos
- Azure Functions
  - Uma oferta PaaS que dá suporte a operações de computação sem servidor
  - Código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos 
- Area de trabalho virtual do Azure (VDIs)
  - Crie um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway
  - Reduza o risco de que o recurso seja deixado para trás
  - Implantações reais de várias sessões  
  - HOSTS
    - pessoal: vou criar para uma pessoa, quando tiver software específico (custa mais por ser única)
    - em pool: compartilhar para mais usuários e sai mais em conta


Rede Virtual do Azure (VNet)
  - permite a comunicação dos recursos no azure se comuniquem usn com os outros, com a interner e com redes locais
  - Comunicação entre VNets por padrão não existe, tem que configurar
  - As sub-redes virtuais segmentam sua rede para atender às suas necessidades
  - O emparelhamento de rede conecta suas redes privadas diretamente
  - Serviços de rede do Azure: Gateway de VPN: usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela Internet pública (através de um túnel de rede virtual privada IPsec)
  - ExpressRoude: Conexão direta via cabo, ligando a rede do cliente com o servidor da microsoft, as vezes é viável ou não. Ela estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade

DNS (domain name service) do Azure
  - Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast
  - A segurança baseia-se no gerenciador de recursos do Azure, habilitando o contro de acesso baseado em função e o monitoramento registrado em log
  - Facilita o uso e gerenciamento dos recursos e do Azure com um único serviço DNS
  - As redes virtuais personalizáveis permitem nomes privados e totalmente personalizáveis
  - Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure

pontos de extremidaede
 - publico
 - privado




Hospedagem de aplicativos
Redes virtuais
