# JPA
Anotações sobre a especificação JPA e sua implementação com Hibernate

- Java Persistence API (JPA) é a especificação padrão da plataforma Java EE (pacote javax.persistence) para mapeamento objeto-relacional e persistência de dados.

![image](https://user-images.githubusercontent.com/78964459/189126509-902b1ad9-0389-4e29-9144-80e230743ff4.png)

## Pricipais classes

### EntityManager
- Um objeto EntityManager encapsula uma conexão com a base de dados e serve para efetuar operação de acesso a dados (inserção, remoção, deleção, atualização).
- **Escopo:** tipicamente mantem-se uma instância única de EntityManager para cada thread do sistema (no caso de aplicações web, para cada requisição do sistema). Ou seja, quando um usuário faz uma requisição a aplicação instancia um único EntityManager para trabalhar com todos os dados daquela requisição.

### EntityManagerFactory
- Um objeto EntityManagerFactory é utilizado para instanciar objetos EntityManager
- **Escopo:** tipicamente mantem-se uma instância única de EntityManagerFactory para toda aplicação

## Serializable
- Habilita que um objeto de uma determinada classe possa ter seu estado persistido pela API padrão do Java
