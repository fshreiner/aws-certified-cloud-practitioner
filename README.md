# aws-certified-cloud-practitioner
Estudos para Certificação AWS Certified Cloud Practitioner

# Intro

Cloud Practitioner!
  
  * ## **Cloud?**
    - **O que é cloud computing?**
	      Computação em nuvem se demonstra extremamente vantajosa, você aluga uma estrutura de acordo com a sua necessidade, sem se preocupar com a condição do hardware do seu servidor fisicamente. Exemplos de empresas que alugam cloud (Microsoft - Azure, Amazom - AWS, Google - Cloud).
	      Você reduz seus custos de hardware.
	      Você tem um nível de refrigeração, segurança e qualidade no hardware que seria muito caro a ser feito localmente por sua empresa.
	      É escalável, você dá upgrade conforme precisa do recurso, não precisa comprar já tudo de início.
	      Cloud é uma empresa disponibilizando seus recursos com um custo mais baixo e gerenciamento muito melhor.
      
    - **Vantagens em se utilizar Cloud Computing**
	      - 1º - Capital expense vs variable expense - Você pensa que vai gastar um valor, porém no fim a demanda é maior em caso de servidores físicos. Nos serviços de                cloud você já sabe o valor fixo do serviço e ele não muda, você já define na hora de adquirir baseado no tempo de uso.
      
	      - 2º - Economies of scale AWS - Quanto mais clientes migrarem para cloud mais baixo a AWS consegue deixar o valor do produto. Desta forma, com o grande crescimento do conceito, é vantajoso optar por soluções cloud.
	      
	      - 3º - Guessing capacity - Quando uma estrutura é feita não dá pra saber como vai ser o uso dela, na cloud você consegue escalar de especificações baixas e subir              aos poucos conforme necessidade. Guessing seria ficar adivinhando a capacidade, na cloud não é necessário se preocupar.
	      
	      - 4º - Speed and Agility - Todo ambiente cloud é rápido e ágil de ser montado, expandido, tratado. Com alguns cliques é possível dar o upgrade necessário a                    qualquer momento.
	      
	      - 5º - Maintaning Data Center - Não é necessário se preocupar com o ambiente, manutenção física, refrigeração, segurança, cuidar de backup dos racks, tudo isso é problema da Amazon, evita muita dor de cabeça.
	      
	      - 6º - Live! in minutes - Agilidade em tudo, é muito rápido para subir um novo serviço, coisa que numa estrutura física seriam dias.
      
	- **Tipos de Cloud Computing**
		 * **IAAS** - Infrastructure As A Service
			 * Trabalhar com a estrutura física deles sem que eles possam acessar seus dados dentro do servidor. Por exemplo, montagem de servidores virtuais (EC2). Você faz aquisição de serviços de infraestrutura porém a AWS não tem acesso ao conteúdo do servidor. Todo gerenciamento dentro do servidor depende de você mesmo, incluindo toda configuração e montagem do mesmo.
		 * **PAAS** - Plattform As A Service 
			 * Montagem de uma plataforma. Você adquire ou utiliza uma plataforma como serviço. Por exemplo, você tem um site e quer subir o site a um servidor na nuvem, porém não quer cuidar da configuração deste servidor nem nada, querendo somente mesmo hospedar o site em um provedor já criado. Você só se preocupa com sua WebPage. Você mesmo fica sem acesso a parte de infraestrutura.
		 * **SAAS** - Software As A Service
			 * Você somente utiliza o software. Por exemplo o gmail, você não tem que criar a página, nem gerenciar os servidores deles, tudo que você faz é acessar a página deles já pronta e utilizar (E-mail, Drive, Etc).
	
	- **Privado, Público e Híbrido - Cloud Deployments**
		- **Plublic Cloud** - Um provedor de nuvem (AWS, Azure, Google Cloud) toma conta da infraestrutura física disponibilizando os serviços. Sendo público, significa que é aberto a qualquer pessoa a opção de adquirir um desses serviços em nuvem, mas não significa que seus dados ficam públicos também, tudo fica seguro e privado ao usuário. Envolve muita segurança aplicada, para garantir a confidencialidade do serviço. 
		- **Hybrid** - Você faz uma junção de publico e privado, por exemplo uma empresa que tem servidores físicos próprios (privados) porém também tem parte dos serviços em funcionamento na núvem pública. Você pode ter um servidor AD local na sua empresa, e manter seu servidor do WebSite na nuvem.
		- **Private Cloud** - (On Premise) É quando você faz o gerenciamento do seu próprio Data Center, você faz o gerenciamento completo de refrigeração, hardware, segurança, controle de acessos, basicamente é você criando sua própria nuvem, basicamente uma arquitetura local, que você expanda aos seus colaboradores.
		
		Atualmente grande parte das empresas ainda se encontram em private cloud. A tendência geralmente é a empresa migrar do private para o hybrid, subindo alguns serviços na public clound, e posteriormente ao validar que o serviço é seguro, que não há falta de disponibilidade nem nada, a tendencia é que as empresas migrem totalmente para a public cloud, visando menores gastos e melhor gerenciamento e facilidade. 
	
	- **Serviços dentro da AWS** 
		- Existe uma grande quantidade de serviços dentro da AWS. O serviço existe para atender todas necessidades que surgirem.
	
	- **Global Infrastruture (Infra Global AWS)**
		- **Regions**
			- AWS trabalha com regiões, geralmente o país, por exemplo Estados Unidos, Brasil, entre outros países.
		- **Availability Zone**
			- São os Data Centers dentro de uma região (Region). Exemplo, dentro da Região (país) Brasil temos as zonas de disponibilidade em SP, BR e RJ para seleção ao adquirir serviços Cloud.
			
		O Brasil infelizmente tem uma das zonas de serviços mais caras devido a cobrança de impostos. Muitas empresas optam por selecionar data centers para utilizar fora do Brasil, para evitar assim os impostos.
	
	- **Free Tier Account (Conta Gratuíta Amazon)**
		- A AWS tem um sistema Free Tier, ou seja, você consegue criar uma conta na AWS  e utilizar os serviços da AWS básicos pelo período de 12 meses para testes, sem cobrança alguma. A Amazon cobra no final do mês pelos serviços utilizados, então é só tomar cuidado e utilizar somente os serviços gratuítos.
  
  * ## **EC2(VM)**
	* **Introdução ao EC2** (Elastic Compute Cloud)
		  * A AWS chama de Instance as máquinas virtuais criadas na Cloud.
		  * Virtualização veio para resolver o problema de ter uma máquina amarrada física servindo somente para um propósito. A virtualizar uma máquina você divide ela em partes para instalar vários outros serviços. Hyper V é um excelente exemplo de virtualização de máquina física.
		  * É muito mais inteligente virtualizar, e em cloud é tudo melhor ainda, pois não é necessário se preocupar com os recursos físicos deste servidor virtualizador. Por isto é tão interessante investir em cloud (AWS), e este serviço de virtualização é chamado de EC2.
	
	- **Tipos de Planos e Valores do EC2**
		- **Plano Sob Demanda**
			- O plano sob demanda é para aquelas situações de urgência, em que você precisa de uma máquina rápida por uma demanda não esperada que surgiu. A AWS deixa reservado muito hardware "parado", não alocado, justamente para atender as demandas deste tipo, porém por necessitar ficar com equipamento ocioso a AWS acaba cobrando um pouco mais caro nas máquinas deste plano. Este plano também não tem nenhum vínculo a longo prazo, sendo cobrado por hora ou segundos de uso, sem compromisso de prazo mínimo, sendo ideal para momentos de pico, testes de novas funcionalidades, e você tem total gerenciamento de processamento.
		- **Plano Saving Plans**
			- No saving planes, você firma um contrato de compromisso com a AWS, podendo ser de 1 ano, 3 anos, ou mais. É o tipo certo para quando a empresa tem o servidor já definido e sabe que vai ficar com ele por longos períodos ativos, graças a este comprometimento de aluguel a Amazon oferece um preço muito mais em conta comparado ao plano sob demanda, sendo a melhor opção para aplicações físicas.
		- **Plano Host Dedicados**
			- Este plano é para quem necessita de um host dedicado exclusivamente a sua empresa, você aluga um servidor completo para seu uso, que acaba saindo um pouco mais caro, porém você pode economizar usando suas licenças neste servidor que você já possua previamente, como licenças de sistema operacional, banco de dados ou se quiser aplicar outros tipos de softwares, como Linux, ou algo específico que precise ser instalado por completo num host geral.
		- **Plano Instâncias Spot**
			- No spot instances você pode conseguir economia de até 90% no valor da máquina. Essa economia é conseguida através de uma barganha, como a AWS mantém muito de seu hardware ocioso para atender os planos sob demanda, você pode pedir uma instância spot, a AWS vai ceder recursos desses hardwares parados a você com um preço bem mais baixo, porém caso a AWS precise de recurso para atender planos sob demanda, ela vai desligar seu host sem prévio aviso e alocar para quem está pagando sob demanda. É feito para quando você precisa de um recurso grande e urgente, porém para testes, nunca produção, visando que sua aplicação pode ser interrompida a qualquer momento.
		- **Cobrança por segundo**
			- A cobrança nos planos por segundo pode ser solicitada, então é cobrado um mínimo de 60 segundos, e posteriormente você só vai pagar o que utilizar pelo tempo que a máquina estiver ligada. Perfeito para desenvolvimento/testes de aplicações.
	
	- **Calculadora de Instancias EC2**
		- A AWS disponibiliza o AWS Pricing Calculator, em que você pode utilizar a ferramenta para calcular todo tipo de plano, máquina, recursos, tudo isto para criar uma estimativa de valor referente ao serviço que você necessita.
		- https://calculator.aws/#/?nc2=h_ql_pr_calc
	
	- **Tipos de Instancias EC2**
		- Tipos de instâncias se tratam de tipos de VMs, máquinas virtuais
			- Uso Geral
				- Mac, T4g, T3, T3a, N2, M6g, M6i, M6a, M5, M5a, M5n, M5zn, M4, A1
				
			- Otimizadas para Computação
				- C7g, C6g, C6gn, C6i, C6a, Hpc6a, C5, C5a, C5n, C4
				
			- Otimizadas para Memória
				- R6g, R6i, R5, R5a, R5b, R5n, R4, X2gd, X2idn, X2iedn, X2iezn, X1e, X1, Alta Memória, z1d
				
			- Computação Acelerada
				- P4, P3, P2, DL1, Trn1, Inf1, G5, G5g, G4dn, G4ad, G3, F1, VT1
				
			- Otimizadas para Armazenamento
				- Im4gn, Is4gen, I4i, I3, I3en, D2, D3, D3en, H1
				
			- Recursos das Instâncias
				- Instâncias expansíveis
				- Várias opções de armazenamento
				- Instâncias otimizadas para o EBS
				- Redes em cluster
				- Recursos do processador Intel
				
			- Medir performance das Instâncias
				- Por que é necessário medir a performance das instâncias?
					- O Amazon EC2 permite que você provisione diversos tipos de instâncias, que oferecem combinações diferentes de CPU, memória, disco e rede. É fácil executar novas instâncias e testes em paralelo. Recomendamos a medição de performance dos aplicativos para identificar os tipos de instâncias adequados e validar a arquitetura dos aplicativos. Também recomendamos testes rigorosos de carga e escala para garantir que seus aplicativos tenham a escalabilidade pretendida.
	 
	- **Introdução ao EBS**
		- EBS significa Elastic Block Store, a AWS não deixa os HDs ou SSDs na própria máquina física, mas sim tem storages de armazenamento dedicados somente para lidar com estes armazenamentos. (Vai armazenar dados bora pro HD, vai rodar aplicações de sistemas bora SSD)
			- SSD
				- io2, io2 Block Express, io1, gp3, gp2
			- HDD
				- st1, SC1
	
	- **O que é um Load Balancer**
		- A AWS tem o Elastic Load Balancer, que cuida basicamente de receber as requisições aos seus servidores e distribuir entre todos seus servidores automaticamente de forma a não sobrecarregar nenhum dos servidores, ele cuida de balancear as requisições entre todos seus servidores. Existem 3 tipos:
			- Application - Você tem um load balancer bem inteligente, ele consegue visualizar a camada 7 da camada OSI, ou seja a Aplicação. Resumidamente ele consegue verificar o que o usuário está acessando dentro do site, e ele direciona o tráfego da pessoa de acordo com isso. Por exemplo, um site que tem duas linguas (PT e English) o load balancer application já consegue ver de onde você acessou e te redireciona ao seu idioma.
			- Network - Este modelo não se preocupa com o tipo de tráfego, mas sim com a quantidade, ele só verifica endereçamento IP, vendo até a camada 4 do modelo OSI, podendo ver os protocolos TCP e UDP. Você pode dividir o tráfego de forma a separar porcentagens de tráfego em cada servidor.
			- Classic - Ele é uma junção do network e do application. Ele ainda vê a camada 7, mas não muito precisamente, ele foi o primeiro a ser criado pela AWS por isto está um pouco defasado, e atualmente já não é tão utilizado.
	
	- **O que é AutoScaling**
		- Este serviço pode nos ajudar muito, por exemplo, em um site de e-commerce em uma época tem uma redundância de 2 servidores, porém o site é acessado por vários usuários que acessam esses servidores. E se de uma hora pra outra a quantidade de usuários aumentar muito? Os servidores aguentaram? Com muito uso, isso afetará o desempenho do site, o serviço vai se tornar pior para os usuários. É impossível prever com exatidão a quantidade de acessos que você vai ter, porém podemos usar o serviço de autoscaling para nos salvar, o correto seria iniciar outros servidores para suprir a demanda, porém invés de fazer de forma manual, podemos usar o autoscaling para fazer essa extensão de forma automática, bem mais rápida, sobe muito rápido automaticamente, invés de você ter que ir lá e fazer isso manualmente. Precisamos definir somente 3 passos para usar autoscaling, os grupos (instâncias EC2 por exemplo, para servidores WEB), o template que é qual tipo de máquina será adicionado quando tiver necessidade de escalar, e por último a parte de options, onde você configura o formato de escalagem, se vai subir quantas máquinas manualmente, se vai desativar depois, todas essas configurações. Existem 5 tipos de autoscaling:
			- All Times - Manter as intâncias atuais a todo tempo, por exemplo você tem 4 instâncias que vai deixar sempre ligado, e mais 6 que vão escalar. Se seus servidores principais, um deles caírem, uma dessas 4 ativas vão assumir o que cair.
			- Scale Manally - Neste tipo você define manualmente, você define por exemplo que quer 5 instâncias agora, e programa o fim de semana para tirar essas 5.
			- Schedule - Você cria tarefas, por exemplo de segunda a sexta você quer manter 4 máquinas, e nos fins de semana você ativa só 2 máquinas (podem ser dias, ou horas, bem personalizável).
			- On Demand - Quando você configura por exemplo porcentagens de uso, quando suas máquinas chegarem a 50% de CPU você sobe mais máquinas por exemplo, tem todo um gerenciamento por meio de processamento para saber quando subir.
			- Predictive - Um dos mais novos da AWS, é utilizado em conjunto a outros serviços, você conecta todas suas métricas de todos serviços e faz o ajuste automático interligando tudo, independente de qual serviço seja usado na máquina.

