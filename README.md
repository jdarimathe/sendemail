# sendemail
1- Add the email dependency 
  - <dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-mail</artifactId>
    </dependency>
2- Add this configuration in the application.properties file
  - spring.mail.host=smtp.gmail.com 
    spring.mail.port=587
    spring.mail.username=
    spring.mail.password= (This password is not the gmail password. You should generate a new one)
    spring.mail.properties.mail.smtp.auth=true
    spring.mail.properties.mail.smtp.starttls.enable=true
    
3- Autowired JavaMailSender in the service layer
   - The JavaMailSender have many methods like 
     message.setFrom("example@gmail.com");
     message.setTo("example@gmail.com");
     message.setCc("example@gmail.com");
     message.setSubject("Test Subject My Spring Boot App");
     message.setText("Test Body My Spring Boot App, Just trying to send a mail from my spring boot app");
    
