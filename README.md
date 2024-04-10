# APP-DanceSP
## descrição detalhada do APP e funções das telas e os recursos que serão aplicados 
## Quais são as telas estaticas e as dinamicas

## Tela Inicial
![1](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/1a2c2359-a81e-487b-9b1c-038bdb99a73d.png)
### Widgets - Tela Inicial
**1 - Image:** Será ultilizado para implementar a logo na tela incial.

**Parametro -** 
  const Image(
  image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
)

--------------------------------------------------------------------------------------------------

**2 - Text:** Será ultilizado para implementar o nome da logo e o copyright na tela incial.

**Parametro -** 
RichText(
const TextSpan(text: 'texto'),)


## Tela Home
![3](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/7823267a-51c6-408b-a30b-b74e80985f68)
### Widgets
**1 - Container:** Será ultilizado para pintar uma parte especifica na tela Home.

**Parametro -** 
Container(
    color: Colors.red,
  child: Text('Container'),
);

--------------------------------------------------------------------------------------------------

**2 - TextButton:** Será ultilizado como botão com um texto na tela de Home para direcionar para outra tela de modalidade.

**Parametro -** 
TextButton(
  style: TextButton.styleFrom(
    primary: Colors.blue,
  ),
  onPressed: () { },
  child: Text('TextButton'),
)

--------------------------------------------------------------------------------------------------

**3 - Text:** Será ultilizado para implementar o nome no rodapé de cada icone e nas frases na tela Home.

**Parametro -** 
RichText(
const TextSpan(text: 'texto'),)

--------------------------------------------------------------------------------------------------

**2 - IconButton:** Será ultilizado como botão com imagem na tela de Home para direcionar para outra tela de modalidade.

**Parametro -** 
 IconButton(
          splashRadius: 100,
          iconSize: 200,
          icon: Ink.image(
            image: const NetworkImage(
                'https://picsum.photos/250?image=9'),
          ),
          
## Tela modalidade Hip-Hop
![4](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/ee8ca5a2-3576-4af5-9136-1df753bad070)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)

## Tela modalidade Ballet
![5](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/f61923f2-2190-4a42-b93f-a090dc39e27a)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)

## Tela modalidade Jazz
![6](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/99cc8bed-7be2-4b15-9eaf-3182abcfdfb7)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)

## Tela1 do grupo de dança
![7](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/7f0062f6-25f8-44e4-a226-a2d3cefbf07b)
## Tela2 do grupo de dança
![8](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/88f68cdb-e822-4e10-a408-bf46d0597ee7)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)

## Tela QuemSomos
![2](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/7992a4fe-65cc-46ed-93da-aa1e2ea70ab1)
### Widgets
**1 - Container:** Será ultilizado para pintar uma parte especifica na tela Home.

**Parametro -** 
Container(
    color: Colors.red,
  child: Text('Container'),
);

--------------------------------------------------------------------------------------------------

**2 - Image:** Será ultilizado para implementar as Imagens na tela QuemSomos.

**Parametro -** 
  const Image(
  image: NetworkImage('https://flutter.github.io/assets-for-api-docs/assets/widgets/owl.jpg'),
)

--------------------------------------------------------------------------------------------------

**3 - Text:** Será ultilizado para implementar os textos na tela QuemSomos.

**Parametro -** 
RichText(
const TextSpan(text: 'texto'),)

## Tela Favoritos
![12](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/f83aa6b3-7ce2-47ec-b83e-4ae47c54b0c1)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)

## Tela de Login
![9](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/b9a1762b-945c-48e3-8c19-2ba5a1e2c857)
## Tela de Cadastro
![10](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/bfaf4e1f-48b3-430d-b3ee-6a83306ac632)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)

## Tela de Perfil
![11](https://github.com/IsabelaCSS/APP-DanceSP/assets/128037357/fca189ac-7ec1-445d-913f-146c713bea6e)
### Widgets ultilizados e explicação a implementação de cada um deles (principais parametros)