* ## **Storage S3**
	* 

* IAM - Identity and access management (Users, Groups)

* Billing, Pricing

* Security
  
  
  Exam CLF - C01
  
  --------------


# Leitura Complementar -
  
  **- O que é a computação em nuvem?**
A computação em nuvem é a entrega de recursos de TI sob demanda por meio da Internet com definição de preço de pagamento conforme o uso. Em vez de comprar, ter e manter datacenters e servidores físicos, você pode acessar serviços de tecnologia, como capacidade computacional, armazenamento e bancos de dados, conforme a necessidade, usando um provedor de nuvem como a Amazon Web Services (AWS).

  **- Quem usa a computação em nuvem?**
Organizações de todos os tipos, portes e setores usam a nuvem para uma grande variedade de casos de uso, como backup de dados, recuperação de desastres, e-mail, desktops virtuais, desenvolvimento e teste de software, análises de big data e aplicativos web voltados ao cliente. Por exemplo, as empresas do setor de saúde usam a nuvem para desenvolver tratamentos mais personalizados para os pacientes. Empresas de serviços financeiros usam a nuvem como base para detectar e prevenir fraudes em tempo real. E fabricantes de videogames usam a nuvem para entregar jogos online para milhões de jogadores em todo o mundo.


**- Benefícios da computação em nuvem**

  **Agilidade**
