### Clases Abstractas


<table align="center" >
  <tr>
    <td align="center" style="padding=0;width=50%;">
      <img align="center" style="padding=0;" src="../images/caseAbstracta.png" />
    </td>
  </tr>
</table>


```java

public abstract class FiguraGeometica{
    //las clase padre no define ocomportamiento
    abstract void dibujar();
}
````

---


```java

pulic class Rectangulo extends FiguraGometrica{

    void dibujar(){
        // comportamiento de la subclase
    }

}

```