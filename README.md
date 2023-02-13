# Marketing Analytics

## Conceito
Marketing Analytics compreende os processos e tecnologias que permitem aos profissionais de Marketing avaliar o sucesso de suas iniciativas.

Isso é feito medindo o desempenho das campanhas de Marketing, coletando os dados e analisando os resultados. Marketing Analytics utiliza métricas importantes de negócios, como ROI (Retorno Sobre o Investimento), Atribuição de Marketing e Eficácia Geral de Marketing. Em outras palavras, o Marketing Analytics mostra se os programas de Marketing estão sendo efetivos ou não.

Marketing Analytics reúne dados de todos os canais de marketing e os consolida em uma visão de marketing comum. A partir dessa visão comum, você pode extrair resultados analíticos que podem fornecer assistência inestimável para impusionar os esforços de marketing.

## Por que Marketing Analytics é importante? 

Ao longo dos anos, à medida que as empresas expandiram para novas categorias de marketing, novas tecnologias foram adotadas para apoiá-las. Como cada nova tecnologia era normalmente implantada isoladamente, o resultado foi uma mistura de ambientes de dados desconectados. 

Consequentemente, os profissionais de marketing costumam tomar decisões com base em dados de canais individuais (marketing digital e métricas de sites, por exemplo), sem levar em consideração todo o cenário de marketing. Dados de mídia social por si só não são suficientes. Dados de análise da Web por si só não são sufientes. E ferramentas que analisam apenas um instantâneo do tempo de um único canal são lamentavelmente inadequadas.

Marketing Analytics, por outro lado, considera todos os esforços de marketing em todos os canais ao longo de um período de tempo - o que é essencial para tomadas de decisões corretas e a execução eficiente das companhas e iniciativas de marketing de uma empresa.

## O que podemos fazer com Marketing Analytics?
Com Marketing Analytics, podemos responder a perguntas como estas:
- Como estão as nossas iniciativas de marketing hoje? Que tal a longo prazo? O que podemos fazer para melhorá-las?
- Como as nossas atividades de marketing se comparam às de nossos concorrentes? Onde eles estão gastando seu tempo e dinheiro? Eles estão usando canais que não estamos usando?
- O que devemos fazer em seguida? Nossos recursos de marketing estão alocados corretamente? Estamos dedicando tempo e dinheiro aos canais certos? Como devemos priorizar nossos investimentos para o próximo ano?
- Qual o perfil dos nossos clientes? Eles são da mesma área regional? Tem os mesmos gastos e preferências?
- Consigo segmentar meus clientes por similiaridade? Tenho como saber os gastos por grupo?
- E muitas outras...

## O que é segmentação de cliente? 
A segmentação de clientes é o processo de dividir os clientes em grupos com base em características comuns, para que as empresas possam comercializar para cada grupo de forma eficaz e adequada, ou simplesmente compreender o padrão de consumo dos clientes.

## Marketing B2B x Marketing B2C
No Marketing Business-to-Business (B2B), uma empresa pode segmentar clientes de acordo com uma ampla variedade de fatores, incluindo: 
- Indústria
- Número de empregados
- Produtos comprados anteriormente na empresa
- Localização

No Marketing Business-to-Consumer (B2C), as empresas segmentam os clientes de acordo com dados demográficos e padrões de consumo, tal como: 
- Idade
- Gênero
- Estado Civil
- Localização (urbana, suburbana, rural)
- Estágio da vida (sem filhos, aposentado etc)
- Produtos comprados
- Valor Gasto
- Horário de consumo

## Por que Segmentar Clientes? 
A segmentação permite que os profisionais de marketing adaptem melhor seus esforços de marketing a vários subconjuntos de público-alvo. Esses esforços podem estar relacionados às comunicações e ao desenvolvimento de produtos. Especificamente, a segmentação ajuda uma empresa a:

- Criar e comunicar mensagens de marketing direcionadas que ressoarão com grupos específicos de clientes, mas não com outros (que receberão mensagens personalizadas para suas necessidades e interesses).
- Selecionar o melhor canal de comunicação para o segmento, que pode ser e-mail, publicações em mídias sociais, publicamente em rádio ou outra abordagem, dependendo do segmento.
- Identificar maneiras de melhorar produtos ou novas oportunidades de produtos ou serviços.
- Estabelecer melhor relacionamentos com os clientes.
- Testar as opções de preços.
- Concentrar-se nos clientes mais rentáveis.
- Melhores o atendimento ao cliente.
- Escolher entre venda por atacado e venda cruzada de outros produtos e serviços.

## Como Segmentar Clientes? 
A segmentação de clientes exige que uma empresa colete informações específicas - dados - sobre clientes e analise-as para identificar padrões que podem ser usados para criar segmentos.

Parte disso pode ser obtida a partir de informações de compra - cargo, geografia, produtos adquiridos, por exemplo. Algumas delas podem ser obtidas da forma como o cliente entrou no seu sistema. Um profissional de marketing que trabalha com uma lista de e-mail de inscrição pode segmentar mensagens de marketing de acordo com a oferta de inscrição que atraiu o cliente, por exemplo. Outras informações, no entanto, incluindo dados demográficos do consumidor, como idade e estado civil, precisarão ser adquiridas de outras maneiras.

Os métodos típicos de coleta de informações incluem:
- Entrevistas presenciais ou por telefone
- Pesquisas
- Coleta de informações publicadas sobre categorias de mercado
- Grupos de foco
- Dados de acesso a sistemas ou apps

## Usando Segmentos de Clientes
Características comuns nos segmentos de clientes podem orientar como uma empresa comercializa segmentos individuais e quais produtos ou serviços ela promove. A segmentação de clientes pode ser praticada por todas as empresas, independente do tamanho ou setor, e se vendem on-line ou presencialmente. Começa com a coleta e a análise de dados e termina com a atuação nas informações coletadas de maneira apropriada e eficaz, com a entrega das conclusões.

## Marketing Analytics também é:
- Market Basket Analysis - Extração de regras de associação -> https://github.com/EricPassosScience/Market_Basket_Analysis/blob/main/README.md
- Teste A/B
- Análise de KPIs
- Text Analytics

# Segmentação de clientes de uma rede de Food Delivery
Criaremos um conjunto de dados fictício para segmentar clientes com base na quantidade de produtos adquiridos e localidade. O script em pyton é bem simples, mas serve de base para diversos trabalhos.

## Dicionário de Dados
- id_transação <- ID da transação. Um mesmo ID pode ter vários itens de pedidos.
- horario_pedido <- Horário exato do pedido
- localidade <- Localidade que processou o pedido (unidade do restaurante)
- nome_item <- Nome do item (pizza, salada, bebida e sobremesa)
- quantidade_item <- Quantidade de itens no pedido
- Latitude <- Latitude da localidade onde o pedido foi gerado
- Longitude <- Longitude da localidade onde o pedido for gerado