A nuvem oferece acesso fácil a uma grande variedade de tecnologias para que você possa inovar mais rapidamente e criar praticamente tudo o que puder imaginar. Você pode gerar rapidamente recursos conforme a necessidade, de serviços de infraestrutura, como computação, armazenamento e bancos de dados até Internet das Coisas, machine learning, data lakes, análises de dados e muito mais.
Você pode implantar serviços de tecnologia em questão de minutos e passar da ideia à implementação com agilidade várias ordens de grandeza maior do que antes. Assim, você tem a liberdade de experimentar, testar novas ideias para diferenciar as experiências dos clientes e transformar a sua empresa.

  **Elasticidade**
Com a computação em nuvem, você não precisa provisionar recursos em excesso para absorver picos de atividades empresariais no futuro. Em vez disso, você provisiona a quantidade de recursos realmente necessária. Você pode aumentar ou diminuir instantaneamente a escala desses recursos para ajustar a capacidade de acordo com a evolução das necessidades empresariais.

  **Economia de custo**
A nuvem permite que você troque as despesas de capital (datacenters, servidores físicos etc.) por despesas variáveis e pague apenas pela TI consumida. Além disso, as despesas variáveis são muito menores do que as que você pagaria por conta própria devido às economias de escala.

  **Implantação global em questão de minutos**
