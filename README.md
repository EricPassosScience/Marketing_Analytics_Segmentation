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

## Análise de Cluster
Para fazer a clusterização utilizaremos o algoritmo mais utilizado por conta da sua usabilidade, o K-means.
Documentation -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html

## Algoritmo 
O k-Means Clustering é um algoritmo de aprendizado de máquina não supervisionado. Em contraste com algoritmos tradicionais de aprendizado de máquina supervisionado, o K-Means tenta classificar dados sem antes ter sido treinado com dados rotulados.

K-Means é provavelmente o algoritmo de agrupamento mais conhecido e fácil de entender e implementar. Vejamos:
- Para começar, primeiro selecionamos um número de classes / grupos que desejamos e inicializamos aleatoriamente seus respectivos pontos centrais (centróides). Para descobrir o número de classes a serem usadad, é bom dar uma olhada rápida nos dados e tentar identificar grupos distintos.
- Cada ponto de dados é classificado calculando a distância entre esse ponto e cada centro de grupo e, em seguida, classificando o ponto no grupo cujo centro está mais próximo.
- Com base nesses pontos classificados, recalculamos o centro do grupo, calculando a média de todos os vetores do grupo.
- Repetimos essas etapas para um número definido de iterações ou até que os centros dos grupos não alterem muito entre as iterações. Você também pode optar por inicializar aleatóriamente os centros do grupo algumas vezes e selecionar a execução que parece ter fornecido os melhores resultados. O K-Means tem a vantagem de ser muito rápido, pois estamos realmente calculando as distâncias entre pontos e centros de grupos; são poucos cálculos! Portanto, possui uma complexidade linear O(n).

Por outro lado, o K-Means tem algumas desvantagens. Primeiro, você deve selecionar quantos grupos / clusters. Isso nem sempre é trivial e, idealmente, com um algoritmo de agrupamento, queremos que ele os descubra, porque o objetivo é obter algumas informações dos dados.

O K-means também começa com uma escolha aleatória de centros de cluster e, portanto, pode produzir resultados de cluster diferentes em execuções diferentes do algoritmo. Assim, os resultados podem não ser repetíveis e não têm consistência. Outros métodos de cluster são mais consistentes.

K-Medians é outro algoritmo de agrupamento relacionado ao K-Means, exceto que, em vez de recalcular os pontos centrais do grupo usando a média, usamos o vetor de medianas do grupo. Esse método é menos sensível a outliers (por causa do uso da Mediana), mas é muito mais lento para conjuntos de dados maiores, pois a classificação é necessária em cada iteração ao calcular o vetor Mediana.

### Outros algoritmos de Clusterização: 
- Mean-Shift Clustering -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.MeanShift.html
- Density-Based Spatial Clustering of Applications with Noise (DBSCAN)- (dados com ruídos/erros - o ruído não vai unfluenciar no agrupamento) -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html
- Expectation–Maximization (EM) Clustering using Gaussian Mixture Models (GMM) - > https://scikit-learn.org/stable/modules/mixture.html
- Agglomerative Hierarchical Clustering -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html

## Métricas de Clusterização
## Interpretação
Examine o número de observações em cada cluster ao interpretar as medidas de variabilidade, como a distância média e a soma dos quadrados dentro do cluster. A variabilidade de um cluster pode ser afetada por ter um número menor ou maior de observações. Por exemplo, a soma dos quadrados dentro do cluster se torna maior à medida que mais observações são adicionadas.

Examine os clusters que possuem significativamente menos observações que outros clusters. Clusters que têm poucas observações podem conter discrepâncias ou observações incomuns com características únicas.

Ainda temos as seguintes métricas: distância média do centróide, distância máxima do centróide, centróide do cluster, distâncias entre os centróides do cluster.

Referência - > https://www-users.cse.umn.edu/~kumar001/dmbook/ch8.pdf

## Español

## Concepto
Marketing Analytics comprende los procesos y tecnologías que permiten a los especialistas en marketing medir el éxito de sus iniciativas.

Esto se hace midiendo el rendimiento de las campañas de marketing, recopilando los datos y analizando los resultados. Marketing Analytics aprovecha las métricas comerciales clave, como el retorno de la inversión (ROI), la atribución de marketing y la eficacia general de marketing. En otras palabras, Marketing Analytics muestra si los programas de Marketing están siendo efectivos o no.

Marketing Analytics reúne datos de todos los canales de marketing y los consolida en una vista de marketing común. A partir de esa vista común, puede extraer resultados analíticos que pueden brindar una asistencia invaluable para impulsar los esfuerzos de marketing.

## ¿Por qué es importante la analítica de marketing?

A lo largo de los años, a medida que las empresas se expandieron a nuevas categorías de marketing, se adoptaron nuevas tecnologías para respaldarlas. Como cada nueva tecnología se implementaba normalmente de forma aislada, el resultado era un revoltijo de entornos de datos desconectados.

