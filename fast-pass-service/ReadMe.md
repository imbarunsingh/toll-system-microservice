A backened downstrean microservice that details on customer details.

#NOTE : Prefer to use bootstrap.yml for spring cloud project
bootstrap.yml is loaded before application.yml.

It is typically used for the following:

when using Spring Cloud Config Server, you should specify spring.application.name and spring.cloud.config.server.git.uri inside bootstrap.yml
some encryption/decryption information
Technically, bootstrap.yml is loaded by a parent Spring ApplicationContext. That parent ApplicationContext is loaded before the one that uses application.yml.