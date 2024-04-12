# APP-DanceSP
## Descrição detalhada do APP e funções das telas e os recursos que serão aplicados 
## Quais são as telas estaticas e as dinamicas

# Tela Inicial
![alt text](image-1.png)

Essa tela de apresentação irá mostrar uma foto de fundo, o nome, a logo do app e o copyright.

### Widgets - Inicial
**1 - Image:** É a implementação de uma imagem

**Parametro** 

    const Image(
      image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
    )

--------------------------------------------------------------------------------------------------

**2 - Text:** Implementação de Texto

**Parametro** 

    RichText(
        const TextSpan(text: 'texto'),)


# Tela Home
![alt text](image-2.png)

Essa tela irá apresentar 3 escolhas para o usuário decidir qual modalidade, mostrando uma imagem representativa da modalidade e o nome, sendo as modalidades Hip Hop, Ballet e Jazz.
Logo abaixo da opções terá um rodapé com botões que irão indicar a navegação do usuário durante toda a aplicação.

### Widgets - Home
**1 - TextButton:** Ultilizado como botão com um texto.

**Parametro** 

    TextButton(
        style: TextButton.styleFrom(
          primary: Colors.blue,
          ),
          onPressed: () { },
          child: Text('TextButton'),
    )

--------------------------------------------------------------------------------------------------

**2 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**3 - IconButton:** Ultilizado como botão com imagem.

**Parametro** 
 
    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
    ),

        
# Tela modalidade Hip-Hop/Ballet/Jazz
![alt text](image-3.png)

Essas telas serão exatamentes indenticas na sua funcionalidade, como um botão em formato de estrela que irá adicionar aos favoritos, imagem e o nome de cada grupo e um botão que irá direcionar as informações do grupo. 

### Widgets - Modalidades
**1 - Container:** Ultilizado para pintar uma parte especifica na tela.

**Parametro** 

    Container(
      color: Colors.black,
        child: Text('Container'),
    );

--------------------------------------------------------------------------------------------------

**2 - Image:** É a implementação de uma imagem.

**Parametro** 

    const Image(
      image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
      )

--------------------------------------------------------------------------------------------------

**3 - IconButton:** Ultilizado como botão com imagem.

**Parametro -** 

    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),

--------------------------------------------------------------------------------------------------

**4 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

# Tela do grupo de dança
![image](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/c47b744e-b738-49e5-9ab1-972029f2b15b)

Essa tela irá apresentar uma foto do grupo junto,o nome e um botão de favoritos, logo abaixo o nome do lider/gerente, história e turmas disponiveis do grupo. Também será implementado um mapa para a vizualização do endereço para o usuário, um botão de matricular que direcionará para o site de inscrição do grupo, comentários e avaliações do google sobre o local.

### Widgets - Telas do grupo.
**1 - Container:** Ultilizado para pintar uma parte especifica na tela.

**Parametro** 

    Container(
        color: Colors.black,
        child: Text('Container'),
    );

--------------------------------------------------------------------------------------------------

**2 - Image:** É a implementação de uma imagem.

**Parametro** 

    const Image(
      image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
    )

--------------------------------------------------------------------------------------------------

**3 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**4 - TextButton:** Ultilizado como botão com um texto.

**Parametro** 

    TextButton(
        style: TextButton.styleFrom(
          primary: Colors.blue,
          ),
          onPressed: () { },
          child: Text('TextButton'),
    )

--------------------------------------------------------------------------------------------------

**5 - IconButton:** Ultilizado como botão com imagem.

**Parametro -** 

    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),
          
--------------------------------------------------------------------------------------------------

**6 - FlutterMap:** Ultilizado para mapa do google.

**Parametro -** 

        Widget build(BuildContext context) {
          return FlutterMap(
            options: MapOptions(
              initialCenter: LatLng(51.509364, -0.128928),
                 initialZoom: 9.2,
        ),
        children: [
          TileLayer(
            urlTemplate: 'https://tile.openstreetmap.org/{z}/{x}/{y}.png',
            userAgentPackageName: 'com.example.app',
          ),
          RichAttributionWidget(
            attributions: [
              TextSourceAttribution(
                'OpenStreetMap contributors',
                onTap: () => launchUrl(Uri.parse('https://openstreetmap.org/copyright')),
              ),
            ],
          ),
        ],
      );
    }
    
