# Tablas-de-senku
tipo tablero(tipo tab[][9],int opcion){
    tipo ingles [9][9] =   {{'x','x','x','x','x','x','x','x','x'},
                            {'x','x','x','O','O','O','x','x','x'},
                            {'x','x','x','O','O','O','x','x','x'},
                            {'x','O','O','O','O','O','O','O','x'},
                            {'x','O','O','O','+','O','O','O','x'},
                            {'x','O','O','O','O','O','O','O','x'},
                            {'x','x','x','O','O','O','x','x','x'},
                            {'x','x','x','O','O','O','x','x','x'},
                            {'x','x','x','x','x','x','x','x','x'}};

    tipo frances [9][9] = {{'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},
                           {'x','x','x','x','x','x','x','x','x'},};

    for(int fila = 0; fila < 9 ; fila++){
        for(int columna = 0; columna < 9 ; columna++){
            if(opcion == 1)
                tab[fila][columna] = ingles[fila][columna];
            else{
                if(opcion == 2)
                    tab[fila][columna] = frances[fila][columna];
            }
        }
    }
    return tab[9][9];
