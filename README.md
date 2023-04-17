# 🔴 Padrões de Projetos com Java - DIO

Neste projeto, o objetivo é demonstrar a utilização de Padrões de Projetos em Java, como Singleton, Facade e Strategy, para implementar um sistema de gerenciamento de clientes.

## 🛠️ Funcionamento do Programa 

O programa utiliza o banco de dados relacional H2 para armazenar os dados dos clientes cadastrados. Com isso, é possível realizar operações de cadastro, edição, exclusão e consulta de clientes de maneira persistente e disponível para uso posterior. Além disso, o sistema também utiliza a API ViaCEP para buscar informações de endereço a partir do CEP informado pelo usuário

## ⚙️ Padrões de projeto explorados

- **Singleton**: utilização do padrão Singleton para garantir que apenas uma instância da classe responsável pelo acesso ao banco de dados seja criada, evitando problemas de concorrência e garantindo a consistência dos dados. 
- **Facade**: utilização do padrão Facade para fornecer uma interface simples e unificada para o gerenciamento dos clientes, isolando a complexidade do sistema e facilitando o seu uso. 
- **Strategy**: utilização do padrão Strategy para permitir a busca de endereço a partir de diferentes provedores de serviços, como a API ViaCep, possibilitando a fácil extensão do sistema para suportar outros provedores.

## 🌐 Consumo da API ViaCep 

O projeto consome a API ViaCep para obtenção dos dados de endereço do cliente. Para isso, é utilizada a biblioteca "Retrofit", que facilita o consumo de APIs REST em Java. Os dados de endereço são obtidos a partir do CEP informado pelo usuário e são armazenados no objeto "Endereço".