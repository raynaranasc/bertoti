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

