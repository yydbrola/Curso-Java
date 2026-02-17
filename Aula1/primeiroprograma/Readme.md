O Camel Case (ou "caixa de camelo") é um padrão de nomenclatura muito usado na programação para juntar palavras sem usar espaços. O nome vem da semelhança visual com as corcovas de um camelo: as letras maiúsculas no meio da palavra se destacam como se fossem as corcovas.

A regra geral é simples: você remove os espaços entre as palavras e coloca a primeira letra de cada nova palavra em maiúscula.

Existem duas variações principais que você vai encontrar no dia a dia:
1. lowerCamelCase (ou apenas camelCase)

A primeira letra da primeira palavra é minúscula, e a primeira letra de todas as palavras seguintes é maiúscula.

    Onde é usado: Normalmente para nomear variáveis, atributos, funções e métodos na maioria das linguagens (como Java, JavaScript e TypeScript).

    Exemplos:

        nomeUsuario (em vez de nome usuario)

        calcularTotalCarrinho (em vez de calcular total carrinho)

        idadeMedia (em vez de idade media)

2. UpperCamelCase (também conhecido como PascalCase)

A primeira letra de todas as palavras (incluindo a primeira) é maiúscula.

    Onde é usado: É o padrão universal para nomear Classes, Interfaces e, no caso de frameworks front-end (como React/Next.js), para nomear Componentes.

    Exemplos:

        CarrinhoDeCompras (Classe)

        BotaoPrimario (Componente visual)

        SistemaDeLogin (Classe)

Como isso se aplica nas linguagens do seu dia a dia?

Como você trabalha com diferentes tecnologias, é importante notar que cada ecossistema tem suas preferências:

    No Front-end (JavaScript / TypeScript / Next.js): O camelCase domina. Você usará para quase tudo, exceto para os componentes do React, que exigem PascalCase para que o framework entenda que é um componente e não uma tag HTML padrão (ex: <BotaoPrimario /> em vez de <botaoPrimario />).

    Em Python (Para seus estudos de IA/LLMs):
    O Python é um pouco diferente. A comunidade Python prefere usar o snake_case (palavras separadas por underline, todas em minúsculo, como nome_usuario) para variáveis e funções. No entanto, o Python usa o PascalCase para nomear Classes (ex: class ModeloDeLinguagem:).

    No Java (Como no vídeo do Guanabara):
    O Java segue a regra estritamente: PascalCase para Classes/Interfaces e camelCase para métodos e variáveis.



    Para entender o System.out.print("hello World"), a melhor forma é "desmontar" esse comando pedaço por pedaço.

Como o próprio Guanabara explicou no vídeo, o Java foi criado para rodar em qualquer lugar (computadores, celulares antigos, geladeiras, relógios). Por isso, o comando parece um pouco longo: ele precisa ser muito específico sobre onde e como a mensagem vai aparecer.

Aqui está a anatomia exata desse comando:

    System (O Sistema):
    É uma Classe nativa do Java (note o "S" maiúsculo seguindo a regra do CamelCase/PascalCase). Ela representa o sistema ou o ambiente onde o seu programa está rodando no momento.

    .out (A Saída):
    É um atributo dentro da classe System. O out (saída, em inglês) representa o destino padrão de saída de dados do sistema. Em um computador convencional, esse destino padrão é a tela do terminal/console. Se fosse um relógio digital, a saída seria o pequeno visor de cristal líquido.

    .print() (A Ação):
    É o método (ou função) que executa a ação de fato. O print pega a informação que você colocou dentro dos parênteses e a "imprime" (exibe) na saída (out) do sistema (System).

    "hello World" (O Parâmetro/Argumento):
    É o dado que você está entregando para o método print trabalhar. Como é um texto, ele precisa estar sempre entre aspas duplas " " para que o Java entenda que é uma String (uma cadeia de caracteres), e não um comando ou variável.

    ; (Ponto e vírgula):
    No Java, o ponto e vírgula no final é obrigatório. Ele funciona como o ponto final de uma frase, dizendo ao computador: "Esta instrução acabou aqui, pode executar".

Um detalhe importante: print vs println

Na prática, você vai ver muito mais o uso do println (print line) do que apenas print.

    O print("hello") escreve a palavra e deixa o cursor do console exatamente ao lado da última letra. Se você der outro print("World") logo em seguida, o resultado sai grudado: helloWorld.

    O println("hello") escreve a palavra e automaticamente aperta a tecla "Enter" (quebra de linha) no final. O próximo comando será escrito na linha de baixo.