Como resultado, los especialistas en marketing a menudo toman decisiones basadas en datos de canales individuales (marketing digital y métricas de sitios web, por ejemplo) sin considerar todo el panorama de marketing. Los datos de las redes sociales por sí solos no son suficientes. Los datos de análisis web por sí solos no son suficientes. Y las herramientas que solo analizan una instantánea de tiempo de un solo canal son lamentablemente inadecuadas.

Marketing Analytics, por otro lado, considera todos los esfuerzos de marketing en todos los canales durante un período de tiempo, lo cual es esencial para tomar las decisiones correctas y ejecutar de manera eficiente las campañas e iniciativas de marketing de una empresa.

## ¿Qué podemos hacer con Marketing Analytics?
Con Marketing Analytics, podemos responder preguntas como estas:
- ¿Cómo están nuestros esfuerzos de marketing hoy? ¿Qué tal a largo plazo? ¿Qué podemos hacer para mejorarlos?
- ¿Cómo se comparan nuestras actividades de marketing con las de nuestros competidores? ¿Dónde están gastando su tiempo y dinero? ¿Están usando canales que nosotros no estamos usando?
- ¿Qué debemos hacer a continuación? ¿Están nuestros recursos de marketing asignados correctamente? ¿Estamos dedicando tiempo y dinero a los canales correctos? ¿Cómo debemos priorizar nuestras inversiones para el próximo año?
- ¿Cuál es el perfil de nuestros clientes? ¿Son de la misma área regional? ¿Tienes los mismos gastos y preferencias?
- ¿Puedo segmentar a mis clientes por similitud? ¿Cómo puedo saber los gastos por grupo?
- Y muchos otros...

## ¿Qué es la segmentación de clientes?
La segmentación de clientes es el proceso de dividir a los clientes en grupos en función de características comunes, de modo que las empresas puedan comercializar a cada grupo de manera efectiva y adecuada, o simplemente comprender los patrones de consumo de los clientes.

## Marketing B2B frente a marketing B2C
En el marketing Business-to-Business (B2B), una empresa puede segmentar a los clientes de acuerdo con una amplia variedad de factores, que incluyen:
- Industria
- Número de empleados
- Productos comprados previamente a la empresa
- Ubicación

En el marketing Business-to-Consumer (B2C), las empresas segmentan a los clientes según la demografía y los patrones de consumo, como:
- Edad
- Género
- Estado civil
- Ubicación (urbana, suburbana, rural)
- Etapa de vida (sin hijos, jubilado, etc.)
- Productos comprados
- Cantidad gastada
- Tiempo de consumo

## ¿Por qué segmentar clientes?
La segmentación permite a los especialistas en marketing adaptar mejor sus esfuerzos de marketing a varios subconjuntos de audiencias objetivo. Estos esfuerzos pueden estar relacionados con las comunicaciones y el desarrollo de productos. Específicamente, la segmentación ayuda a una empresa a:

- Crear y comunicar mensajes de marketing dirigidos que resonarán en grupos específicos de clientes, pero no en otros (que recibirán mensajes adaptados a sus necesidades e intereses).
- Seleccione el mejor canal de comunicación para el segmento, que puede ser correo electrónico, publicaciones en redes sociales, públicamente en la radio u otro enfoque, según el segmento.
- Identificar formas de mejorar productos o nuevas oportunidades para productos o servicios.
- Establecer mejores relaciones con los clientes.
- Probar opciones de precios.
- Centrarse en los clientes más rentables.
- Mejora del servicio al cliente.
- Elegir entre venta al por mayor y venta cruzada de otros productos y servicios.

## ¿Cómo segmentar clientes?
La segmentación de clientes requiere que una empresa recopile información específica (datos) sobre los clientes y la analice para identificar patrones que puedan usarse para crear segmentos.

Parte de esto se puede obtener de la información de compra: título, geografía, productos comprados, por ejemplo. Algunos de estos se pueden obtener de cómo el cliente ingresó a su sistema. Un especialista en marketing que trabaja con una lista de correo electrónico de registro puede segmentar los mensajes de marketing de acuerdo con la oferta de registro que atrajo al cliente, por ejemplo. Sin embargo, otra información, incluida la demografía del consumidor, como la edad y el estado civil, deberá adquirirse de otras maneras.

Los métodos típicos de recopilación de información incluyen:
- Entrevistas presenciales o telefónicas
- Investigaciones
- Recopilación de información publicada sobre categorías de mercado.
- Grupos de enfoque
- Acceder a datos a sistemas o aplicaciones.

## Uso de segmentos de clientes
Las características comunes entre los segmentos de clientes pueden guiar cómo una empresa comercializa segmentos individuales y qué productos o servicios promueve. La segmentación de clientes puede ser practicada por todas las empresas, independientemente de su tamaño o sector, y de si venden online o de forma presencial. Comienza con la recolección y análisis de datos y finaliza con actuar sobre la información recolectada de manera adecuada y eficaz, con la entrega de conclusiones.

