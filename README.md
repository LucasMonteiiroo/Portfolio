<h1>Pedro Lucas dos Santos Rodrigues</h1>

<h2>Projeto 1: 2º Semestre de 2020</h2>
<H3> Easy Way </H3>
<H4> Interno - FATEC </H4>
<img width="250" src="imagens/Quadrados_Pretos_e_Brancos_Industrial_Logotipo.png">
<h3>Descrição do Projeto</h3>
O aplicativo "Easy Way" visa resolver os problemas enfrentados pelos motoristas de vans em relação ao gerenciamento de rotas e tempo de viagem. Muitas vezes, os motoristas enfrentam dificuldades quando os usuários não comunicam previamente sua intenção de utilizar o serviço, resultando em perda de tempo e gastos extras. Além disso, quando os usuários comunicam, ainda há a necessidade de ajustar as rotas, o que também consome tempo. Portanto, o VanConnect é uma solução que visa otimizar esses processos, garantindo uma experiência mais eficiente para motoristas e passageiros.

<h3>Tecnologias Utilizadas</h3>
<h4>AppInventor</h4>
<img width="250" src="imagens/AppInventor.png">

O App Inventor é uma ferramenta de desenvolvimento de aplicativos para Android criada pelo Google e agora mantida pelo MIT. Ele permite que pessoas sem conhecimento avançado em programação criem aplicativos móveis usando uma interface gráfica intuitiva de arrastar e soltar, tornando o desenvolvimento de aplicativos mais acessível para uma variedade de usuários.

<h4>Firebase</h4>
<img width="250" src="imagens/Firebase.jpg">
O Firebase é uma plataforma de desenvolvimento de aplicativos oferecida pelo Google, que fornece uma variedade de serviços úteis, como armazenamento em nuvem, autenticação de usuários e banco de dados em tempo real. Ele simplifica o desenvolvimento de aplicativos, permitindo que os desenvolvedores se concentrem na lógica do aplicativo, enquanto o Firebase cuida da infraestrutura de back-end.

## Contribuições pessoais
Por ser o primeiro projeto, dediquei meu tempo aos estudos e trabalhar em conjunto com o time de desenvolvimento da equipe, atuando principalmente na parte logica o AppInventor para construir tanto a interface grafica quanto suas funcionalidades. Atuei na construção de métodos para expor os dados de maneira clara e organizada.

<h2>Projeto 2: 1º Semestre de 2022</h2>

### Empresa parceira  

<p align="center">
    <b>Dom Rock</b>
</br>
    <img src="https://github.com/alantrs/Bertoti/blob/efd7a4e3055f78276feb65f55b0702623e0f2636/metodologia/Imagens/domrock2.png" alt="Logo dom rock">
</p>


## Descrição do projeto

Este projeto visa gerenciar a ativação de clientes na plataforma Dom Rock.

A solução proposta concentra-se na entrada de dados, incluindo parâmetros e variáveis específicas de cada cliente, para efetuar a alocação adequada de recursos na plataforma. A abordagem inclui a estimativa de consumo de recursos, considerando fatores como o volume de dados do cliente e o número de usuários. Adicionalmente, a solução é projetada para gerar relatórios e consultas. 

## Tecnologias utilizadas

- **Java**: Linguagem orientada a objetos, foi escolhida para o desenvolvimento do back-end devido à familiaridade prévia da equipe, ampla utilização no mercado e extensa documentação, facilitando a implementação do projeto.

- **PostgreSQL**: PostgreSQL é um sistema de gerenciamento de banco de dados relacional de código aberto que é amplamente utilizado em aplicações empresariais e científicas, devido à sua confiabilidade, escalabilidade e recursos avançados. Além disso, o PostgreSQL é compatível com muitas linguagens de programação, incluindo Java, que foi usada neste projeto.

## Contribuições pessoais

