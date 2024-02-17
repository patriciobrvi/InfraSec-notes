
## Machete MD+Mermaid
Machete de objetos en Mermaid para MarkDown (MD):

| Símbolos           | Resultado                          
|--------------------|-------------------------------
|Corchetes []        | Crean Rectángulos
|Paréntesis simples()| Crean Rectángulos redondeados
|Doble Paréntesis(())| Crean Círculos
|Llaves {}           | Crean Rombos de Decisión
|Pipe \|texto\|        | Se utiliza para texto fuera de un objeto
|Flecha -->        | Se utiliza para definir ownership

## ejemplo

```mermaid
flowchart LR
A[Rectangulo]
B(Paréntesis)
C((Doble Paréntesis))--> |Texto Pipe| D{Decisión} 
```

## Ejemplo FLujo de markdown + Mermaid 

```mermaid
flowchart TD
    
    A_Inicio((INICIO)) --> |Dato| B_accion[ACCION]
    B_accion --> C_Decision{DECISION}
    C_Decision -->|Dato 1| D[Auto]
    D -->FIN((FIN))
    C_Decision -->|Dato 2| E_accion[Moto] 
    C_Decision -->|Dato 3| F_accion[Camion]
    E_accion --> G(Cuadradondo)
    F_accion --> G
    
    G --> decision_op{Otra Pregunta}
    decision_op --> B_accion
```
