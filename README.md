# Deadline #1
### Protótipo gráfico

Imagens do protótipo na pasta [prototipo](assets/prototipo).

Splash | Login | Registro
:-:|:-:|:-:
![](/assets/prototipo/app1.jpeg) | ![](/assets/prototipo/app2.jpeg) | ![](/assets/prototipo/register.jpeg) 

Feed | Buscar Categoria | Buscar Título | Meu Perfil
:-:|:-:|:-:|:-:
![](/assets/prototipo/app3.jpeg) | ![](/assets/prototipo/app4.jpeg) | ![](/assets/prototipo/app5.jpeg) | ![](/assets/prototipo/app6.jpeg) 

### Crud de entidades
* Movie
* Category
* Post
* Comment
* User

As entidades listadas acima serão armazenadas na aplicação para uma melhor experiência do usuário e serão atualizadas sempre que necessário.

### Internacionalização
A internacionalização consiste de dois arquivos de resources _strings.xml_ um arquivo padrão (default) com os valores das strings em inglês e outro arquivo destinado a dispositivos configurados com a lingua portuguesa com os valores traduzidos para o português. Caso o dispositivo utilize uma linguagem diferente do PT-BR o app usará o arquivo padrão. Os arquivos estão separados nas pastas _values_ e _values-pt_, ambos dentro da pasta [res](app/src/main/res).

### Integração com serviço externo
O aplicativo utilizará a API de filmes [The Movie Database](https://www.themoviedb.org/documentation/api) onde consultará todas as  informações relacionadas aos filmes e categorias. Além dessa API o app irá se comunicar com uma api desenvolvida específicamente para ele onde será registrado os comentários, posts e informações dos usuários.

### Recursos da plataforma
* Login Facebook
* Reprodutor de mídia nativo

O app irá utilizar o reprodutor de vídeos nativo do Android para exibir trailers dos filmes e também irá utilizar a [sdk do Facebook](https://developers.facebook.com/docs/android/) para realizar login.

# Deadline #2
## Diagrama Arquitetura de Projeto

![](/assets/diagrama_arquitetura/d_arquitetura.png)

## Estrutura de Projeto

![](/assets/estrutura_projeto/e_projeto.png)

### Pacotes

1. *data*: Contêm todas as classes que manipulam os dados armazenados na aplicação.
2. *di*: Implementações e interfaces relacionadas ao Dagger2.
3. *ui*: pacotes e classes relacionadas com a interface gráfica.
4. *commons*: Constantes e funções(helpers) utilizadas no projeto.

### Recursos de referência de biblioteca

1. *Picasso* - http://square.github.io/picasso/
2. *RxJava* - https://github.com/ReactiveX/RxJava
3. *RxAndroid* - https://github.com/ReactiveX/RxAndroid
4. *Room* - https://developer.android.com/topic/libraries/architecture/room.html
5. *LiveData* - https://developer.android.com/topic/libraries/architecture/livedata.html
6. *Retrofit* - http://square.github.io/retrofit/
7. *Dagger2* - https://google.github.io/dagger/