Fui o administrador do banco de dados da equipe. Desenvolvi a modelagem de dados e a criação da base de dados por completo. Ajudei a equipe de backend sendo solicitado por melhorias na distribuição dos dados promovendo a maior facilidade para manipulação dos mesmos.
<br>
    <details>
<summary><b>Modelagem do banco de dados</b></summary>
<br>
        
Nesse projeto, o objetivo da modelagem de dados foi representar os dados inseridos pelo cliente e como seria distribuido na nossa base. Utilizei o Modelo Entidade-Relacionamento (MER) como uma representação visual para entender a distribuição das tabelas com seus atributos e relacionamento entre elas.

![Modelagem do banco de dados](https://github.com/alantrs/Bertoti/blob/778fd69f6e9fecddd2342af75295ff9542562f1e/metodologia/Imagens/modelagem-domrock.jpeg)
</details>

<details>
      <summary><b>Implementação física do banco de dados</b></summary>
      <br>
    A implementação física é uma etapa fundamental na modelagem de dados, pois envolve a tradução do modelo conceitual em uma estrutura de dados real e eficiente para armazenar e processar os dados em um sistema de banco de dados. Ela é importante para garantir a eficiência, a integridade, a segurança e o desempenho do banco de dados, bem como sua escalabilidade e facilidade de manutenção.

    ```SQL
    CREATE TABLE public.produto
    (
        solucao character varying COLLATE pg_catalog."default" NOT NULL,
        nome_produto character varying COLLATE pg_catalog."default" NOT NULL,
        id_produto serial NOT NULL,
        CONSTRAINT produto_pkey PRIMARY KEY (id_produto),
        CONSTRAINT produto_nome_produto_key UNIQUE (nome_produto)
    
    )
    
    CREATE TABLE public.funcionalidade
    (
        id_funcionalidade serial NOT NULL,
        nome_funcionalidade character varying COLLATE pg_catalog."default" NOT NULL,
        CONSTRAINT funcionalidade_pkey PRIMARY KEY (id_funcionalidade),
        CONSTRAINT funcionalidade_nome_funcionalidade_key UNIQUE (nome_funcionalidade)
    
    )
    	
    CREATE TABLE public.core
    (
        id_core serial NOT NULL,
        nome_core character varying COLLATE pg_catalog."default" NOT NULL,
        
        CONSTRAINT core_pkey PRIMARY KEY (id_core),
        CONSTRAINT core_nome_core_unique UNIQUE (nome_core)
    
    )
    ```
    
 </details>

## Aprendizados efetivos

Aprendi a base para criar um banco de dados. Como iniciar uma modelagem de dados, definir cardinalidades e tranformar o modelo conceitual em script SQL. Aprendi alguns comandos básicos para trabalhar com versionamento de código com Git.

### Hard Skills

<details>
  <summary><b>Recursos básicos de Banco de dados: sei fazer com autonomia</b></summary>
    <br>
  <ul>
    <li>Estrutura do banco, distribuição das tabelas</li>
    <Li>Modelo conceitual, Modelo lógico e Modelo físico</Li>
    <Li>Criar script</Li>
    <Li>Realizar querys simples</Li>
  </ul>
 </details>

 <details>
  <summary><b>Git: sei fazer com autonomia</b></summary>
     <br>
  <ul>
    <li>Comandos básicos: git add, git commit, git pull, git push</li>
    <Li>Criar branches</Li>
  </ul>
 </details>

### Soft Skills

<details>
  <summary><b>Adaptação</b></summary>
  <br>
  <ul>
    <li>Lidar com uma equipe totalmente nova exigiu rápida adaptação e flexibilidade para nos ajustarmos ao ambiente e às dinâmicas de trabalho. A capacidade de ser flexível e adaptável foi essencial para responder de forma eficaz às mudanças e desafios que surgiram, permitindo-nos manter o foco no objetivo final e atender às necessidades do cliente de maneira ágil e eficiente</li>
  </ul>
</details> 
<details>
  <summary><b>Aprendizado contínuo</b></summary>
  <br>
  <ul>
    <li>A partir desse semetre foi introduzido a tecnologia de banco de dados para a aplicação a ser desenvolvida, e foi necessário estudar para aprender sobre SQL e sobre PostgreSQL.</li>
  </ul>
</details> 
<hr>

<h2>Projeto 3: 2º Semestre de 2022</h2>
<h3>Parceiro Acadêmico</h3>
<img width="250" src="https://www.iacit.com.br/imgs/meta-image.jpg">

<h3>Descrição do Projeto</h3>
Foi criado um sistema avançado para o manejo eficiente de dados meteorológicos, com recursos de importação, pesquisa e geração de relatórios. Além disso, o sistema integra-se de forma automatizada ao banco de dados desenvolvido para ter a maior eficiencia no gerenciamento do mesmo, permitindo a obtenção e armazenamento dos dados disponibilizados por eles. A interface web do sistema oferece uma ampla gama de opções de filtragem, possibilitando a seleção precisa dos registros com base em datas, regiões, estados, localidades e tipos de dados específicos. A apresentação dos dados é realizada por meio de gráficos visualmente atrativos, e os usuários têm a opção de exportar um relatório personalizado com base na consulta efetuada. Esse sistema oferece uma solução completa para o acompanhamento e análise detalhada das condições meteorológicas, com facilidade de acesso e uso intuitivo.

<h3>Tecnologias Utilizadas</h3>

<h4>PostgreSQL</h4>
<img  width="250" src="https://www.luiztools.com.br/wp-content/uploads/2021/02/postgres.jpg">
O sistema utiliza o PostgreSQL como banco de dados principal para armazenar e gerenciar as informações. O PostgreSQL é uma escolha confiável para lidar com grandes volumes de dados meteorológicos. Ele oferece recursos avançados de consulta e recuperação eficiente dos dados. Além disso, o PostgreSQL possui medidas de segurança abrangentes, como controle de acesso e permissões, para proteger as informações armazenadas, que foi amplamente utilizados no projeto. Sua utilização garante a integridade e consistência dos dados, proporcionando um ambiente confiável para o sistema.
<h4>Java Spring</h4>
<img  width="250" src="https://4.bp.blogspot.com/-ou-a_Aa1t7A/W6IhNc3Q0gI/AAAAAAAAD6Y/pwh44arKiuM_NBqB1H7Pz4-7QhUxAgZkACLcBGAs/s1600/spring-boot-logo.png">
O back end do sistema foi desenvolvido usando o Java Spring. O Java Spring é um framework poderoso que nos permite criar a lógica e manipular os dados do banco de dados de forma centralizada. Ele facilita o processamento das solicitações, o acesso aos dados e a implementação das regras de negócio. Com o Java Spring, podemos importar os dados meteorológicos, realizar pesquisas e filtragens, gerar relatórios e disponibilizar os dados para a interface web. Além disso, ele facilita a integração com o PostgreSQL, garantindo um acesso eficiente aos dados armazenados. O uso do Java Spring torna o desenvolvimento do back end mais organizado e eficiente, permitindo uma manipulação otimizada dos dados.
  
  <h4>JavaScript</h4>

  <img  width="250" src="https://static.javatpoint.com/images/javascript/javascript_logo.png">
  
JavaScript é uma linguagem de programação amplamente utilizada no desenvolvimento web. Ela oferece interatividade e dinamismo às páginas, permitindo a manipulação de elementos HTML, estilos CSS e a interação com o usuário. Uma das vantagens do JavaScript é sua capacidade de ser executado em diferentes plataformas, independentemente do sistema operacional. Além disso, JavaScript evoluiu ao longo dos anos, com a criação de bibliotecas e frameworks que facilitam o desenvolvimento de aplicações web mais complexas. Um exemplo disso é o REST (Representational State Transfer), uma arquitetura para criação de APIs que utiliza os princípios da web e é compatível com JavaScript. Com o uso do REST, é possível construir aplicações web escaláveis, flexíveis e de fácil integração com outros sistemas.


  <h4>Chart.js</h4>
  <img  width="250" src="https://avatars.githubusercontent.com/u/10342521?s=280&v=4">

A biblioteca Chart.js é uma poderosa ferramenta em JavaScript para exibir dados em forma de gráficos em páginas da web. No nosso projeto, essa biblioteca desempenhou um papel fundamental na interface, permitindo que apresentássemos os dados meteorológicos selecionados e filtrados de maneira interativa para os usuários. Além disso, com o Chart.js, tivemos a flexibilidade de personalizar as propriedades de design dos gráficos, possibilitando a exibição personalizada de diferentes tipos de dados.

<h3>Contribuições Individuais</h3>

<details>
  <summary>Desenvolvimento e personalização dos endpoints no back-end.</summary>
  </br>
  Para que tudo isso sejá possivel, criamos um código que implementa uma API REST para manipulação de usuários em um sistema. A classe UsuarioController define os endpoints e os métodos que lidam com as requisições HTTP relacionadas aos usuários, como listar usuários, criar um novo usuário, editar um usuário existente e excluir um usuário.

Através desses endpoints, os clientes podem interagir com o sistema, enviando requisições para obter informações dos usuários, criar novos usuários, atualizar informações existentes e excluir usuários. O controlador utiliza a classe UsuarioService para executar a lógica de negócio relacionada aos usuários, como acessar o banco de dados, realizar validações e manipular os objetos de usuário.

Portanto, o objetivo principal do código é fornecer uma interface para a manipulação de usuários em um sistema, seguindo as práticas e convenções do padrão REST. Isso permite que os clientes interajam com o sistema de forma padronizada e eficiente, através de requisições HTTP bem definidas.

  ```java
      private UsuarioService usuarioService;
      public UsuarioController(UsuarioService usuarioService){
          this.usuarioService = usuarioService;

      }

      @GetMapping
      public ResponseEntity<List<Usuario>> listaUsuarios(){
      return ResponseEntity.status(200).body(usuarioService.listarUsuario());

      }

      @PostMapping
      public ResponseEntity<Usuario> criarUsuario(@RequestBody Usuario usuario){
          return ResponseEntity.status(201).body(usuarioService.criarUsuario(usuario));
      }

      @PutMapping()
      public ResponseEntity<Usuario> editarUsuario(@RequestBody Usuario usuario){
          return ResponseEntity.status(200).body(usuarioService.editarUsuario(usuario));
      }

      @DeleteMapping("/{id}")
      public ResponseEntity<?> excluirUsuario(@PathVariable Integer id){
          usuarioService.excluirUsuario(id);
          return ResponseEntity.status(204).build();
      }
  
  ```

</details>

<details>
  <summary>Consulta e manipulação de endpoints personalizados do backend.</summary>
  </br>
Os modelos de conexão para recuperar dados do backend:
Faz uma solicitação assíncrona para obter dados JSON do servidor.
Armazena os dados recebidos em variáveis.
Realiza iterações e manipulações nos dados para extrair informações específicas.
Atualiza o conteúdo de elementos HTML no documento com os dados processados.
Em resumo, o código está obtendo dados sobre temperaturas máximas de diferentes estações, realizando operações nos dados recebidos e exibindo os resultados no documento HTML.
  
 ```javascript

    $(document).ready(function(){
        $.getJSON("/temperatura_max",function(data){

                 var estacoes = []
                for(var i = 0; i<data.length;i++){
                if(estacoes.indexOf(data[i].estacao) == -1 || estacoes.length == 0)
                    estacoes.push(data[i].estacao)
                }
                    const inventory = data;
                    var tempMin = []
                    for(var i = 0;i<estacoes.length;i++){
                        function isCherries(fruit){
                             return fruit.estacao === estacoes[i];
                                   }
                        var usuario = inventory.find(isCherries);
                        tempMin.push(usuario)
                        }


                        $(document).ready(function(){
                                $.getJSON("/estacoes",function(data2){
                                console.log("SP dado 1: "+data2[0].nome_estacao)
                                for(var i = 0;i<5;i++){
                                    function nomeEstacao(nomear){

                                         return nomear.codigo == estacoes[i];
                                              }
                                         var esta = data2.find(nomeEstacao);
                                         const prec_data = new Date(tempMin[i].temp_data);
                                             prec_data.setDate(prec_data.getDate()+1);

                                         $("#tempMinEstacaoM"+i).prepend(esta.nome_estacao)
                                         $("#tempMinM"+i).prepend("Temperatura Mínima: "+tempMin[i].temp_min+"°C")
                                         $("#tempMaxM"+i).prepend("Temperatura Máxima: "+tempMin[i].temp_max+"°C")
                                         $("#tempMinOrvalhoMinM"+i).prepend("Ponto de Orvalho Mínimo: "+tempMin[i].temp_orvalho_min+"°C")
                                         $("#tempMinOrvalhoM"+i).prepend("Ponto de Orvalho: "+tempMin[i].temp_ponto_orvalho+"°C")
                                         $("#tempMinOrvalhoMaxM"+i).prepend("Ponto de Orvalho Máximo: "+tempMin[i].temp_orvalho_max+"°C")
                                         $("#tempDataM"+i).prepend("DATA: "+prec_data.toLocaleDateString("pt-BR"))

                                        const a = document.querySelector("#verDetalhesM"+i);
                                        a.href = "/charts=temperatura="+tempMin[i].estacao+"="+tempMin[i].temp_data+"="+tempMin[i].temp_data;
                                            }
                                    });
                                });
            });
        });

```

</details>
No projeto desenvolvido, foi implementada uma solução para armazenar dados climáticos em um banco de dados e apresentá-los por meio de gráficos interativos. Você criou o backend utilizando Java Spring Boot, responsável por gerenciar as comunicações com o banco de dados e fornecer os endpoints necessários para acessar os dados.

Além disso, você também realizou as comunicações no frontend, utilizando JavaScript para fazer requisições assíncronas para o backend e obter os dados climáticos. Por meio de filtros, os usuários têm a possibilidade de personalizar a visualização dos registros por datas, localidade e tipo de dado, permitindo uma análise mais precisa e específica.

No aspecto visual, você desenvolveu os gráficos que apresentam os dados climáticos de forma clara e compreensível. Utilizando HTML e CSS, você criou a interface necessária para exibir os gráficos e as informações relevantes relacionadas aos dados climáticos.

Em resumo, o projeto consiste em uma solução completa que engloba o desenvolvimento do backend, as comunicações no frontend e a criação dos gráficos para análise dos dados climáticos.

<h4>Aprendizados Efetivos</h4>
<details>
  <summary>Spring Framework</summary>
  <ul>
  <li>Arquitetura REST: Implementação da arquitetura REST (Representational State Transfer) para criação de APIs web.</li>
  <li>Integração com Banco de Dados: Integração da aplicação com banco de dados para armazenamento e recuperação de dados.</li>
  <li>Injeção de Dependências: Utilização do recurso de injeção de dependências do Spring para facilitar o gerenciamento de componentes e suas dependências.</li>
  <li>Desenvolvimento Orientado a Interfaces: Desenvolvimento de código seguindo o princípio de programação orientada a interfaces, que promove a modularidade e flexibilidade do sistema.</li>
  <li>Integração com Banco de Dados: Realização da integração da aplicação com banco de dados para armazenamento e recuperação de dados.</li>
  </ul>
</details>

<details>
  <summary>Banco de dados</summary>
  <ul>
  <li>Linguagem SQL: Familiarizei-me com a linguagem SQL (Structured Query Language) utilizada para manipulação e consulta de dados em bancos de dados relacionais. Aprendi a escrever consultas eficientes para recuperar e manipular informações.</li>
  <li>Bancos de Dados Relacionais: Entendi os fundamentos e características dos bancos de dados relacionais, como tabelas, chaves primárias, chaves estrangeiras, índices e normalização.</li>
  <li>Consultas com Condições: Entender como adicionar condições às consultas SQL para filtrar os resultados com base em critérios específicos.</li>
  <li>Backup e Restauração de Banco de Dados: Compreender a importância de fazer backups regulares de bancos de dados e como restaurar um backup em caso de falha.</li>
</details>

<details>
  <summary>JavaScript</summary>
  <ul>
  <li>Manipulação do DOM: Aprender a interagir com o Document Object Model (DOM) para manipular elementos HTML, como adicionar ou remover elementos, alterar conteúdo e estilos.</li>
  <li>Manipulação de Arrays: Compreender as operações básicas de manipulação de arrays, como adicionar elementos, remover elementos, percorrer e realizar transformações nos dados.</li>
  <li>AJAX e Requisições Assíncronas: Aprender a fazer requisições assíncronas usando a técnica AJAX (Asynchronous JavaScript and XML) para interagir com servidores e atualizar o conteúdo da página sem recarregá-la.</li>
  <li>Manipulação de Dados JSON: Aprender a trabalhar com dados JSON (JavaScript Object Notation), incluindo a serialização e desserialização de dados, e a interação com APIs que retornam dados nesse formato.</li>
  </ul>
</details>

# <h2>Projeto 2: 1º Semestre de 2023</h2>

### Empresa parceira

<p align="center">
    <b>Embraer</b> 
    <img src="https://github.com/alantrs/Bertoti/blob/09db3eee9ca94737bc0fc52ef7fc1313ae6cdf71/metodologia/Imagens/embraer.png" alt="Logo embraer">
</p>

## Descrição do projeto

Sistema de gerenciamento de equipamentos de voo e versões de software instalados na aeronave para pilotos freelancers.

A solução foi um sistema que armazenava todas as regras de composição de itens em um banco de dados. Quando um número de chassi era consultado, o sistema recuperava as regras de composição correspondentes desse chassi no banco de dados. Em seguida, os itens compatíveis com o chassi consultado eram exibidos na tela para o usuário.

## Tecnologias utilizadas

- **Java e Spring boot**: A linguagem Java foi utilizada para desenvolver todo o back-end da aplicação, utilizando o framework Spring Boot. O Spring Boot é uma estrutura que permite aos desenvolvedores criar rapidamente aplicativos web em Java, fornecendo um conjunto de ferramentas e bibliotecas que tornam a construção de aplicativos mais rápida e fácil.

- **Vue.js**: Vue.js é um framework de desenvolvimento web de código aberto e progressivo. Sua arquitetura centrada em componentes oferece uma abordagem modular que facilita a construção eficiente de aplicativos complexos. Utilizamos Vue.js para o frontend da aplicação.

- **Autonomous Database Oracle**: O Oracle Autonomous Database é uma solução de banco de dados em nuvem que se destaca pela automação completa, autogerenciamento e uso de machine learning. Elimina tarefas manuais, otimiza o desempenho, garante segurança e oferece escalabilidade automática, proporcionando eficiência e economia de custos. Utilizamos o autonomous database para armazenar nossa lógica de negócio.
  
- **Ambiente Cloud Oracle**: O ambiente Cloud Oracle oferece uma infraestrutura altamente escalável e eficiente para hospedar aplicativos empresariais. Utilizamos para hospedar nossa aplicação.

## Contribuições pessoais

Nesse projeto fui novamente o DBA da equipe. Desenvolvi toda estrutura da base de dados, de forma estratégica para construir um esquema robusto e que comportasse os relacionamentos complexos da melhor forma. Apliquei funções e procedures para tratamento da logica de instalação de itens em uma aeronave. Apliquei o uso de triggers para fins de auditoria para captar eventos. Apliquei o uso de views para visualização de dados.
<br>
    <details>
<summary><b>Modelagem do banco de dados</b></summary>
<br>

No caso deste projeto, o objetivo da modelagem de dados foi representar os dados de boletins de serviço, itens e chassi. Essa modelagem foi estratégica para facilitar a consulta da lógica interna de instalações de itens em uma aeronave. O objetivo central era estruturar as tabelas de maneira que exitisse uma hierarquia de condições recebidas pela empresa, facilitando assim para o backend tratar e ter códigos mais limpos e de fácil manutenção.

![Modelagem do banco de dados](https://github.com/alantrs/Bertoti/blob/7f11e2e448aaac2afb7da5aab6d272305d2051aa/metodologia/Imagens/diagrama-embraer.jpg)
</details>

<details>
<br>
<summary><b>Funções e procedures</b></summary>
<br>
 Essa é uma procedure em PL/SQL que tem como objetivo verificar se determinados itens estão instalados de fábrica em uma aeronave. Ela percorre as tabelas chassi e logica_fabrica e, para cada combinação de chassi e item, utiliza a função verificar_instalacao_fabrica para determinar se o item está instalado.
A lógica principal está na cláusula MERGE, que realiza operações de atualização e inserção na tabela chassi_item. Se houver uma correspondência entre o chassi e o item na tabela chassi_item, ela atualiza o status de instalação. Se não houver correspondência, insere um novo registro indicando se o item está ou não instalado de fábrica.
    
    ```SQL
    CREATE OR REPLACE PROCEDURE verificar_e_inserir_instalacao_fabrica AS
      v_chassi chassi.id_chassi%TYPE;
      v_item logica_fabrica.id_item%TYPE;
      v_instalado NUMBER;
    BEGIN
      FOR r_chassi IN (SELECT id_chassi FROM chassi) LOOP
        FOR r_item IN (SELECT id_item FROM logica_fabrica) LOOP
          v_instalado := verificar_instalacao_fabrica(r_chassi.id_chassi, r_item.id_item);
             MERGE INTO chassi_item ci
              USING (
                SELECT r_chassi.id_chassi AS id_chassi, r_item.id_item AS id_item, v_instalado AS instalado
                FROM dual
              ) temp
              ON (
        ci.id_chassi = temp.id_chassi AND ci.id_item = temp.id_item
      )
      WHEN MATCHED THEN
        UPDATE SET ci.instalado = temp.instalado
      WHEN NOT MATCHED THEN
        INSERT (id_chassi, id_item, instalado)
        VALUES (temp.id_chassi, temp.id_item, temp.instalado);
        END LOOP;
      END LOOP;
    END verificar_e_inserir_instalacao_fabrica;
    /
</details>

<details>
<br>
<summary><b>Triggers</b></summary>
Essa trigger foi criada para realizar auditoria na tabela CHASSI_BOLETIM após operações de atualização no campo STATUS. Quando uma atualização ocorre, a trigger gera um novo identificador de auditoria utilizando a sequência SEQ_CHASSI_BOLETIM_AUDIT e registra os dados relevantes na tabela de auditoria CHASSI_BOLETIM_AUDIT. Isso inclui o ID de auditoria, IDs de chassi e boletim, status anterior e novo, além do responsável pela modificação, armazenado na coluna MODIFICADO_POR. Essa abordagem proporciona um histórico detalhado das alterações de status na tabela principal, contribuindo para a transparência e rastreabilidade das modificações realizadas no sistema.


    ```SQL
    CREATE OR REPLACE TRIGGER TRG_AUDIT_CHASSI_BOLETIM
    AFTER UPDATE OF STATUS ON CHASSI_BOLETIM
    FOR EACH ROW
    DECLARE
    V_ID_AUDITORIA INTEGER;
    BEGIN
    -- Gerar um novo ID de auditoria
    SELECT SEQ_CHASSI_BOLETIM_AUDIT.NEXTVAL INTO V_ID_AUDITORIA FROM DUAL;

    -- Inserir os dados na tabela de auditoria
    INSERT INTO CHASSI_BOLETIM_AUDIT (ID_AUDITORIA, ID_CHASSI, ID_BOLETIM, STATUS_ANTERIOR, STATUS_NOVO, modificado_por)
    VALUES (V_ID_AUDITORIA, :OLD.ID_CHASSI, :OLD.ID_BOLETIM, :OLD.STATUS, :NEW.STATUS, :NEW.MODIFICADO_POR);
    END;
    /
    ```


</details>


<details>
<br>
<summary><b>Views</b></summary>

Essa view retorna um caminho hierarquico das lógicas, facilitando o tratamento para o backend, onde é possivel definir uma entrada (buscando a dependencia ou buscando pelo nivel) para recuperar a lógica de aplicação de um determinado item.

    ```SQL
    -- view que retorna o caminho hierarquico das logicas
    CREATE OR REPLACE VIEW v_hierarquia AS SELECT id_logica, logica_boletim.id_Item, ITEM.NOME, input1, operacao,  input2, dependencia,  LEVEL AS nivel, 
    CONNECT_BY_ROOT(ID_logica) AS no_raiz, SYS_CONNECT_BY_PATH(ID_logica, '/') AS caminho_hierarquia
    FROM Logica_Boletim
    JOIN item ON logica_boletim.id_item = item.id_item
    START WITH dependencia IS NULL
    CONNECT BY PRIOR ID_logica = dependencia;

    ```
</details>




## Aprendizados efetivos

Este projeto proporcionou a oportunidade de aprendizado sobre tópicos avançados em banco de dados. Durante o desenvolvimento, adquiri habilidades como a criação e execução de funções e procedimentos, o que me permitiu entender melhor a manipulação e gestão de dados.
Tive a oportunidade de trabalhar com auditoria usando triggers, o que me deu uma visão mais profunda sobre a segurança e integridade dos dados. Além disso, a visualização de dados com views me permitiu entender como apresentar dados de uma maneira mais eficiente e eficaz.
Aprofundei meus conhecimentos na linguagem PL/SQL da Oracle, o que me permitiu desenvolver soluções mais robustas e eficientes.


### Hard Skills

 <details>
  <summary><b>Funções e Procedures com PL/SQL: sei fazer com ajuda</b></summary>
     <br>
  <ul>
    <li>Estrutura e funcionamento de uma função</li>
    <li>Estrutura e funcionamento de uma procedure</li>
    <Li>Como executar funções e procedures</Li>
  </ul>
 </details>

  <details>
  <summary><b>Triggers: sei fazer com autonomia</b></summary>
     <br>
  <ul>
    <li>Estrutura e funcionamento de uma trigger</li>
    <li>Utilização e vantagens</li>
  </ul>
 </details>

   <details>
  <summary><b>Views: sei fazer com autonomia</b></summary>
     <br>
  <ul>
    <li>Estrutura e funcionamento de uma view</li>
    <li>Utilização e vantagens</li>
    <Li>Hierarquia de dados no oracle com connect_by</Li>
  </ul>
 </details>

### Soft Skills

<details>
  <summary><b>Proatividade</b></summary>
  <br>
  <ul>
    <li>Utilizando uma tecnologia nova, o Autonomous Database da Oracle, precisei ser proativo em aprender sobre a ferramenta e descobrir funcionalidades que ajudariam no controle da lógica do projeto. Essa soft skill me permitiu aprender muito e ver minha capacidade de tomar a frente de uma responsabilidade que era fundamental para o funcionamento do projeto.</li>
  </ul>
</details> 

<details>
  <summary><b>Trabalho em equipe</b></summary>
  <br>
  <ul>
    <li>Apresentei pra equipe meus conhecimentos adquiridos na ferramenta de banco de dados para facilitar o desenvolvimento do back-end.</li>
  </ul>
</details> 

<hr>
