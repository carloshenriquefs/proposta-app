# :construction: - Projeto: Proposta-app

- Aplicação baseada em microsserviços;
- Os serviços irão conversar entre si de forma assíncrona utilizando RabbitMQ;


## :computer: - Tecnologias: 

- Java;
- Spring Boot;
- Spring Framework;
- RabbitMQ;
- Docker;
- Maven;
- JPA;


## :pencil2: - Subir imagem Docker & RabbitMQ: 

```json
docker run -d -p 5672:5672 -p 15672:15672 --name my-rabbit rabbitmq:3-management

docker run --name proposta-web-container -d --rm -p 80:80 matheuspieropan/proposta-web
```


## :card_index_dividers: - Microsserviços:

![microdrawio](https://github.com/carloshenriquefs/proposta-app/assets/54969405/cf0694b5-9769-4529-b372-aa00ff29095f)

## :white_check_mark: - Vantagens: 

- Melhor para se trabalhar quando se tem muitos profissionais atuando na aplicação;
- Se um apresentar algum problema/instabilidade os outros continuam funcionando normalmente;
- Maior facilidade em adotar escalabilidade horizontal;
- Mais fácil adotar novas tecnologias/seguir padrões de projeto -boas práticas;


## :x: - Desvantagens:  

- Maior tráfego de rede;
- Deploy se torna mais algo mais complexo uma vez que todos microsserviços precisam estar 'casando' entre as versões;
- Maior dificuldade em depuração;

  
## :screwdriver: - JPA:

![jpa drawio](https://github.com/carloshenriquefs/proposta-app/assets/54969405/5808b5ad-d64c-4a41-88e1-101dbd792af1)

