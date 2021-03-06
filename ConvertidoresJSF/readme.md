## Convertidores JSF

- Los Convertidores cubren la necesidad de asignar valores entre la vista y el modelos de manera automatica

```
|VISTA -->(Conversion a un tipo de datos) --> MODELO |
```


```
|VISTA <-- (Formato a Desplegar) <-- MODELO |
```


## Convertidores Implicitos y Explicitos

- Conversiones Implicitas:

Son todas las conversiones que JSF realiza de manera automatica, por ejemplo al usar tipos primitivos, BigInteger o String

```java
<h:inputText id="edadId" value="#{empleadoBean.edad}">  
```

## Conversiones Explicitas

Utilizando el atributo ```converter```

```java
<h:inputText id="edadId" value="#{empleadoBean.edad}"
converter="javax.faces.Integer">  
```

Utilizando el componente ```converter```

```java
<h:inputText value="#{empleadoBean.edad}">
    <f:converter convertedId="javax.faces.Integer"/>  
</h:inputText>
```

## Convertidores Personalizados

- JSF permite crear convertidores personalizados
- Pass para crear y utilizar una clase Converter