## Marketing Analytics también es:
- Análisis de cesta de la compra - Extracción de reglas de asociación -> https://github.com/EricPassosScience/Market_Basket_Analysis/blob/main/README.md
- Pruebas A/B
- Análisis de KPI
- Text Analytics 

# Segmentación de clientes de una red de Food Delivery
Crearemos un conjunto de datos ficticio para segmentar a los clientes según la cantidad de productos comprados y la ubicación. El script en pyton es muy sencillo, pero sirve de base para varios trabajos.

## Diccionario de datos
- id_transacción <- ID de transacción. Un único ID puede tener varios artículos de pedido.
- horario_pedido <- Hora exacta del pedido
- ubicación <- Ubicación que procesó el pedido (unidad de restaurante)
- item_name <- Nombre del artículo (pizza, ensalada, bebida y postre)
- item_quantity <- Cantidad de artículos en el pedido
- Latitud <- Latitud de la ubicación donde se generó el pedido
- Longitud <- Longitud de la ubicación donde se genera el pedido

## Análisis de conglomerados
Para realizar el agrupamiento utilizaremos el algoritmo más utilizado por su usabilidad, el K-means.
Documentación -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html

## Algoritmo
k-Means Clustering es un algoritmo de aprendizaje automático no supervisado. A diferencia de los algoritmos tradicionales de aprendizaje automático supervisado, K-Means intenta clasificar los datos sin ser entrenado primero en datos etiquetados.

K-Means es probablemente el algoritmo de agrupación en clústeres más conocido y es fácil de entender e implementar. Vamos a ver:
- Para empezar, primero seleccionamos el número de clases/grupos que queremos e inicializamos aleatoriamente sus respectivos puntos centrales (centroides). Para calcular el número de clases a utilizar, es bueno echar un vistazo rápido a los datos e intentar identificar grupos distintos.
- Cada punto de datos se ordena calculando la distancia entre ese punto y cada centro de grupo y luego ordenando el punto en el grupo cuyo centro está más cercano.
- En base a estos puntos clasificados, recalculamos el centro del grupo, promediando todos los vectores del grupo.
- Repetimos estos pasos para un número determinado de iteraciones o hasta que los centros de clúster no cambien mucho entre iteraciones. También puede optar por inicializar aleatoriamente los centros del grupo varias veces y seleccionar la ejecución que parece haber dado los mejores resultados. K-Means tiene la ventaja de ser muy rápido, ya que en realidad estamos calculando las distancias entre puntos y centros de conglomerados; ¡Son solo algunos cálculos! Por lo tanto, tiene una complejidad lineal O(n).

Por otro lado, K-Means tiene algunos inconvenientes. Primero, debe seleccionar cuántos grupos/clústeres. Esto no siempre es trivial, e idealmente con un algoritmo de agrupamiento queremos que los resuelva, porque el objetivo es obtener información de los datos.

K-means también comienza con una elección aleatoria de centros de conglomerados y, por lo tanto, puede producir diferentes resultados de conglomerados en diferentes ejecuciones del algoritmo. Por lo tanto, los resultados pueden no ser repetibles y carecer de consistencia. Otros métodos de agrupamiento son más consistentes.

K-Medians es otro algoritmo de agrupamiento relacionado con K-Means, excepto que en lugar de volver a calcular los puntos centrales del clúster usando la media, usamos el vector de la mediana del clúster. Este método es menos sensible a los valores atípicos (debido al uso de la mediana), pero es mucho más lento para conjuntos de datos más grandes, ya que se requiere ordenar en cada iteración al calcular el vector de la mediana.

### Otros algoritmos de agrupamiento:
- Agrupación de desplazamiento medio -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.MeanShift.html
- Agrupación espacial basada en densidad de aplicaciones con ruido (DBSCAN)- (datos con ruido/errores; el ruido no dejará de influir en la agrupación) -> https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html
- Agrupación de expectativas-maximización (EM) utilizando modelos de mezcla gaussiana (GMM) - > https://scikit-learn.org/stable/modules/mixture.html
- Agrupación jerárquica aglomerativa ->https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html

## Métricas de agrupamiento
## Interpretación
Examine el número de observaciones en cada conglomerado al interpretar medidas de variabilidad como la distancia media y la suma de cuadrados dentro del conglomerado. La variabilidad de un conglomerado puede verse afectada por tener un número mayor o menor de observaciones. Por ejemplo, la suma de los cuadrados dentro del conglomerado aumenta a medida que se agregan más observaciones.

Examine los conglomerados que tienen significativamente menos observaciones que otros conglomerados. Los conglomerados que tienen pocas observaciones pueden contener valores atípicos u observaciones inusuales con características únicas.

Todavía tenemos las siguientes métricas: distancia de centroide promedio, distancia de centroide máxima, centroide de clúster, distancias entre centroides de clúster.

Referencia -> https://www-users.cse.umn.edu/~kumar001/dmbook/ch8.pdf
