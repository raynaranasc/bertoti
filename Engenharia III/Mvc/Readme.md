
![mvc](https://github.com/raynaranasc/bertoti/assets/90811047/127975cf-49a5-412f-a3e3-24a30979bca8)

MVC (Strategy + Composite + Observer + Facade + Singleton)

```java
package view;
import java.util.List;

public interface Observer {

    public void update(List l);

}
```

```java
package view;

import java.util.List;

import model.Pipoca;

import controller.Ingresso;

public class View implements Observer{
	
	private Ingresso i;
	private List listPipoca
	
	public void setI(Ingresso ingresso){
		i = ingresso;
	}
	
	public void update(List l){
		listaPipoca = l;
        this.p.emitirIngresso();
		
	}
	
    public void imprimirNotaPaulista(){
        if(!listaPipoca.isEmpty()){
            for(Object j: listaPipoca){
                Pipoca p = (Pipoca)j;
                System.out.println(s.getNome()+ s.getTamanho() +s.getValor());
            }
        }

    }

    public void imprimirIngressoMeia(){
        System.out.println("\nTipo: meia");
        System.out.println("CPF do comprador: xxx.xxx.xxx-xx");
    }

}
    public void imprimirIngressoInteira(){
        System.out.println("\nTipo: inteira");
        System.out.println("CPF do comprador: xxx.xxx.xxx-xx");
    }

}
```
```java
  package controler;

  public interface Ingresso {
    public void emitirIngresso();

}
```

```java
package controler;

import model.Catalogo;
import view.View;

public class TipoMeia implements Ingresso{

    private View v;
    private Cinema c;

    public void setV(View view){
        v = view;
    }

    public void emitirIngresso(){
        v.imprimirNotaPaulista();
        v.imprimirIngresso();
    }

}
```
```java
package controler;

import model.Catalogo;
import view.View;

public class TipoInteira implements Ingresso{

    private View v;
    private Cinema c;

    public void setV(View view){
        v = view;
    }

    public void emitirIngresso(){
        v.imprimirNotaPaulista();
        v.imprimirIngresso();
    }

}
```

```java
package model;
import java.util.List;
import java.util.LinkedList;
import view.Observer;

public class Cinema implements Subject {

    private List<Pipoca> pipoca;
    private List<Observer> observers;

    public Cinema(){
        pipoca = new LinkedList<>();
        observers = new LinkedList<>();
    }

    public void registerObserver(Observer o){
        observers.add(o);
    }

    public void notifyObservers(List encontrados){
        for(Observer o : observers){
            o.update(encontrados);
        }
    }

    public void addPipoca(Pipoca p){
        shows.add(s);
    }

    public void buscarPipoca(Pipoca p){
        List<Pipoca> encontrados = new LinkedList<>();
        for(Pipoca pipocaCinema : pipoca){
            if(pipoca.matches(s)) {
                encontrados.add(pipocaCinema);
            }
        }
        notifyObservers(encontrados);
    }

    public void adicionarPipoca(String nome, char tamanho, double valor){
        Pipoca pipoca = new Pipoca(nome, tamanho, valor);
        addPipoca(pipoca);
    }

    public void buscarPipocaPorNome(String nome, char tamanho, double valor){
        Pipoca pipoca = new Pipoca(Nome, 0);
        buscarPipoca(pipoca);
    }

    public void buscarPipocaPorValorETamanho(String nome, char tamanho, double valor){
        Pipoca pipioca = new Pipoca(tamanho, valor);
        buscarPipoca(pipoca);
    }
}

```

```java
package model;

import java.util.List;

import view.Observer;

public interface Subject {

    public void registerObserver(Observer o);
    public void notifyObservers(List encontrados);

}
```
```java
package model;

public class Pipoca {

    private String nome;
    private char tamanho;
    private double valor;

    public Pipoca(String n, char t, double v){
        nome = n;
        tamanho = t;
        valor = v;
    }

    public String getNome(){
        return nome;
    }

    public char getTamanho(){
        return tamanho;
    }
    public double getValor(){
        return valor;
    }

    public boolean matches(Pipoca){
        if(!nome.equals(s.nome)) return false;
        if(tamanho!=s.tamanho) return false;
        if(valor!=s.valor) return false;
        return true;
    }

}
```java
import java.util.List;

public class Facade {
    private Controller controller;
    private View view;

    public Facade() {
        this.controller = new Controller();
        this.view = new View(controller);
    }

    public List<Show> emitirIngresso() {
        return controller.lista();
       
    }

    public List<Show> imprimirIngresso() {
        return controller.lista();
       
    }
}
```
```java
import java.util.List;

class Observador implements Observer {
    private String email;

    public Observador(String email) {
        this.pipoca = pipoca;
    }

    public void update(List l) {
        System.out.println("A lista foi atualizada");
      
    }

}
```
