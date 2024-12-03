# LibraryApi

### Sumário:
  * [Descrição](#descrição)
  * [Como baixar o repositório](#como-baixar-o-repositório)
  * [Pré-requisitos](#pré-requisitos)
  * [Contribuindo](#contribuindo)
  * [Autores](#autores)
  * [Licença](#licença)

## Descrição
Este é um sistema de gerenciamento de biblioteca, projetado para facilitar o controle de livros, usuários e empréstimos. A aplicação foi construída com **Spring Boot**, utiliza **MySQL** como banco de dados e está totalmente conteinerizada com **Docker**, permitindo fácil implantação em qualquer ambiente que suporte containers.

### Funcionalidades principais
- Cadastro de livros, usuários e empréstimos.
- Gerenciamento e histórico de devoluções.
- Validação e tratamento de erros HTTP.
- Conteinerização completa com suporte a ambientes multi-plataforma.


## **Como baixar o repositório**  
1. Clone este repositório:  
   ```bash
   git clone https://github.com/Tomaz-Arlindo/LibraryApi.git
   ``` 
2. Navegue até o diretório onde se encontra o *docker-compose.yml*
   ```bash
   cd LibraryApi/libraryapi
   ``` 
   

## **Pré-requisitos**  

Você precisará instalar os seguintes programas para rodar o projeto:  
- **Docker** e **Docker Compose**  
- **Java 21+**  

### **Instalação no Linux (Fedora)**
<details>
 
1. Instale o Docker e o Compose:  
   ```bash
   sudo dnf install -y docker-ce docker-compose-plugin
   ```  

2. Inicie o Docker:  
   ```bash
   sudo systemctl start docker
   ```  

3. Verifique a versão do Java:  
   ```bash
   java --version
   ```  
   (Se necessário, instale o Java com `sudo dnf install java-21-openjdk`)

</details>

### **Instalação no Windows**
<details>
 
1. Baixe e instale o **Docker Desktop** :  
   - Acesse [Docker Desktop](https://www.docker.com/products/docker-desktop/) e faça o download.  

2. Certifique-se de ativar a opção para usar o WSL2 durante a instalação.  

3. Instale o **Java 21**:  
   - Baixe o instalador do OpenJDK 21 no site oficial: [OpenJDK Downloads](https://jdk.java.net/21/)
   - Após a instalação, verifique a versão no terminal ou PowerShell:  
     ```bash
     java --version
     ```
</details>

## **Como rodar o projeto**  

1. No diretório "libraryapi" do projeto, configure os containers com:  
   ```bash
   docker compose up --build -d
   ``` 

2. A aplicação estará disponível em:
   `http://localhost:8080`
   
3. Utilize um programa de requisições de sua preferência ([Postman](https://www.postman.com), [Insomnia](https://insomnia.rest/download), etc)

## Contribuindo
[Sabia como contribuir](https://github.com/Tomaz-Arlindo/LibraryApi/blob/master/CONTRIBUTING.md)

## Autores
<table align="center">
  <tr>
    <td align="center"><a href="https://github.com/CimentoPE"><img src="https://avatars.githubusercontent.com/u/150206630?v=4" width="150px" alt="Rafael"/><br /><sub><b>Rafael</b></sub></a></td>
    <td align="center"><a href="https://github.com/Tomaz-Arlindo"><img src="https://avatars.githubusercontent.com/u/109036088?v=4" width="150px" alt="Tomaz Arlindo"/><br /><sub><b>Tomaz Arlindo</b></sub></a></td>
    <td align="center"><a href="https://github.com/raiiguilherme"><img src="https://avatars.githubusercontent.com/raiiguilherme?v=4" width="150px" alt="Rai Guilherme"/><br /><sub><b>Rai Guilherme</b></sub></a></td>
    <td align="center"><a href="https://github.com/paulodbv"><img src="https://avatars.githubusercontent.com/u/142844427?v=4" width="150px" alt="Paulo Mateus"/><br /><sub><b>Paulo Mateus</b></sub></a></td>
    <td align="center"><a href="https://github.com/LucasAires01"><img src="https://avatars.githubusercontent.com/u/142992717?v=4" width="150px" alt="Lucas Aires"/><br /><sub><b>Lucas Aires</b></sub></a></td>
  </tr>
</table>

---
## Licença
**GNU General Public License v3.0**

Este projeto está licenciado sob a GNU GPL-3.0. Abaixo, um resumo dos principais pontos:

**Liberdade de uso:** Você pode usar o software para qualquer finalidade.

**Distribuição:** É permitido distribuir cópias, desde que a licença seja mantida.

**Modificações:** Alterações no código são permitidas, mas as versões modificadas devem ser licenciadas sob os mesmos termos.

**Software Livre:** O código-fonte deve estar disponível em todas as distribuições do software.

**Garantias:** Não há garantias para o software.

Para mais detalhes, consulte o texto completo da licença [aqui](https://github.com/Tomaz-Arlindo/LibraryApi/blob/master/LICENSE).
