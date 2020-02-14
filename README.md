# javalin-kotlin-example

## source code 

# Adicionando Independencias.

<dependencies>
        <dependency>
            <groupId>io.javalin</groupId>
            <artifactId>javalin</artifactId>
            <version>3.7.0</version>
        </dependency>
  
 # Manipuladores
O Javalin possui três tipos principais de manipuladores: manipuladores anteriores, manipuladores de terminais e manipuladores posteriores. (Também existem manipuladores de exceções e manipuladores de erros, mas os abordaremos posteriormente). Os manipuladores antes, terminal e pós-processamento requerem três partes:

Um verbo, um dos seguintes: before, get, post, put, patch, delete, after (... head, options, trace, connect)
Um caminho, ex: /, /hello-world,/hello/:name
Uma implementação de manipulador ctx -> { ... }
A Handlerinterface possui um tipo de retorno nulo. Você usa ctx.result()para definir a resposta que será retornada ao usuário.

