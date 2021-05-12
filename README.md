# todo-list-spring-boot

### Getting Started

git clone https://github.com/EdioPaul/todo-list-spring-boot

Execute com SpringToolSuite4
Abra http://localhost:8080/todolist

### Script SQL para criar a tabela

CREATE TABLE `todo`.`todo` (
 `id` INT NOT NULL,
 `todo` VARCHAR(255) NULL,
 `time` VARCHAR(25) NULL,
 `commit` VARCHAR(255) NULL,
 PRIMARY KEY (`id`));

 ALTER TABLE `todo`.`todo`
 CHANGE COLUMN `id` `id` INT(11) NOT NULL AUTO_INCREMENT ,
 ADD UNIQUE INDEX `id_UNIQUE` (`id` ASC);
 
 
### Spring DATASOURCE (DataSourceConfiguration & DataSourceProperties)

src/main/resources > application.properties

spring.datasource.url=jdbc:mysql://localhost:3306/todo?useSSL=false
spring.datasource.username=(login do seu BD)
spring.datasource.password=(senha do seu BD)

