![Observer](https://github.com/raynaranasc/bertoti/assets/90811047/d8f4a6ab-ada4-4677-a0b8-2d5fa0ae21c0)

```java
import java.util.ArrayList;
import java.util.List;

public class Ingresso {
    private List<Observer>:observers;
    private EmpresaNome: String
    private IngressoFilme:String
    
    public Ingresso(){
        this.observers = new ArrayList<>();
        this.EmpresaNome: String
        this.funcionarioNome = String
    }

    public void setFuncionarioNome(String nome){
        this.empresaNome = nome
    }

    public void addObserver(Observer observer){
        this.observers.add(observer);
    }
    
    public void postFuncionarioDados(String nome){
        setFuncionarioNome(nome)
        notify(nome)
    }

    public void notify(String nome){
        this.observers.stream().forEach(item -> {
           item.update(nome) ;
        });
    }
    
}
```