Com a nuvem, você pode ampliar as atividades para novas regiões geográficas e implantar globalmente em minutos. Por exemplo, a AWS tem infraestrutura em todo o mundo, o que permite que você implante aplicativos em vários locais físicos com apenas alguns cliques. Aproximar os aplicativos dos usuários finais reduz a latência e melhora a experiência desses usuários.


**-Diferentes Tipos de Cloud**

**Infraestrutura como serviço (IaaS)**
O IaaS contém os componentes básicos da IT na nuvem. Normalmente, o IaaS oferece acesso a recursos de rede, computadores (virtuais ou em hardware dedicado) e espaço de armazenamento de dados. O IaaS oferece o mais alto nível de flexibilidade e controle de gerenciamento sobre os recursos de TI. Ele é o tipo de computação mais semelhante aos recursos existentes de TI, já conhecidos por vários departamentos e desenvolvedores de TI.

**Plataforma como serviço (PaaS)**
Com o PaaS, você não precisa mais gerenciar a infraestrutura subjacente (geralmente, hardware e sistemas operacionais) e pode manter o foco na implantação e no gerenciamento de aplicativos. Dessa forma, você fica mais eficiente, pois não precisa se preocupar com aquisição de recursos, planejamento de capacidade, manutenção de software, correções ou qualquer outro tipo de trabalho genérico repetitivo necessário para a execução dos aplicativos.

