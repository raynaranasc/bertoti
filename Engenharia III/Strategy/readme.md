## Strategy
 ![1](https://github.com/raynaranasc/bertoti/blob/main/Engenharia%20III/Strategy-Images/Diagrama.png)
```java
public class Ingresso {
   
    private String ingressoFilme;
    private TipoCompra tipoCompra;
    
    public Ingresso(String filme,TipoCompra tipoCompra){
        this.ingressoFilme = filme;
        this.tipoCompra = tipoCompra;
    }

    public String getTipoCompra() {
        return tipoCompra;
    }
    
    public void comprar(){
        show.participar();
    }
    
    }
}
```
```java
public interface TipoCompra {
    
    void participar();
}
```
```java
public class CompraMeia implements Show {
    
    public void participar(){
        System.out.println("Ingresso Meia.");
    }
}
```
```java
public class CompraInteira implements Show {
    
    public void participar(){
        System.out.println("Ingresso Inteira.");
    }
}
```
