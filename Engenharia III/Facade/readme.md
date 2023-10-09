![Facade](https://github.com/raynaranasc/bertoti/assets/90811047/c89bb0e3-f56f-4c53-9eb1-25fd4a59c069)

```java
class Ingresso {
    private IngressoMeia ingressoMeia;
    private IngressoInteira ingressoInteira;


    public Ingresso() {
        ingressoMeia = new IngressoMeia();
        ingressoInteira = new IngressoInteira();
    }

    public void comprarMeia(String meiaFile) {
        ingressoMeia.comprarMeia(meiaFile);
    }

    public void comprarIngressoInteira(String ingressoInteiraFile) {
        ingressoInteirao.comprarIngressoInteira(ingressoInteiraFile);
    }
}
```
```java
class IngressoMeia {
    public void comprarMeia(String meiaFile) {
        System.out.println("Comprando ingresso Meia: " + meiaFile);
    }
}
```
```java
class IngressoInteira {
    public void comprarInteira(String inteiraFile) {
        System.out.println("Comprando ingresso Inteira: " + inteiraFile);
    }
}
```
