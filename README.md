# Back-end using Spring Boot framework

<h2>Executar usando docker</h2>
Se for a primeira vez, execute

$docker-compose up

Execute o seguinte comando se quiser atualizar o aplicativo

$docker-compose up --build --no-deps user-crud-application-container


Para limpar o cache do docker: $docker system prune -a



<h2>Configuração no local</h2>
- Baixe o projeto ou use $git clone git@github.com:joel021/crud_user_jwt.git
- Vá para <i>src/main/resources/</i>
- Criar <i>application.properties</i> arquivo usando <i> application.properties.example</i> como exemplo
- Altere os valores dos parâmetros aplicáveis ​​no arquivo, conforme <i>spring.datasource.username</i> e <i>spring.datasource.password</i>
- Se preferir, é possível criar uma variável de ambiente e utilizá-la em <i>application.properties</i> arquivo. Por exemplo, crie DB_PASSWORD e atribuir <i>spring.datasource.password</i> como ${DB_PASSWORD}.
- Instale o java 17 ou superior em sua máquina
- no nível raiz do projeto, execute:
    - $ mvn clean spring-boot:run, to run the project
    - $ mvn clean install, to install the project in your envromment

<h3>Para executar usando Java 8</h3>

<p>Este projeto foi desenvolvido usando Java 17 com spring boot 3. No entanto, ele pode ser construído usando Java 8.</p>

- Instale o Java 8 em sua máquina
- Acesse https://start.spring.io/ e crie um novo projeto escolhendo Java 8, Maven e Spring Boot 2.7.
- Copie os arquivos de classes deste projeto para o novo projeto
- Lidar com as dependências
