Esse repositório contém o layout para Teclados Internacionais com a aspa mais fácil de utilizar :)

## Contextualização

Digitar aspas em um teclado internacional é um saco. Sim, um saco. Usando o layout "Estados Unidos (internacional)", temos um mesmo botão tanto para aspas quanto para acentos. Se eu quero digitar aspas, eu preciso apertar no botão [ ' ] do teclado duas vezes, e aí o que acontece? '' - o Windows nos devolve duas aspas simples.

Por si só já é chato que isso aconteça, mas fica ainda pior quando digitamos isso dentro de uma IDE, e aí sempre temos que apertar duas vezes na tecla [ ' ], e, em seguida, mover o cursor para dentro delas para que possamos digitar o que queremos.

Desde que comecei no meu emprego atual, estou com uma máquina com Ubuntu, e no Ubuntu há um layout chamado "Inglês (EUA, intern. alt.)". É praticamente igual ao "Estados Unidos (internacional)" do Windows, mas com uma diferença: a maneira como ele lida com a tecla do acento/aspa.

Nesse layout do Ubuntu, quando eu aperto duas vezes na [ ' ], ele devolve ´, que é o acento agudo. Quando é que utilizamos um acento agudo sozinho? Praticamente nunca. Quando aperto a [ ' ] e qualquer outra letra que possa ser acentuada, ele acentua normalmente. E como é que eu faço a aspa no Ubuntu então? Simples: [ AltGr ] + [ ' ]. Dessa maneira, o Ubuntu devolve UMA aspa simples. E é aí que vem a mágica das IDEs: quando digitamos uma aspa simples, ela autocompleta com a segunda e deixa nosso cursor dentro das aspas, onde normalmente queremos digitar.

Na prática, o que seriam três pressionamentos de tecla sequenciais ( [ ' ] [ ' ] [ <- ] ) podem se transformar em dois pressionamentos simultâneos ( [AltGr] + [ ' ] ) para um mesmo resultado.

Agora você pode estar pensando: beleza. Mas isso é no Ubuntu? Como faço isso no Windows?

A própria Microsoft disponibiliza uma ferramenta chamada Microsoft Keyboard Layout Creator (MSKLC) onde você pode criar seus próprios layouts do zero ou até mesmo a partir de layouts existentes, e foi isso que eu fiz!

Baixei o programa, importei o layout "Estados Unidos (internacional)" e basicamente inverti o funcionamento da tecla [ ' ]. Toda a acentuação continua funcionando como antes, porém, a partir disso, as aspas simples funcionam pelo [ AltGr ] + [ ' ] e as aspas duplas pelo [ Shift ] + [ AltGr ] + [ ' ].

A boa notícia é que você não precisa editar o layout manualmente, pois ele já está prontinho aqui!

## Como instalar?

a) Você pode baixar o pacote compactado dead-apostrophe.rar na [release](https://github.com/pedr0diniz/layout-aspa-facil/releases/tag/v1.0), descompactar e simplesmente rodar o setup.exe

ou

b) Caso prefira, você pode buildar o layout diretamente do arquivo .klc. Dessa forma, você gera a mesma estrutura de pastas que estão no .rar, incluindo o setup.exe, por onde deve ser feita a instalação. Para isso:
  1. Abra o Microsoft Keyboard Layout Creator
  2. File > Load Source File
  3. Project > Build DLL and Setup Package
