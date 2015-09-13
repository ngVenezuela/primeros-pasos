# ngVenezuela

![logo](https://github.com/ngVenezuela/press-kit/blob/master/img/logo/logo_angular.png)

 
¿Eres nuevo con Angular? Este repo te guiará un poco sobre cómo empezar a conocer este maravilloso framework. Aquí podrás encontrar:

  - [Conceptos Básicos.](#conceptos-basicos) 
  - Códigos de Ejemplo Documentados.
  - [Enlaces y Referecias a Librerias.](#modulos-adicionales)
  - [Recursos en Linea.](#recursos-en-linea)


Somos una comunidad que promueve el aprendizaje colectivo, con miembros dispuestos a enseñar, aprender y compartir conocimientos. Queremos invitarte a que formes parte de ella. Encuentranos en nuetsras redes:

 - [Google Groups](bit.ly/ng-venezuela-google-groups) : Tienes alguna duda sobre el framework ven y participa en nuestro foro.
 - [Telegram](bit.ly/ng-venezuela-telegram): Ḿantente en contacto con los demas mienbros, enterete y comparte recursos y enlaces de interes con nosotros.
 - [Github](https://github.com/ngVenezuela): Conoce, aprende, participa y comparte aportes de la comunidad para la comunidad.



### Que necesito para comenzar a Aprender AngularJS

* Conocimientos de Javascript *
* Tu editor de Texto o IDE Favorito (Como [Sublime](http://www.sublimetext.com/),[Atom](https://atom.io/) o [NotePad](https://notepad-plus-plus.org/))
* Un Navegador Web. 
* Motivación por aprender y dominar este magnifico Framework

**Nota:** Te recomendamos antes de aprender un framework dominar el lenguaje en el que esta basado para aprovechar todas sus bondades.

### Recursos para aprender Javascript
- En Español:
    - [Codecademy](https://www.codecademy.com/tracks/javascript) : Un excelente recurso para aprender lo básico del lenguaje.
    - [Guía de Javascript de MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide): la gente de Mozilla nos ofrece esta excelente guía sobre el lenguaje.

- English:
    - [JavaScript for Cats](http://jsforcats.com/): So easy your human companion could do it too !


## Primeros Pasos
### Conceptos Basicos
- [¿Que es un Framework?](#que-es-un-framework)
- [¿Que es AngularJS?](#que-es-angularjs)
- [¿Ventajas de usar AngularJS?](#ventajas-de-usar-angularjs)
- [Instalar AngularJS](#instalar-angularjs)
- [Directives (Directivas )](#directives)
- [Module (Modulos)](#module)
- [Scope](#scope)
- [Controllers (Controladores)](#controllers)
- [Models (Modelos)](#models)
- [Filters (Filtros)](#filters)
- [Data Binding](#data-binding)
- [Dependecy Injection (Inyección de Dependencias)](#dependecy-injection)
- [Services (Servicios)](#services)
- [Templates (Plantillas)](#templates)
- [Forms (Formularios)](#form)

[Volver](#ngvenezuela)

### Que Es Un Framework

[Volver Indice](#conceptos-basicos)

### Que es AngularJS

**AngularJS** es un *framework javascript* estructural para el desarrollo de aplicaciones web dinamicas del lado del cliente, basado en el 
patrón de diseño **MVVM** (Modelo - Vista - Vista - Modelo) y el desarrollo de sitios SPA (Aplicaciones de una sola página). AngularJs te 
permite *extender la sintaxis de HTML* para expresar clara y concisa tus componentes de aplicacion, esto es gracias a que Angular 
le enseña al navegador una nueva sintaxis a través de la contrucción de [directivas](#directives), así como también de contar con 
características como el [Data-Binding](#data-binding) y [Dependecy Injection](#dependecy-injection) puede ahorrarte líneas de código
que de otra forma tendrías que escribir. Todo esto ocurre dentro del navegador, haciendo de AngularJS el compañero ideal de cualquier 
tecnología del lado del servidor.
[Volver Indice](#conceptos-basicos)

### Ventajas de usar AngularJS
[Volver Indice](#conceptos-basicos)

### Instalar AngularJS
[Volver Indice](#conceptos-basicos)

### Directives
[Volver Indice](#conceptos-basicos)

### Module
[Volver Indice](#conceptos-basicos)

### Scope
[Volver Indice](#conceptos-basicos)

### Controllers
[Volver Indice](#conceptos-basicos)

### Models
[Volver Indice](#conceptos-basicos)

### Filters
Un filtro da formato al valor de una expresion para la visualizacion de los usuarios. Los filtros pueden ser usados en las plantillas de vistas, controladores o servicios. AngularJS cuenta con vaios filtros predeterminados para dar formato como el caso de modena (currency), fecha (Date), mayusculas (uppercase), minisculas (lowercase), json (json) e incluso nos brinda la facilidad de crear nuestros propios filtros.  Para aplicar filtros lo podemos hacer de la siguiente forma:
```
{{ valor | filtro }}

{{ 100 | currency }}
```
puedes aplicar varios filtros con la siguiente sintaxis:
```
{{ valor | filtro1:arg1:arg2:argN }}
```
Puedes ver un pequeno ejemplo de codigo [AQUI](https:github.com/JMEspiz/primeros-pasos/Ejemplos/filter.html).
Para crear tus propios filtros puedes guiarte por este ejemplo en la [documentacion oficial](https://docs.angularjs.org/guide/filter)
```
angular.module('myReverseFilterApp', [])
.filter('reverse', function() {
  return function(input, uppercase) {
    input = input || '';
    var out = "";
    for (var i = 0; i < input.length; i++) {
      out = input.charAt(i) + out;
    }
    // conditional based on optional argument
    if (uppercase) {
      out = out.toUpperCase();
    }
    return out;
  };
})
```
primero se define el modulo de nuestra aplicación angular, luego se usa el método **filter** el cual recibe como primer parámetro el nombre de nuestro filtro personalizado y como segundo una función que retorna una nueva función en donde se especificaran los argumentos y la lógica que definirá nuestro nuevo formato.
[Volver Indice](#conceptos-basicos)

### Data Binding
Data-bindig en aplicaciones Angular hace referencia a la sincronización automática entre los los componentes del modelo ([Model](#models)) y las vista (Views).  Lo cual conlleva a que todo cambio realizado en el modelo estos serán reflejados en la vista y viceversa. Este proceso es conocido como Two-Way Data Binding, donde podemos considerar la vista como una proyección instantánea del modelo, lo que deja a el controlador ([controller](#controllers)) completamente separador de la vista e inconsciente de esta, facilitando las tareas de testing debido a que testear el controlador de forma aislada sin la vista y lo relacioando con dependecias DOM/Browser.
[Volver Indice](#conceptos-basicos)

### Dependecy Injection
[Volver Indice](#conceptos-basicos)

### Services
[Volver Indice](#conceptos-basicos)

### Templates
[Volver Indice](#conceptos-basicos)

### Forms
[Volver Indice](#conceptos-basicos)

### Modulos Adicionales

- [Angular-resource](https://code.angularjs.org/1.4.4/angular-resource.min.js): el módulo **ngResource** provee soporte para interactuar con servicios REST-Full por medio del servicio **$resource**. 
- [Angular-route](https://code.angularjs.org/1.4.4/angular-route.min.js): el modulo **ngRoute** provee servicios de enrutemiento y enlazado profundo, asi como tambien directivas para Aplicaciones Angular.

[Volver](#ngvenezuela)

### Recursos En Linea

- [Guia para Desarrolladores  oficial de AngularJS](https://docs.angularjs.org/guide) (English)
- [Referencia del API oficial de AngularJS](https://docs.angularjs.org/api) (English)
- [Curso de AngularJS en codecademy](https://www.codecademy.com/es/courses/learn-angularjs) (English)
- [Shaping up with angular.JS](http://campus.codeschool.com/courses/shaping-up-with-angular-js/intro) (English)

[Volver](#ngvenezuela)
