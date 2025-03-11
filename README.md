# 📌 ConsomeCEP2025

## 📖 Sobre o Projeto
Este projeto foi desenvolvido para **consultar endereços a partir de um CEP** utilizando a API pública **ViaCEP**. Além disso, os dados são armazenados em um banco de dados local para otimizar consultas futuras.

## 🚀 Tecnologias Utilizadas
- **Java (Jakarta EE)**
- **Maven**
- **JPA (Jakarta Persistence API)**
- **Banco de Dados H2 ou MySQL**
- **API ViaCEP**

## 🔄 Fluxo do Programa
1. O sistema solicita um **CEP** ao usuário.
2. Verifica no **banco de dados** se o CEP já foi consultado.
3. Se o CEP **existe no banco**, exibe as informações armazenadas.
4. Se o CEP **não existe**, busca os dados na **API ViaCEP**.
5. Os dados do endereço e a **data/hora da consulta** são salvos no banco.
6. O sistema informa ao usuário que a busca foi feita via API e que os dados foram armazenados.

## ⚙️ Como Executar o Projeto

### 🔹 Pré-requisitos
Antes de começar, você precisa ter instalado:
- [Java 17+](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Maven](https://maven.apache.org/download.cgi)
- Um banco de dados (H2, MySQL, etc.)

### 🔹 Passo a Passo
1. **Clone o repositório**:
   ```sh
   git clone https://github.com/seu-usuario/consomeCep2025.git
   cd consomeCep2025
   ```
2. **Compile o projeto com Maven**:
   ```sh
   mvn clean install
   ```
3. **Execute o programa**:
   ```sh
   mvn exec:java -Dexec.mainClass="br.unipar.programacaoweb.ConsomeCEP"
   ```
4. **Digite um CEP** e veja as informações retornadas.

## 📌 Melhorias Futuras
- Criar uma interface gráfica para interação com o usuário.
- Melhorar o tratamento de erros para CEPs inválidos.
- Implementar uma API interna para consultas via REST.

---  
Este `README.md` agora está alinhado com o seu código! 😊🚀 Se precisar de mais alguma coisa, me avise!