--------------------------------------------------------------------------------------------------

*7 - Scrollbar:** Ultilizado para rolagem de tela.
**Parametro -** 

        Scrollbar(
         child: listView.builder(
             itemCount: 20,
             itemBuilder:(c, i) => MyItem(i).
            ),
        )
        
# Tela QuemSomos
![alt text](image-6.png)

Essa tela será apresentado as criadoras do aplicativo com seus nomes e fotos, o objetivo e informações sobre a aplicação.

### Widgets - Quem Somos
**1 - Container:** Ultilizado para pintar uma parte especifica na tela.

**Parametro** 

    Container(
        color: Colors.black,
        child: Text('Container'),
    );

--------------------------------------------------------------------------------------------------

**2 - Image:** É a implementação de uma imagem.

**Parametro** 

    const Image(
      image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
    )

--------------------------------------------------------------------------------------------------

**3 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**4 - IconButton:** Ultilizado como botão com imagem.

**Parametro -** 

    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),

# Tela Favoritos
![alt text](image-7.png)

Essa tela mostrará e salvará os grupos escolhidos como favoritos pelo usuário, assim estabelecendo um histórico de favoritos do usuário.

### Widgets - Favoritos
**1 - IconButton:** Ultilizado como botão com imagem.

**Parametro -** 

    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),

  --------------------------------------------------------------------------------------------------

**2 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**3 - Image:** É a implementação de uma imagem.

**Parametro** 

    const Image(
      image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
    )

--------------------------------------------------------------------------------------------------

**4 - Container:** Ultilizado para pintar uma parte especifica na tela.

**Parametro** 

    Container(
        color: Colors.black,
        child: Text('Container'),
    );

# Tela de Cadastro/Login

Ambas telas terão o mesmo layout onde irá cadastrar o email e senha do usuário, um botão para prosseguir com o login ou cadastro do usuário.

![alt text](image-8.png)
### Widgets - Login/Cadastro

**1 - Container:** Ultilizado para pintar uma parte especifica na tela.

**Parametro** 

    Container(
        color: Colors.black,
        child: Text('Container'),
    );

 --------------------------------------------------------------------------------------------------

**2 - TextField:** Caixa de texto.

**Parametro** 

    TextField(
      decoration: InputDecoration(
          border: OutlineInputBorder(),
        hintText: 'Enter a search term',
    ),
),

 --------------------------------------------------------------------------------------------------

**3 - IconButton:** Ultilizado como botão com imagem.

**Parametro -** 

    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),

  --------------------------------------------------------------------------------------------------

**4 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**5 - TextButton:** Ultilizado como botão com um texto.

**Parametro** 

    TextButton(
        style: TextButton.styleFrom(
          primary: Colors.blue,
          ),
          onPressed: () { },
          child: Text('TextButton'),
    )

# Tela de Perfil
![alt text](image-9.png)

Essa tela será onde as informações de login serão mostradas ao usuário, como o nome, email, foto de perfil e foto de fundo. Será implementado um botão para os favoritos do usuário.

### Widgets - Perfil

**1 - TextButton:** Ultilizado como botão com um texto.

**Parametro** 

    TextButton(
        style: TextButton.styleFrom(
          primary: Colors.blue,
          ),
          onPressed: () { },
          child: Text('TextButton'),
    )

  --------------------------------------------------------------------------------------------------

**2 - Text:** Implementação de Texto.

**Parametro** 

    RichText(
      const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**3 - IconButton:** Ultilizado como botão com imagem.

**Parametro -** 

    IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),
          
--------------------------------------------------------------------------------------------------

**4 - Container:** Ultilizado para pintar uma parte especifica na tela.

**Parametro** 

    Container(
        color: Colors.black,
        child: Text('Container'),
    );

--------------------------------------------------------------------------------------------------

**5 - Image:** É a implementação de uma imagem.

**Parametro** 

    const Image(
      image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
      )
