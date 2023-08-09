![20230730_134526](https://github.com/notebook-t/notebook-t/assets/140947135/5171d43f-94d2-47f1-8f8b-8cd8d85adaef)
El archivo `readme.md` es generalmente utilizado en los proyectos de software para proporcionar información relevante sobre el proyecto. 
Contiene información sobre cómo instalar, configurar y utilizar el software, así como cualquier otro detalle importante que los usuarios o desarrolladores deben conocer. 
Además, el archivo `readme.md` puede incluir información sobre el propósito del proyecto, los requisitos del sistema, las dependencias, los pasos de instalación, la estructura de archivos y directorios, y cualquier otra información relevante que los desarrolladores o usuarios necesiten saber.
Para conocer más a profundidad acerca de este tipo archivo empecemos por el principio.

# Markdown 
Es un lenguaje sencillo, con una sintaxis muy resumida y fácil de recordar e interpretar por humanos, que permite escribir HTML sin la necesidad de usar etiquetas, lo que redunda en velocidad de escritura y facilidad de mantenimiento del contenido. Existen multitud de liberías, para cualquier lenguaje, que permiten convertir el código markdown en HTML y viceversa, por lo que usarlo en cualquier tipo de aplicación es también muy sencillo y directo.
- [Para qué se usa Markdown](https://desarrolloweb.com/home/markdown#track263)
- [Archivos Markdown](https://desarrolloweb.com/home/markdown#track198)
- [Sintaxis](https://desarrolloweb.com/home/markdown#track199)

## Markdown en GitHub para documentar repositorios en el README.md
- [Librería para reconocer Markdown en JavaScrip](https://desarrolloweb.com/home/markdown#track261)
- [notebook-t](https://desarrolloweb.com/home/markdown#track242)
  
> A continuación, se muestran algunos ejemplos de cómo utilizar Markdown en GitHub para agregar formato al archivo README.md:

1. Encabezados: Los encabezados se utilizan para estructurar el contenido y se definen agregando uno o varios símbolos de numeral (#) antes del texto. Por ejemplo:


![header_transparent_bg@3x](https://github.com/notebook-t/notebook-t/assets/140947135/e477731a-ca46-4b16-963d-a175c4e9addd)
```

# Bundle

Esta guía asume que tiene [Ruby](https://www.ruby-lang.org/en/downloads/) instalado. Si no tiene instalado Ruby, hágalo primero y luego vuelva a consultar aquí.

Cualquier distribución moderna de Ruby viene con Bundler preinstalado de forma predeterminada.

¡Empezar con Bundler es fácil! Especifique sus dependencias en un Gemfile en la raíz de su proyecto:

```

```
source 'https://rubygems.org'
gem 'nokogiri'
gem 'rack', '~> 2.2.4'
gem 'rspec'
```
Instale todas las gemas requeridas de sus fuentes especificadas:

```
$ bundle install
$ git add Gemfile Gemfile.lock
```

El segundo comando agrega Gemfile y Gemfile.lock a su repositorio. Esto garantiza que otros desarrolladores de su aplicación, así como su entorno de implementación, usarán el mismo código de terceros que está usando ahora.

Dentro de su aplicación, cargue el entorno incluido:

```
require 'bundler/setup'

# require your gems as usual
require 'nokogiri'
```

Ejecute un ejecutable que viene con una gema en su paquete:

```
$ bundle exec rspec spec/models
```

En algunos casos, la ejecución de ejecutables sin `bundle exec` puede funcionar, si el ejecutable está instalado en su sistema y no genera ninguna gema que entre en conflicto con su paquete.

Sin embargo, esto no es fiable y es la fuente de un dolor considerable. Incluso si parece que funciona, es posible que no funcione en el futuro o en otra máquina.

Finalmente, si desea una forma de obtener un acceso directo a las gemas en su paquete:
```
$ bundle install --binstubs
$ bin/rspec spec/models
```
Los ejecutables instalados bin están dentro del alcance del paquete y siempre funcionarán.

## Crear una rubygem con Bundler

Bundler también es una manera fácil de crear nuevas gemas. Al igual que puede crear un proyecto de Rails estándar con rails new, puede crear un proyecto de gema estándar con bundle gem.

Cree una nueva gema con un archivo README, .gemspec, Rakefile, estructura de directorios y toda la plantilla básica que necesita para describir, probar y publicar una gema:

```
$ bundle gem my_gem
Creating gem 'my_gem'...
      create  my_gem/Gemfile
      create  my_gem/.gitignore
      create  my_gem/lib/my_gem.rb
      create  my_gem/lib/my_gem/version.rb
      create  my_gem/my_gem.gemspec
      create  my_gem/Rakefile
      create  my_gem/README.md
      create  my_gem/bin/console
      create  my_gem/bin/setup
      create  my_gem/CODE_OF_CONDUCT.md
      create  my_gem/LICENSE.txt
      create  my_gem/.travis.yml
      create  my_gem/test/test_helper.rb
      create  my_gem/test/my_gem_test.rb
Initializing git repo in ./my_gem
```
### Usar paquete con
| [RIELES](https://bundler.io/guides/rails.html) | [SINATRA](https://bundler.io/guides/sinatra.html) | [RUBYGEMS](https://bundler.io/guides/rubygems.html) | [RUBYMOTION](https://bundler.io/guides/rubymotion.html) |

2. Estilos de texto: Se pueden aplicar estilos a texto como cursiva, negrita o tachado utilizando caracteres especiales. Por ejemplo:

```
*Texto en cursiva*
**Texto en negrita**
~~Texto tachado~~
```

3. Listas: Se pueden crear listas ordenadas utilizando números o listas desordenadas utilizando viñetas. Por ejemplo:

```
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
```

```
- Primer elemento
- Segundo elemento
- Tercer elemento
```

4. Enlaces: Para agregar enlaces a otros sitios web, se utiliza la siguiente sintaxis:

```
[Texto del enlace](URL_del_enlace)
```

Por ejemplo:

```
[Aprende Markdown en GitHub](https://guides.github.com/features/mastering-markdown/)
[~ibarracar0](https://dev.launchpad.net/)
```

5. Imágenes: Para agregar imágenes al archivo README.md, se utiliza la siguiente sintaxis:

```
![Texto alternativo](URL_de_la_imagen)
```

Por ejemplo:

```
![20230730_134526](https://github.com/notebook-t/notebook-t/assets/140947135/5171d43f-94d2-47f1-8f8b-8cd8d85adaef)
```

6. Bloques de código: Para mostrar código de programación, se utiliza la siguiente sintaxis:

![feedback](https://github.com/notebook-t/notebook-t/assets/140947135/d3f5c424-a56d-415d-93ff-a86c1da63089)





