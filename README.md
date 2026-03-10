💱 Conversor de Moedas em Java

Aplicação desenvolvida em Java que permite converter valores entre diferentes moedas utilizando taxas de câmbio em tempo real através da API ExchangeRate-API.

O projeto foi estruturado utilizando boas práticas de organização de código, separação de responsabilidades e integração com API externa.

📌 Funcionalidades

✔ Conversão entre múltiplas moedas
✔ Consulta de taxas em tempo real via API
✔ Menu interativo no terminal
✔ Histórico das últimas conversões realizadas
✔ Sistema de cache para evitar chamadas repetidas à API
✔ Registro de logs com data e hora das conversões
✔ Tratamento de erros de conexão e entrada inválida

💻 Tecnologias utilizadas

Java 11+

HTTP Client (Java nativo)

Gson

ExchangeRate-API

Biblioteca java.time

Arquitetura MVC simplificada

📂 Estrutura do Projeto
ConversorMoedas
│
├── Principal.java
│
├── controller
│   └── ConversorController.java
│
├── service
│   └── ExchangeService.java
│
├── model
│   ├── ExchangeResponse.java
│   └── Conversao.java
│
├── util
│   ├── Cache.java
│   └── HistoricoConversoes.java
│
└── exception
    └── ApiException.java
    
⚙️ Como executar o projeto

1️⃣ Clonar o repositório
git clone https://github.com/seuusuario/conversor-de-moedas.git

2️⃣ Entrar na pasta do projeto
cd conversor-moedas-java

3️⃣ Inserir sua chave da API

Crie uma conta na:

ExchangeRate-API

Depois substitua no arquivo:

ExchangeService.java
private static final String API_KEY = "SUA_API_KEY";

4️⃣ Compilar o projeto

javac Principal.java

5️⃣ Executar o programa

java Principal
📊 Exemplo de uso
===== CONVERSOR DE MOEDAS =====

1 - Fazer conversão
2 - Ver histórico
3 - Sair

Escolha: 1

Moedas disponíveis:
1 - Real (BRL)
2 - Dólar (USD)
3 - Euro (EUR)
4 - Libra (GBP)
5 - Iene (JPY)
6 - Dólar Canadense (CAD)

Escolha moeda base: 1
Escolha moeda destino: 2

Valor: 100

Resultado: 19.85 USD
📜 Histórico de Conversões

O sistema registra automaticamente as conversões realizadas:

2026-03-10T14:30:15 | 100 BRL → 19.85 USD
2026-03-10T14:31:40 | 50 USD → 246.50 BRL
🧠 Conceitos aplicados

Este projeto utiliza conceitos importantes da programação Java:

Consumo de API REST

Manipulação de JSON

Uso de bibliotecas externas

Programação orientada a objetos

Separação de responsabilidades

Arquitetura MVC

Tratamento de exceções

Sistema de cache

Logs de execução

🚀 Melhorias futuras

Algumas melhorias planejadas para evolução do projeto:

Interface gráfica com JavaFX

Suporte a mais de 150 moedas

Salvamento do histórico em arquivo JSON

Implementação de testes automatizados

Dockerização da aplicação

Gráficos de variação cambial

👨‍💻 Autor

Desenvolvido por Jonathan Karllo

Projeto criado para fins de estudo e prática em Java, consumo de APIs e arquitetura de software.
