# Web scraping to gain company insights

## Contexto e objetivo
Na era atual, em que os consumidores se tornaram cada vez mais críticos e exigentes na decisão de compra, é fundamental que as empresas adotem uma abordagem centrada no cliente para se manterem competitivas no mercado. Para isso, é essencial ouvir o que os clientes valorizam e sentem em relação à empresa, coletando dados relevantes que direcionem ações e melhorias internas, a fim de aprimorar a experiência do cliente e aumentar o valor percebido da marca.

No âmbito do meu projeto de portfólio, propus uma iniciativa focada na companhia aérea British Airways. O objetivo principal é extrair informações valiosas de comentários e notas atribuídas à empresa em um site público, utilizando técnicas avançadas de WebScrapping para coletar de forma eficiente os feedbacks dos clientes que utilizaram os serviços da companhia. Além disso, vou empregar métodos de análise de dados para obter uma visão detalhada da percepção dos clientes em relação aos serviços prestados pela empresa.

O site no qual os dados estão disponíveis pode ser acessado pelo seguinte [link](https://www.airlinequality.com/)

## Definição de método e observações

### Exemplo de estrutura do comentário no site
![Texto Alternativo](modelo_comentario.png)

### Lógica de desenvolvimento

O algoritmo funciona coletando dados de comentários de clientes em um site específico. Cada comentário possui um ID representado por `anchor######` na página HTML, e os dados são coletados seguindo um formato estruturado.

A coleta de dados ocorre em duas partes:

1. **Informações básicas**: Essa parte inclui o score geral, data do comentário, texto resumo destacado e o comentário completo feito pelo cliente.

2. **Informações analíticas**: Nessa parte, são coletados atributos específicos, como modelo da aeronave, tipo de viajante, classe de viagem e data do voo. Além disso, são coletadas avaliações de atributos, como conforto do assento, serviço de bordo, comidas e bebidas, entretenimento de voo, serviço de solo e custo-benefício. Também é coletada uma marcação indicando se o cliente recomendaria a empresa ou não.

Essas informações são coletadas por meio de funções separadas para cada página e, posteriormente, compiladas em um formato tabular. Os dados podem ser analisados tanto no ambiente Python quanto exportados para o Excel para serem tratados e visualizados usando ferramentas como o Power BI para criar visuais analíticos.

Essa abordagem permite uma análise aprofundada dos comentários dos clientes, fornecendo insights valiosos sobre a percepção geral dos serviços prestados pela empresa. Os dados podem ser explorados de maneira flexível, permitindo a aplicação de técnicas analíticas avançadas como análise de sentimento e a criação de visualizações interativas para uma melhor compreensão dos resultados.