**Software como serviço (SaaS)**
O SaaS oferece um produto completo, executado e gerenciado pelo provedor de serviços. Na maioria dos casos, quando as pessoas mencionam SaaS, estão falando de aplicativos de usuários finais (como e-mail baseado na web). Com uma oferta de SaaS, você não precisa pensar sobre a manutenção do serviço ou o gerenciamento da infraestrutura subjacente. Você só precisa se preocupar sobre como utilizará esse software específico.


**-Regiões e Availability Zones (Zonas de Disponibilidade)**

 **Regiões**
A AWS tem o conceito de uma região, que é um local físico em todo o mundo onde agrupamos datacenters. Chamamos cada grupo de datacenters lógicos de zona de disponibilidade. Cada região da AWS consiste em várias AZs isoladas e separadas fisicamente em uma área geográfica. Diferentemente de outros provedores de nuvem, que geralmente definem uma região como um único datacenter, o design de múltiplas AZs de cada região da AWS oferece vantagens para os clientes. Cada AZ tem energia, refrigeração e segurança física independentes e está conectada por meio de redes redundantes de latência ultrabaixa. Os clientes da AWS, focados em alta disponibilidade, podem projetar seus aplicativos para serem executados em várias AZs, a fim de obter tolerância a falhas ainda maior. As regiões de infraestrutura da AWS atendem aos mais altos níveis de segurança, conformidade e proteção de dados.
A AWS fornece uma presença global mais extensa do que qualquer outro provedor de nuvem. Para oferecer suporte à sua presença global e garantir que os clientes sejam atendidos em todo o mundo, a AWS abre novas regiões rapidamente. A AWS mantém várias regiões geográficas, incluindo regiões da América do Norte, África do Sul, América do Sul, Europa, China, Ásia-Pacífico e Oriente Médio.

 **Zonas de disponibilidade**
Uma zona de disponibilidade (AZ) é um ou mais datacenters distintos com energia, rede e conectividade redundantes em uma região da AWS. As AZs proporcionam aos clientes a capacidade de operar aplicativos e bancos de dados de produção com alta disponibilidade, tolerância a falhas e escalabilidade em níveis superiores aos que um único datacenter pode oferecer. Todas as AZs em uma região da AWS estão interconectadas por redes de alta largura de banda e baixa latência, usando fibra metropolitana dedicada e totalmente redundante para proporcionar redes de alto throughput e baixa latência entre AZs. Todo o tráfego entre as AZs é criptografado. A performance da rede é suficiente para realizar a replicação síncrona entre as AZs. As AZs particionam aplicativos para facilitar a alta disponibilidade. Se um aplicativo for particionado em várias AZs, as empresas estarão melhor isoladas e protegidas contra problemas como quedas de energia, raios, tornados e terremotos, entre outros. As AZs são fisicamente separadas por uma distância significativa (vários quilômetros) das outras AZs, embora todas estejam a um raio de até 100 km entre si.

