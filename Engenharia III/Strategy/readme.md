## Strategy
![Strategy](https://github.com/raynaranasc/bertoti/assets/90811047/a3fc0cee-f53b-4f9c-87eb-6af2deed6309)
```java
public class Ingresso {
   
    private String ingressoDescricao;
    private Cinema cinema;
    
    public Cliente(String descricao, Cinema cinema){
        this.ingressoDescricao = descricao;
        this.cinema = cinema;
    }

    public String getClienteNome() {
        return clienteNome;
    }
    
    public void comprar(){
        tipoCompra.comprar();
    }
    public void setCinema(Cinema cinema){
        this.cinema = cinema
    }
}
```
```java
public interface Cinema {
    
    void comprar();
}
```
```java
public class IngressoMeia implements comprar {
    
    public void comprar(){
        System.out.println("Ingresso de entrada Meia.");
    }
}
```
```java
public class IngressoInteira implements comprar {
    
    public void comprar(){
        System.out.println("Ingresso de entrada Inteira.");
    }
}
```
