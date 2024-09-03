# Proyecto-1
```mermaid
graph TD
    subgraph Inicializar
        A1["Para cada columna de la matriz"]
        A2["Filas a evaluar, fila 1 =22, fila 2 = 66, fila 3 = 154, fila 4 = 198"]
    end

    subgraph Evaluaciones
        B01["A qué jugador o jugadores pertenecen las str?"]
        B02["A qué jugador o jugadores pertenecen las str?"]
        B03["A qué jugador o jugadores pertenecen las str?"]
        B04["A qué jugador o jugadores pertenecen las str?"]
        B05["A qué jugador o jugadores pertenecen las str?"]
        B06["A qué jugador o jugadores pertenecen las str?"]
        B07["A qué jugador o jugadores pertenecen las str?"]
        B08["A qué jugador o jugadores pertenecen las str?"]
        B09["A qué jugador o jugadores pertenecen las str?"]
        B010["A qué jugador o jugadores pertenecen las str?"]
        B011["A qué jugador o jugadores pertenecen las str?"]
        B012["A qué jugador o jugadores pertenecen las str?"]
        B013["A qué jugador o jugadores pertenecen las str?"]
        B014["A qué jugador o jugadores pertenecen las str?"]
        B015["A qué jugador o jugadores pertenecen las str?"]
        B1["Fila 1 tiene str y demás vacías?"]
        B2["Fila 2 tiene str y demás vacías?"]
        B3["Fila 3 tiene str y demás vacías?"]
        B4["Fila 4 tiene str y demás vacías?"]
        B5["Fila 1 y 2 tienen str y demás vacías?"]
        B6["Fila 3 y 4 tienen str y demás vacías?"]
        C1["Fila 1 y 4 tienen str?"]
        C2["Fila 2 y 4 tienen str?"]
        C3["Fila 1 y 3 tienen str?"]
        C4["Fila 1, 2 y 4 tienen str?"]
        C5["Fila 1, 3 y 4 tienen str?"]
        C6["Fila 2 y 3 tienen str?"]
        C7["Fila 1, 2 y 3 tienen str?"]
        C8["Fila 2, 3 y 4 tienen str?"]
        C9["Filas 1, 2, 3 y 4 tienen str?"]
        C10["Ninguna de las filas tienen str?"]
    end

    subgraph Calculos
        D1["Calcular vida y daño del jugador fila 1"]
        D2["Calcular vida y daño del jugador fila 2"]
        D3["Calcular vida y daño del jugador fila 3"]
        D4["Calcular vida y daño del jugador fila 4"]
        D5["Calcular vida y daño de jugadores fila 1 y 2"]
        D6["Calcular vida y daño de jugadores fila 3 y 4"]
        E1["Calcular vida y daño del jugador de fila 1 y fila 4"]
        E2["Calcular vida y daño del jugador de fila 2 y fila 4"]
        E3["Calcular vida y daño del jugador de fila 1 y fila 3"]
        E4["Calcular vida y daño del jugador de fila 1, 2 y 4"]
        E5["Calcular vida y daño del jugador de fila 1, 3 y 4"]
        E6["Calcular vida y daño del jugador de fila 2 y 3"]
        E7["Calcular vida y daño del jugador de fila 1, 2 y 3"]
        E8["Calcular vida y daño del jugador de fila 2, 3 y 4"]
        E9["Calcular vida y daño del jugador de fila 1, 2, 3 y 4"]
        E10["Filas vacías"]
    end

    subgraph Acciones
        F1["Goles primer jugador += daño del jugador primera fila"]
        F2["Goles primer jugador += daño del jugador segunda fila"]
        F3["Goles segundo jugador += daño del jugador tercera fila"]
        F4["Goles segundo jugador += daño del jugador cuarta fila"]
        F5["Goles primer jugador += daño del jugador primera fila más daño del jugador segunda fila"]
        F6["Goles segundo jugador += daño del jugador tercera fila más daño del jugador cuarta fila"]
        G1["Vida jugador línea 1 -= Daño jugador línea 4 y vida jugador línea 4 -= daño jugador línea 1"]
        G2["Vida jugador línea 2 -= Daño jugador línea 4 y vida jugador línea 4 -= daño jugador línea 2"]
        G3["Vida jugador línea 1 -= Daño jugador línea 3 y vida jugador línea 1 -= daño jugador línea 3"]
        G4["Vida jugador línea 2 -= Daño jugador línea 4 y vida jugador línea 4 -= daño jugador línea 2"]
        G5["Vida jugador línea 1 -= Daño jugador línea 3 y vida jugador línea 3 -= daño jugador línea 1"]
        G6["Vida jugador línea 2 -= Daño jugador línea 3 y vida jugador línea 3 -= daño jugador línea 2"]
        G7["Vida jugador línea 2 -= Daño jugador línea 3 y vida jugador línea 3 -= daño jugador línea 2"]
        G8["Vida jugador línea 2 -= Daño jugador línea 3 y vida jugador línea 3 -= daño jugador línea 2"]
        G9["Vida jugador línea 2 -= Daño jugador línea 3 y vida jugador línea 3 -= daño jugador línea 2"]
        

    end

    subgraph Condiciones
        H4["Vida jugador línea 4 <= 0?"]
        H5["Vida jugador línea 1 <=0?"]
        H7["Vida jugador línea 3 <= 0?"]
        H8["Vida jugador línea 2 <= 0?"]
        H91["Vida jugador línea 3 <= 0?"]
        H92["Vida jugador línea 2 <= 0?"]
    end

    subgraph Ultimas acciones
        U41["Goles primer jugador += daño jugador línea 1"]
        U42["Vida jugador línea 4 -= daño jugador línea 1"]
        U51["Goles segundo jugador += daño jugador línea 4"]
        U52["Vida jugador linea 1 += daño jugador linea 4"]
        U71["Goles primer jugador += daño jugador liena 1"]
        U72["Vida jugador linea 3 -= daño jugador linea 1"]
        U81["Goles segundo jugador += daño jugador linea 4"]
        U82["Vida jugador linea 2 -= daño jugador linea 4"]
        U91["Vida jugador linea 4 -= daño jugador lnea 1"]
        U92["vida jugador linea 3 -= daño jugador linea 1"]
        U93["Vida jugador linea 1 -= daño jugadro linea 4"]
        U94["Vida jugador linea 2 -= daño jugador linea 4"]

        I["Siguiente columna"]
    end


    A1 --> A2
    A2 --> B1
    B1 -- "Sí" --> B01
    B1 -- "No" --> B2
    B2 -- "Sí" --> B02
    B2 -- "No" --> B3
    B3 -- "Sí" --> B03
    B3 -- "No" --> B4
    B4 -- "Sí" --> B04
    B4 -- "No" --> B5
    B5 -- "Sí" --> B05
    B5 -- "No" --> B6
    B6 -- "Sí" --> B06
    B6 -- "No" --> C1
    C1 -- "Sí" --> B07
    C1 -- "No" --> C2
    C2 -- "Sí" --> B08
    C2 -- "No" --> C3
    C3 -- "Sí" --> B09
    C3 -- "No" --> C4
    C4 -- "Sí" --> B010
    C4 -- "No" --> C5
    C5 -- "Sí" --> B011
    C5 -- "No" --> C6
    C6 -- "Sí" --> B012
    C6 -- "No" --> C7
    C7 -- "Sí" --> B013
    C7 -- "No" --> C8
    C8 -- "Sí" --> B014
    C8 -- "No" --> C9
    C9 -- "Sí" --> B015
    C9 -- "No" --> C10
    C10 -- "Correcto" --> E10

    B01 --> D1
    B02 --> D2 
    B03 --> D3
    B04 --> D4
    B05 --> D5
    B06 --> D6
    B07 --> E1
    B08 --> E2
    B09 --> E3
    B010 --> E4
    B011 --> E5
    B012 --> E6
    B013 --> E7
    B014 --> E8
    B015 --> E9

    D1 --> F1
    D2 --> F2
    D3 --> F3
    D4 --> F4
    D5 --> F5
    D6 --> F6

    E1 --> G1
    E2 --> G2
    E3 --> G3
    E4 --> G4
    E5 --> G5
    E6 --> G6
    E7 --> G7
    E8 --> G8
    E9 --> G9

    G4 --> H4
    G5 --> H5
    G7 --> H7
    G8 --> H8
    G9 --> H91
    G9 --> H92

    H4 -- "Sí" --> U41
    H4 -- "No" --> U42
    H5 -- "Sí" --> U51
    H5 -- "No" --> U52
    H7 -- "Sí" --> U71
    H7 -- "No" --> U72
    H8 -- "Sí" --> U81
    H8 -- "No" --> U82
    H91 -- "Sí" --> U91
    H91 -- "No" --> U92
    H91 -- "Sí" --> U93
    H91 -- "No" --> U94

    E10 --> I
    F1 --> I
    F2 --> I
    F3 --> I
    F4 --> I
    F5 --> I
    F6 --> I
    G1 --> I
    G2 --> I
    G3 --> I
    G6 --> I
    U41 --> I
    U42 --> I
    U51 --> I
    U52 --> I
    U71 --> I
    U72 --> I
    U81 --> I
    U82 --> I
    U91 --> I
    U92 --> I
    U93 --> I
    U94 --> I
    
```
