![sINGLETON](https://github.com/raynaranasc/bertoti/assets/90811047/5b42ca64-d750-4ce9-b296-f20fb5f2c242)

```java
public static class Ingresso {
	private static Ingresso ingresso;
	private Ingresso(){}
	public void Ingresso getInstance(){
		if(ingresso==null){
			ingresso = new Ingresso;
		}
		return ingresso;
	}

	public comprar(String documento) {
        System.out.println("Comprando: " + documento);
    }
}
```
