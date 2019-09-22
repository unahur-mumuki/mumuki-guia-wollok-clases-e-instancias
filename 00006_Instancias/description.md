Como habrás visto, definir una clase es muy similar a definir un objeto. Tiene métodos, atributos... ¿cuál es su particularidad, entonces? La clase es nos sirve como **molde** para crear nuevos objetos. :open_mouth:

Momento, ¿cómo es eso? ¿Una clase permite **crear nuevos objetos**? ¿Cuántos?

¡Así es! ¡Todos los que se necesiten! A la acción de crear objetos a partir de una clase la llamamos **instanciar** y decimos que el objeto creado es una **instancia** de esa clase.

Aprovechemos la clase `Celular` para **instanciar** los celulares de María y Lucrecia:

```wollok
const celularDeMaria = new Celular()
const celularDeLucrecia = new Celular()
```

`Celular`, al igual que _todas las clases_, puede usarse con la palabra new para crear una nueva **instancia** de esa clase.

> ¡Ahora te toca a vos! Definí las constantes `bouba` y `kiki` y asignales **instancias** de la clase `Zombi`.