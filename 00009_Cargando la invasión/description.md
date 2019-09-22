Agreguemos una clase para modelar invasiones de zombies

```wollok
class Invasion {
  var zombis = []
  
  method saludTotal() = zombis.sum({zombi => zombi.salud()})
  method agregarZombi(zombi) { zombis.add(zombi) }
}
```

En un REPL creamos una invasión y ... le queremos agregar un zombie. Podemos escribirlo de estas tres formas

```
>>> var invasion = new Invasion()
>>> invasion.agregarZombi(Zombi)
```

```
>>> var invasion = new Invasion()
>>> invasion.agregarZombi(new Zombi())
```

```
>>> var invasion = new Invasion()
>>> var zombito = new Zombi()
>>> invasion.agregarZombi(zombito)
```

¿Cuál/es de estas es/son correcta/s?
