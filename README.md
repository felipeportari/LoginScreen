# LoginScreen - Resumo

## Descrição
A classe `LoginScreen` permite autenticar usuários simulando um banco de dados de usuários. Ela oferece funcionalidades para autenticação e adição de novos usuários.

## Funcionalidades
- **Construtor (`LoginScreen()`):** Inicializa uma instância da classe e configura um banco de dados de exemplo com usuários predefinidos.

- **Método `login(String username, String password)`:** Tenta autenticar um usuário com base no nome de usuário e senha fornecidos. Retorna verdadeiro se a autenticação for bem-sucedida e falso caso contrário.

- **Método `addUser(String username, String password)`:** Adiciona um novo usuário ao banco de dados. Observação: Este método não é recomendado para uso em um ambiente de produção devido à falta de medidas de segurança.

## Uso
A classe `LoginScreen` é útil para demonstrações e testes de autenticação de usuários, mas não deve ser usada em ambientes de produção devido a questões de segurança.

### Exemplo de Uso
```java
LoginScreen loginScreen = new LoginScreen();

// Autenticar um usuário
boolean isAuthenticated = loginScreen.login("john", "password123");

// Adicionar um novo usuário (não recomendado para produção)
loginScreen.addUser("newuser", "newpassword");
