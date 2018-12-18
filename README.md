# DataBaseMySQL
Uma classe muito útil para operações com banco de dados MySQl.
Classe para comunicação com o banco de dados. As explicações dos métodos estão logo acima da declaração.

# IMPORTANTE 
* Antes de utilizar cada método, é necessário CONECTAR (método Conectar) com o banco. 
* Após utilizar o método, FECHE a conexão com o método Fechar - ao menos que necessite usar algum resultSet. Nesse caso, feche a conexão no final de todas as operações.

**Exemplo:**

      DataBase.conectar(); 
      String[] valores = {valor1, valor2, ..., valorN};
      DataBase.gravarDados(tabela, valores);
      DataBase.fechar();

# IMPORTANTE 2: 
* Todos os métodos são estáticos, ou seja, não é necessário criar um objeto DataBase

**Exemplo:**

    DataBase database = new DataBase(); ← ISSO NÃO É NECESSÁRIO
    Utilize os métodos usando DataBase.método();

# Url, usuário e senha
A classe DataBase possui os atributos _url_, _user_ e _password_. **Altere-os** para a url (preste atenção ao nome do banco de dados), o usuário e a senha do seu localhost, respectivamente.

