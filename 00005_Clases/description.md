Si tenemos más de un objeto que se comporta **exactamente** de la misma forma, lo que podemos hacer es generalizar ese comportamiento declarando una **clase**. Por ejemplo, si tenemos dos celulares con el mismo saldo inicial y ambos tienen las mismas funcionalidades, `realizarLlamada` y `cargarSaldo` :iphone: con la misma implementación:

```wollok
object celularDeMaria {
  var saldo = 25
  
  method realizarLlamada(){
    saldo -= 5
  }
  
  method cargarSaldo(pesos){
    saldo += pesos
  }
}

object celularDeLucrecia {
  var saldo = 25
  
  method realizarLlamada(){
    saldo -= 5
  }
  
  method cargarSaldo(pesos){
    saldo += pesos
  }
}
```

Podemos generalizarlos en una **clase** `Celular`:

```wollok
class Celular {
  var saldo = 25
  
  method realizarLlamada(){
    saldo -= 5
  }
  
  method cargarSaldo(pesos){
    saldo += pesos
  }
}
```

> Veamos si se entiende: como `bouba` y `kiki` se comportan exactamente de la misma forma, **generalizalos** creando una clase `Zombi` que entienda los mismos cinco mensajes que ellos. Podés ver el código de ambos zombis en la solapa Biblioteca. 