## Leitura Complementar - Autoscaling

**O que é o AWS Auto Scaling?**
O AWS Auto Scaling é um novo serviço da AWS para ajudar a otimizar o desempenho de aplicativos e reduzir custos de infraestrutura por meio da escalabilidade fácil e segura de vários recursos da AWS. O serviço simplifica a experiência de escalabilidade, permitindo escalar coleções de recursos relacionados usados por um aplicativo com apenas alguns cliques. O AWS Auto Scaling ajuda a configurar políticas de escalabilidade consistentes e congruentes em toda a pilha de infraestrutura usada por um aplicativo. O AWS Auto Scaling escala automaticamente os recursos conforme a necessidade para cumprir a estratégia de escalabilidade selecionada. Assim, você pode manter o desempenho e pagar apenas pelos recursos realmente necessários.

**Quais os benefícios do AWS Auto Scaling?**
O AWS Auto Scaling é uma forma rápida e fácil de otimizar o desempenho e os custos dos aplicativos.
-   **Configure rapidamente a escalabilidade:** o AWS Auto Scaling oferece uma experiência unificada de escalabilidade para todos os recursos escaláveis usados pelos aplicativos. É possível ver a utilização média de todos os recursos escaláveis e definir rapidamente os níveis pretendidos de utilização para cada grupo de recursos semelhantes em uma interface simples e intuitiva.    
-   **Tome decisões de escalabilidade com inteligência:** o AWS Auto Scaling permite automatizar a forma como recursos diferentes respondem às alterações de demanda. Estratégias de escalabilidade fáceis de compreender permitem priorizar disponibilidade, custos ou um equilíbrio ente os dois. O AWS Auto Scaling cria automaticamente todas as políticas de escalabilidade e define objetivos de acordo com sua preferência.  
-   **Mantenha automaticamente o desempenho:** o AWS Auto Scaling monitora continuamente os recursos subjacentes dos aplicativos para garantir que operem nos níveis de performance desejados. Quando ocorrem picos de demanda, o AWS Auto Scaling aumenta automaticamente a capacidade dos recursos restritos para manter uma alta qualidade de serviço.    
-   **Estime os custos e evite gastos desnecessários:** o AWS Auto Scaling pode ajudar a otimizar as eficiências de utilização e custo do consumo de serviços da AWS. Assim, você paga apenas pelos recursos realmente necessários. Quando a demanda cai, o AWS Auto Scaling remove automaticamente toda a capacidade excessiva de recursos, evitando gastos desnecessários.

**Quando devo usar o AWS Auto Scaling?**
Você deve usar o AWS Auto Scaling para aplicativos que usam um ou mais recursos escaláveis e estão sujeitos a cargas variáveis. Um bom exemplo seria um aplicativo web de comércio eletrônico que recebe tráfego variável durante o dia. O aplicativo segue uma arquitetura padrão de três camadas: o Elastic Load Balancing distribui o tráfego recebido, o Amazon EC2 é a camada de computação e o DynamoDB é a camada de dados. Neste caso, o AWS Auto Scaling escalará um ou mais grupos do EC2 Auto Scaling e tabelas do DynamoDB usados pelo aplicativo para responder à curva de demanda.

**Como posso começar a usar o AWS Auto Scaling?**
O AWS Auto Scaling permite a seleção de aplicativos de acordo com tags de recursos ou com pilhas do AWS CloudFormation. Com apenas alguns cliques, é possível criar um plano de escalabilidade para um aplicativo. Esse plano define como cada um dos recursos usados pelo aplicativo será escalado. Para cada recurso, o AWS Auto Scaling cria uma política de escalabilidade de rastreamento direcionada com a métrica mais popular para esse tipo de recurso e mantém essa métrica em um valor direcionado para a estratégia de escalabilidade selecionada. Para definir os valores das métricas de recursos, você pode optar entre três recomendações de escalabilidade predefinidas que otimizam disponibilidade, otimizam custos ou equilibram esses dois critérios. Ou, se preferir, você pode definir seus próprios valores pretendidos. Além disso, o AWS Auto Scaling define automaticamente os valores mínimo e máximo dos recursos.