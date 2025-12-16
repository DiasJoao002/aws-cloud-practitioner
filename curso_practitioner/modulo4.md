<h2>Módulo 4 - Alcançe Global</h2>

<p>Para termos de alta disponibilidade e redução de latênica, a AWS utiliza os chamados "Locias de Borda", instalações menores que armazenam dados frequentemente acessados em cache, para que os usuários acessem com menor latência. Além disso, ela também disponibiliza muitas regiões e zonas de disponibilidade "arround the world", e existem 4 principais critérios que devem ser levados em consideração para se escolher uma região:</p>

1. Compliance - Conformidade
2. Proximity - Proximidade
3. Feature Avaibility - Disponibilidade de recursos
4. Price - Preço

<p>A questão da conformidade varia de acordo com a legislação local, ou seja, pode ser uma na China e outra totalmente diferente no Brasil. E por isso é importante levar esses fatores em consideração para andar segundo a lei. A proximidade também deve ser levada em consideração por conta da latência, porque regiões mais próximas de seus usuários possuem um tempo de resposta menor. No entanto, é mais importante para grandes aplicações que realmente precisam de um tempo de resposta otimizado.</p>
<p>Há também a questão de disponibilidade de recursos, uma vez que a AWS está sempre buscando inovar e expandir seus recursos. Dessa forma, nem todas as regiões possuem exatamente as mesmas ofertas da AWS, como por exemplo em questões de maior segurança física e controle de acesso (é padrão e seguro, mas algumas regiões possuem mais rigor ainda). Por fim, há o preço, que varia de acordo com os gastos operacionais da região, que são incluenciados por exemplo por tarifas e preço de energia elétrica.</p>

<p>É valido lembrar que as Regiões são locais físicos em todo o mundo que contêm vários data centers. Cada Região contém pelo menos três Zonas de Disponibilidade. Cada Zona de Disponibilidade contém um ou mais data centers. Os locais da borda são dispositivos em áreas fora das regiões. Esses dispositivos fornecem ao usuário acesso aos dados acessados com frequência e com baixa latência.</p>

<h2>Infraestrutura</h2>
<p>Visando facilitar a configuração e gerenciamento de infraestruturas na nuvem, a AWS disponibiliza um serviço chamado CloudFormation, um serviço que ajuda a modelar os recuros na AWS para que o foco esteja nas aplicações hospedades na AWS. Para isso, é utilizado um conceito chamado de "Infraestrutura como Código - Infraestructure as Code", que basicamente permite definir um modelo com todos os recursos necessários para a implementação na AWS e então enviar esse modelo para a CloudFormation, que irá se encarregar de provisionar e configurar esses recursos.</p>
<p>Ou seja, com o CloudFormation, os usuários podem modelar e configurar os recursos da AWS com o uso de código para automatizar o provisionamento e gerenciamento da infraestrutura</p>