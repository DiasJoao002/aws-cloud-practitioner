Computação em Nuvem

A AWS oforece uma ferramenta de computação em nuvem chamada Elastic Compute Cloud (EC2). Ela foi projetada para ser mais flexível, econômica e escalável, em comparação com a computação baseada na própria infraestrutura física (on-premisses).

Para configurar uma instância virtual é preciso primeiramente definir a imagem de máquina (AMI), como Linux ou Windows, e então o tipo de instância EC2, ou seja, a potência desejada em termos de processamento, memória e rede.

-- TIPOS DE INSTÂNCIAS --

    1. Uso geral: combina bem os requisitos para se rodar simples aplicações, como hospedar serviços da web
    2. Otimizada para computação: ideiais para tarefas que demandam um poder de processamento massivo, como ML e simulações científicas
    3. Otimizada para memória: ideal para aplicações que consomem grandes volumes de RAM
    4. Computação acelerada: usa aceleradores de hardware para lidar com tarefas como processamento gráfico e cálculos float
    5. Otimizada para armazenamento: projetadas para tarefas que demandam alto desempenho para dados armazenados localmente

-- APIs --

Todas as interações com os serviços da AWS são feitas por meio de APIs, e existem 3 métodos principais de acessá-las: 
1. Console AWS: interface visual onde é possível gerenciar os serviços da AWS de forma manual
2. AWS CLI: Command Line Interface da AWS, onde é possível automatizar as tarefas de gerenciamento dos serviços por meio de scripts, o que ajuda a reduzir erros humanos e ser mais eficiente
3. AWS SDK: Software Development Kit que permite interagir com as APIs por meio de várias linguagens de programação, como python

-- SCALING --   

Os conceitos de escalabilidade e elasticidade são muito usados no EC2, e ajudam a manter a aplicação sempre oferecendo o melhor para o usuário e com um excelente custo benefício. A escalabilidade pode se referir tanto ao aumento vertical (aumento do poder de processamento das máquinas) quanto ao aumento horizontal (mais máquinas). 
Já a elasticidade se refere à capacidade do sistema aumentar ou diminuir seus recursos dinamicamente e de forma automatizada. Ou seja, aumenta os recursos quanto a demanda aumenta diminui quanto a demanda dimunui, o que fornece eficiência e uso ideal dos recursos a qualquer momento. 

Para ajudar no ajuste automático dos recursos existe o Amazon EC2 Auto Scaling, que se encarrega de ajustar automaticamente o número de instâncias com base na demanda. Para isso, é preciso estabelecer grupos de Auto Scaling, que são as coleções que podem ser ampliadas ou reduzidas. Esses grupos precisam de 3 definições:
    1. Capacidade mínima: o mínimo de instâncias necessárias para manter a aplicação em execução
    2. Capacidade desejada: o número ideal de instâncias a serem mantidas (precisa de um estudo sobre a demanda)
    3. Capacidade máxima: o máximo de instâncias que podem ser alocadas para altas demandas. 

-- ELASTIC LOAD BALANCING --

É um serviço que pode (e em muitos casos deve) ser utilizado em conjunto com o Auto Scaling, pois atua como um único receptor das requisições distribuindo o fluxo de tráfego da aplicação sem sobrecarregar as instâncias disponíveis. Ou seja, ele atua em conjunto para distribuir uniformemente o tráfego, aumentando desempenho e confiabilidade. 

-- DISTRIBUIÇÃO DE MENSAGENS --

1. Amazon EventBridge
2. Amazon Simple Queue Service (https://aws.amazon.com/sqs/):
    Serviço que separa os componentes da aplicação por meio do enfileiramento de mensagens, armazenando e processando mensagens de forma confiável.
3. Amazon Simple Notification Service (https://aws.amazon.com/sns/):
    Serviço de mensagens para enviar notificações a usuários ou outras aplicações por meio de SMS, e-mail ou notificações por push móveis.
