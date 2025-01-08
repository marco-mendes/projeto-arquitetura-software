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

Para reduzir o seu viés (e o meu também), sempre recomendo usar um ADR (Registro De Decisões Arquiteturais). Veja [nesse guia aqui](https://github.com/marco-mendes/projeto-arquitetura-software/blob/main/1.4%20ADR.md) como racionalizar as suas decisões.


 *(Em construção)*
