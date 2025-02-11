# O Projeto da Arquitetura de Software
Compilo aqui um conjunto de recursos para a preparação de um projeto de arquitetura de software, bem como um processo para "arquitetar software". 

O processo que aqui descrevo irá seguir essa estrutura didática, que você pode e deve adaptar para a sua realidade.

<img width="602" alt="image" src="https://github.com/user-attachments/assets/ac5cb1bc-ee7e-4914-b757-3a354eafecbf" />


---

## Introdução
Primeiramente, arquitetos devem participar desde os primeiros momentos de um projeto. O envolvimento tardio de um arquiteto é uma receita para exposição ao risco e ao fracasso, como posso atestar por experiência própria.

Se você não é um arquiteto ou deseja entender o que é uma arquitetura de software e o que um arquiteto faz, preparei [esse guia](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/1.0%20O%20que%20é%20arquitetura%20e%20quem%20e%20o%20arquiteto.md) aqui para você.

## Coleta de Requisitos e Definição do Escopo da Arquitetura
Uma vez embarcado, arquitetos devem realizar um trabalho diligante junto aos seus Product Owners/Analistas de Negócio para captura requisitos não-funcionais (atributros de qualidade) e selecionar, a partir dos requisitos funcionais e não-funcionais, aquele subconjunto de requisitos que irão ser classificdos como arquiteturais. 

Spoiler: Nem todo requisito não-funcional é arquitetural. E alguns requisitos arquiteturais podem ser funcionais.

Leia os guias abaixo para entender o que são requisitos arquiteturais e requisitos não-funcionais (atributos de qualidade).

- [Guia 1 - Requisitos Arquiteturais](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/1.1%20Requisitos%20Arquiteturais.md)

- [Guia 2 - Requisitos Não-Funcionais](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/1.2%20Requisitos%20Não-Funcionais.md)

## Definição do Estilo (ou estilos) Arquiteturais

O estilo arquitetural é a maior definição no projeto de uma arquitetura de software. Ele representa uma abordagem estratégica para projetar, implementar e distribuir uma aplicação. Dentro do campo da arquitetura de software para TI, existem diversos estilos arquiteturais disponíveis, cada um com suas próprias vantagens e desvantagens.

Exemplos de estilos comuns no mercado incluem MVC, MVVM, Eventos, Microkernel, API, Serviços ou Nuvem. O guia abaixo traz mais informações sobre estilos arquiteturais.

- [Guia 3 - Estilos Arquiteturais](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/1.3%20Estilos%20Arquiteturais.md)

## Racionalizando a Escolha do Estilo

Uma arquitetura complexa pode ser vários estilos arquiteturais combinados. E tudo bem. Por exemplo, podemos ter uma arquitetura Web com estilos de eventos e nuvem. Agora, é importante que a sua escolha não seja emocional. Ela deve ser racional.

Já observei arquitetos escolhendo estilos e plataformas baseado puramente na preferência emocional, o que pode resultar em riscos expostos e bombas relógios para as organizações onde eles trabalham.

Para reduzir o seu viés (e o meu também), sempre recomendo usar um ADR (Registro De Decisões Arquiteturais). Veja [nesse guia aqui](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/2.1%20ADR.md) como racionalizar as suas decisões.

## Descrição das Visões de Arquitetura

O arquiteto pode descrever a sua arquitetura através de desenhos e esquemas. Uma abordagem simples é o uso da modelagem C4.

Veja [esse guia aqui](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.1%20Modelagem%20C4.md) para rever o que é a modelagem C4.

Depois examine os detalhes dos níveis C1, C2 e C3 nesses guias aqui:

* [Modelagem do nivel C1](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.2%20%20N%C3%ADvel%20C1%20-%20Diagrama%20de%20Contexto.md)
* [Modelagem do nivel C2](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.3%20Nivel%20C2%20-%20Diagrama%20de%20Conteineres.md)
* [Modelagem do nivel C3](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.4%20N%C3%ADvel%20C3%20-%20Diagrama%20de%20Componentes.md)

Preparei alguns exemplos simples de modelagem para sua referência [nesse guia aqui](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.5%20Exemplo%20C1,%20C2%20e%20C3%20de%20um%20Internet%20Banking.md).

Adicionalmente, mostro como modelar estilos arquiteturais com a notação C4:

* [Modelagem de microsserviços com C4](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.6%20Modelagem%20de%20Microsservi%C3%A7os.md)
* [Modelagem de microsserviços com comunicação assíncrona Kafka](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.7%20Modelagem%20de%20microsservicos%20com%20comunicacao%20ass%C3%ADncrona.md)
* [Modelagem de microsserviços com comunicação assíncrona Kafka e gateway de API](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/3.8%20Microsservicos%20Kafka%20e%20Gateway%20de%20API.md)


## Definição da Plataforma Arquitetural 

Com o estilo escolhido e justificado, agora você parte para definir a plataforma arquitetural. A plataforma arquitetural representa a maior decisão tecnonlógica em uma arquitetura de software e represente a materiaização de um ou mais estilos arquiteturais. Na prática, ela é composta pelos frameworks, bibliotecas, componentes e práticas técnicas que irão realizar o seu estilo.

Veja aqui um [guia de plataformas](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/2.2%20Plataforma%20Arquitetural.md),  onde trago exemplos práticos de plataformas para vários domínios.

 ## Detalhamento das Táticas Arquiteturais

Uma tática arquitetural é uma abordagem estruturada para atender a um ou mais requisitos arquiteturais significativos, sejam eles funcionais ou não-funcionais, como desempenho, segurança, disponibilidade ou manutenção. Essas táticas combinam decisões tecnológicas derivadas de Registros de Decisões Arquiteturais (ADRs) com considerações específicas do contexto de um projeto. Elas representam soluções reutilizáveis para problemas recorrentes e ajudam a padronizar a implementação de sistemas complexos, promovendo consistência e clareza durante o ciclo de vida do software.

[Veja esse guia aqui](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/4.1%20T%C3%A1ticas%20Arquiteturais.md) para rever o conceito de táticas arquiteturais.
E veja aqui um exemplo de uma [tática arquitetural bem descrita](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/4.2%20Exemplo%20robusto%20de%20t%C3%A1tica%20arquitetural.md).

## Identificação e Resposta a Riscos Arquiteturais

Os arquitetos de software desempenham um papel crítico ao colaborar com gestores de projeto para identificar, classificar e mitigar riscos arquiteturais. Estes riscos estão relacionados a cenários projetados de problemas futuros que podem impactar a qualidade, o desempenho e a entrega de sistemas de software.

Veja [esse guia aqui](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/4.3%20Riscos%20Arquiteturais.md) para entender como arquitetos podem identificar e descrever riscos arquiteturais.

Depois, estude como montar um [plano de resposta de riscos de arquitetura](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/4.3%20Riscos%20Arquiteturais.md) em formato 5W1H com esse guia aqui.
