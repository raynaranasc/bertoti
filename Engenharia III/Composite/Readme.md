![composite](https://github.com/raynaranasc/bertoti/assets/90811047/7e2be87c-2252-472f-8fa6-aee9d2d79156)
|Código

```java
import java.util.ArrayList;
import java.util.List;

public class Compras implements Produto {
  private List<Produto> Produto;
  private double valorTotal;

  public Compras() {
    this.produto= new ArrayList<>();
    this.valorTotal = 0.00;
  }

  @Override
  public void comprar() {
    System.out.println("Valor da sua compra R$"+this.valorTotal);
  }

  @Override
  public double getValorTotal(){
    return this.valorTotal;
  }

  public void addProduto(Produto produto) {
    produto.add(produto);
    this.valorTotal += produto.getValorTotal();
  }

  public void delProduto(Produto produto) {
    produto.remove(produto);
    this.valorTotal -= produto.getValorTotal();
  }

  public List<Produto> getProduto() {
    return produto;
  }
}
```

```java
public interface Produto {
    void comprar();
    double getValor();
}
```

```java
public class Ingresso implements Produto {
  private String ingressoFilme;
  private String tipoCompra;

  public Ingresso(String ingressoFilme, String tipoCompra) {
    this.ingressoFilme = ingressoFilme;
    this.tipoCompra = tipoCompra;
  }

public void setIngresso(ingressoFilme, tipoCompra){
    this.ingressoFilme = ingressoFilme
    this.tipoCompra = tipoCompra
}

  public double getingressoFilme() {
    return this.ingressoFilme;
  }

  @Override
  public void comprar() {
      System.out.println("Comprando ingresso" + this.ingressoFilme + "tipoCompra:  " + this.tipoCompra);
  }
}
```

```java
public class Pipoca implements Produto {
  private String nome;
  private char tamanho;
  private double valor;

  public Pipoca(String nome, char tamanho, double valor) {
    this.nome = nome;
    this.tamanho = tamanho;
    this.valor = valor;
  }

public void setPipoca(Double valor, char tamanho, String nome){
    this.nome = nome
    this.tamanho = tamanho
    this.valor = valor
}

  public double getValor() {
    return this.valor;
  }

  @Override
  public void comprar() {
      System.out.println("Comprando pipoca " + this.nome + this.tamanho + "valor:  " + this.valor);
  }
}
```
