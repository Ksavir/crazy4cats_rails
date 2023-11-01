# Crazy4Cats

Blog sobre gatos creado en Ruby on Rails.

## Descripción

Esta página funciona principalmente mediante el uso de un CRUD para el manejo de las noticias asi como comentarios dejados por otros usuarios y su gestión a través de una base de datos, en este caso PostgreSQL. Ademas hace uso de las relaciones N a N con un sistema de reacciones, Entre sus funcionalidades destacan:

- Crear nuevas noticias y comentarios que serán almacenados en la base de datos.
- Editar las noticias y comentarios creados.
- Borrar una noticia si no te gusta su contenido.
- Mostrar en su índice todos las noticias creadas, mostrando siempre las últimos noticias al comienzo.
- Muestra los comentarios de cada noticia.
- Ingresa con tu cuenta o crea una propia.
- Los comentarios y publicaciones solo podrán ser borradas por administradores o el mismo usuario que creo la publicación y/o comentario.
- Visitantes podrán dejar sus comentarios en las publicaciones.
- Solo los administradores podrán borrar o editar comentarios dejados por visitantes.

## Importante

Por defecto todo usuario nuevo de la pagina se le asigna el rol de user, si deseas ingresar y probar la pagina como administrador usa la siguiente cuenta: (esto solo en caso de que la pagina este en Heroku u otro servicio)

- mail: <admin@mail.com>
- password: 123456

```bash
# para ingresar a la consola de rails
rails c

# Cambia el mail, password, pero recuerda dejar el role "admin"
User.create(email: 'admin@mail.com', password: '123456', role: 'admin')
```

Listos con esos pasos ya podrás probar la pagina como administrador.

Si deseas probar la pagina como un Usuario normal solo crea una cuenta siguiendo el link en la barra de navegaciones

### Pre-requisitos 📋

- Sistema Operativo: Windows, Ubuntu o macOS
- Lenguaje de programación: Ruby 3.2.2
- Framework Rails: 7.0.6
- PostgreSQL: 14.8

### Instalación 🔧

Clona el repositorio con el siguiente comando:

```bash
git clone https://github.com/ksavir/crazy4cats_rails
```

En la terminal, accede a la carpeta donde se encuentra el repositorio y ejecuta (recuerda que para que esto funcione, debes tener instalado Ruby y la gema bundle):

```bash
bundle install
```

Inicia la base de datos con el siguiente comando:

```bash
rails db:create db:migrate db:seed
```

Finalmente, ejecuta el proyecto con el siguiente comando y ve a la dirección IP que aparecerá en la consola:

```bash
rails s
```

## Construido Con 🛠️

- [Ruby](https://www.ruby-lang.org/es/) - El lenguaje utilizado
- [Ruby on Rails](https://rubyonrails.org) - El framework web utilizado
- [Ruby gems](https://rubygems.org) - Gestión de dependencias
- [Postgresql](https://www.postgresql.org) - Sistema de base de datos
- [Bootstrap](https://getbootstrap.com/) - Framework de CSS
- [Devise](https://github.com/heartcombo/devise) - Gema para autentificación y permisos.

## Versionado 📌

Use [Git](https://git-scm.com) para el versionado.

## Autores ✒️

- **Kevin Rivas** Encuéntrame en [github](https://github.com/ksavir)
