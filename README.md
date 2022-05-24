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
    
* Storage S3

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