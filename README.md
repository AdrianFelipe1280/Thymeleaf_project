# 🍃 Projeto com Spring Boot e Thymeleaf

![Status](https://img.shields.io/badge/status-em--desenvolvimento-yellow)

## 📖 Sobre

Este é um projeto web desenvolvido como parte dos meus estudos em Java com o framework Spring Boot. A aplicação utiliza o **Thymeleaf** como template engine para renderizar as páginas web do lado do servidor, permitindo a criação de interfaces dinâmicas.

---

## ✨ Objetivo

Este módulo implementa um sistema completo de autenticação e autorização de usuários. Utilizando o Spring Security,
o fluxo gerencia o ciclo de vida do usuário (cadastro, login, logout) com proteção de senhas via hashing e validação de dados.
O controle de acesso é granular, baseado em perfis de usuário (roles), restringindo o acesso a endpoints e visualizações específicas.
As informações de usuários e sessões são persistidas em uma instância do MongoDB Atlas, enquanto a interface é renderizada com Thymeleaf,
mantendo a camada de apresentação independente da lógica de negócio para facilitar a manutenção e customização de temas.

---

## 🚀 Como Executar o Projeto

Para executar este projeto em sua máquina local, siga os passos abaixo.

### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
- [Git](https://git-scm.com)
- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/downloads/)
- [Maven](https://maven.apache.org/)
- [Intellij](https://www.jetbrains.com/idea/download/?section=windows)
- [MongoDB Atlas](https://www.mongodb.com/products/platform/atlas-database)

### Rodando a Aplicação

1. **Clone o repositório no Intellij:**
   ```bash
   git clone [https://github.com/AdrianFelipe1280/Thymeleaf_project.git](https://github.com/AdrianFelipe1280/Thymeleaf_project.git)

2. **Acesse [MongoDB Atlas](https://www.mongodb.com/products/platform/atlas-database) e realize os passos para criação de sua conta e posteriormente seu banco**
   
3. **Após criar, clique em connect**
<img width="1089" height="224" alt="Captura de tela 2025-09-25 011517" src="https://github.com/user-attachments/assets/d287e322-2e8c-41d1-b5bb-ab1de9f63fd9" />

4. **"clique em View full code sample" e copie o link que aparecer no código exibido em String connectionString = "seu codigo"**
<img width="720" height="544" alt="image" src="https://github.com/user-attachments/assets/81cc0578-1186-4825-ad24-6a6211e5b0b0" />

5. **"Não esqueça de modificar <db_password>" para a senha que você colocou em seu banco**
<img width="443" height="37" alt="image" src="https://github.com/user-attachments/assets/aa1f7e0a-6ade-4143-8a9b-56f394e8e5a8" />

6. **Vá em "application.properties", localizada em resources e copie a URL modificada em "spring.data.mongodb.uri=" e seu Cluster em spring.data.mongodb.database=**
<img width="456" height="53" alt="image" src="https://github.com/user-attachments/assets/f3cb7c08-917a-4c7f-a9d9-d01d8e18a45d" />

7. **Realize o download de todas as pendências e execute o arquivo ThindeskApplication.java**
<img width="1086" height="335" alt="Captura de tela 2025-09-25 010427" src="https://github.com/user-attachments/assets/f3635181-4c34-49d2-8c9d-9cacf4cd64cc" />

8. **Acesse http://localhost:8080/login para ver a aplicação**
<img width="1152" height="657" alt="image" src="https://github.com/user-attachments/assets/7056d075-1644-4bf6-9cc3-cbf5d831b58b" />

9. **Clique em Criar funcionário padrão para criar automaticamente um usuário funcionário**
<img width="424" height="115" alt="image" src="https://github.com/user-attachments/assets/15eece37-4cec-4057-87ab-55334c8adcdf" />

10. **As credencais do usuário funcionário estão localizadas em "application.properties"**
<img width="348" height="52" alt="image" src="https://github.com/user-attachments/assets/c94534d0-bde0-4d2a-b190-c4eca63677d6" />

11. **As credencais do usuário funcionário podem ser alteradas a gosto modificando "UsuarioService"**
<img width="499" height="133" alt="image" src="https://github.com/user-attachments/assets/4b92e0a5-20db-47f3-a561-b9640ba43bc5" />

12. **Para criar uma conta, clique em "Não tem uma Conta?" onde você será redirecionado para esta tela**
<img width="508" height="610" alt="image" src="https://github.com/user-attachments/assets/3f2486d9-f8c0-49d1-bc01-532cc37a3b8a" />

13. **Após realizar seu cadastro, você poderá realizar o login na página principal. Não há nenhuma funcionalidade no momento**
<img width="1900" height="896" alt="image" src="https://github.com/user-attachments/assets/1cdf4ef1-82db-4bcb-86cd-d69e4205d6a8" />

14. **Você pode verificar como são armazenados os dados no site do MongoDB em collections com a senha criptografada utilizando Bcrypt**
<img width="601" height="178" alt="image" src="https://github.com/user-attachments/assets/61e350bb-e0d4-4e7f-881b-78dd3ea6e523" />

15. **Você pode verificar onde está o token da sessão na aba de cookies, localizado em "inspecionar" do seu navegador**
<img width="791" height="271" alt="image" src="https://github.com/user-attachments/assets/977c40f4-9afa-41d1-b740-14b8924cb9a4" />
