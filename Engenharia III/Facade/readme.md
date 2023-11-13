![facade1](https://github.com/raynaranasc/bertoti/assets/90811047/f5982418-7f50-44b1-859b-81f1942b73d9)

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
