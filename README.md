# RUTA-MAS-CORTA

<h2>Buscar la ruta mas corta<h2>

<p>Colocaremos el código en una función para hacer el llamado cundo sea necesario</p>
<pre>
def inicio():
</pre>

# Pedimos al usuario que introdusca las respectivas distancias

<p>Pedimos al usuario que introdusca las distancias que seran almacenadas en bariables para poderlas manejar mejor</p>
<pre>
    print("El camino más corto y más beneficioso para Usted")
    print(40*"-")
    AB = float(input("Ingrese la distancia del punto A a B :  "))
    AJ = float(input("Ingrese la distancia del punto A a J :  "))
    AF = float(input("Ingrese la distancia del punto A a F :  "))
    BJ = float(input("Ingrese la distancia del punto B a J :  "))
    BF = float(input("Ingrese la distancia del punto B a F :  "))
    JF = float(input("Ingrese la distancia del punto J a F :  "))
    print("------------------------------------------------------------------")
    inicio = input("¿ De que punto desea iniciar ? (opciones F,  J, B, A) :  ")
    print("___________________________________________________________________")
    a1 = BF
    a2 = JF
    a3 = AF
    a4 = AB
    a5 = BJ
    a6 = AJ
</pre>
<p>Combertimos al caracter introducido en mayusculas para emparejar con las funciones "if"</p>
<pre>
    inicio =inicio.upper()
</pre>

# Inicio Por F

<p>Si el usuario decide iniciar por la letra <b>"F"</b> se ejecutara el siguinete código que compobara cada una de las rutas eligiendo la mas corta de punto a punto</p>
<pre>
    if inicio == 'F':
        print(30*"-")
        print("Iniciara por el punto     = F ")
        print(30*"-")
        if (a1 <= a3 )and(a1<=a2):
            print(30*"-")
            print("Luego pasara por el punto = B")
            print(30*"-")
            if (a4 <= a5):
                print(30*"-")
                print("Pasara por el punto       = A")
                print(30*"-")
                print("Terminara por el punto    = J ")
                print(30*"-")
            elif (a5 < a4):
                print(30*"-")
                print("Pasara por el punto       = J")
                print(30*"-")
                print("Terminara por el punto    = A")
                print(30*"-")
        elif (a3 < a1 )and(a3 < a2):
            print(30*"-")
            print("Luego pasara por el punto = A")
            print(30*"-")
            if (a4 < a6):
                print(30*"-")
                print("Pasara por el punto       = B")
                print(30*"-")
                print("Terminara por el punto    = J")
                print(30*"-")
            elif (a6 < a4):
                print(30*"-")
                print("Pasara por el punto       = J")
                print(30*"-")
                print("Terminara por el punto    = B")
                print(30*"-")
        elif (a2 < a5 )and(a2 < a6):
            print(30*"-")
            print("Luego pasara por el punto = J")
            print(30*"-")
            if (a5 < a6):
                print(30*"-")
                print("Pasara por el punto       = B")
                print(30*"-")
                print("Terminara por el punto    = A")
                print(30*"-")
            elif (a6 < a5):
                print(30*"-")
                print("Pasara por el punto       = A")
                print(30*"-")
                print("Terminara por el punto    = B")
                print(30*"-")
</pre>

# Inicio por "A"

<p>Si el usuario decide iniciar por el punto "A" se ejecutara el siguinete código que compobara cada una de las rutas eligiendo la mas corta de punto a punto</p>

<pre>
    if inicio == 'A':
        print(30*"-")
        print("Iniciara por el punto     = A")
        print(30*"-")
        if (a3 <= a4 )and(a3<=a6):
            print(30*"-")
            print("Luego pasara por el punto = F")
            print(30*"-")
            if (a1 <= a2 ):
                print(30*"-")
                print("Pasara por el punto       = B")
                print(30*"-")
                print("Terminara por el punto    = J")
                print(30*"-")
            elif (a2 < a1 ):
                print(30*"-")
                print("Pasara por el punto       = J")
                print(30*"-")
                print("Terminara por el punto    = B")
                print(30*"-")
        elif (a4 < a3 )and(a4 < a6):
            print(30*"-")
            print("Luego pasara por el punto = B")
            print(30*"-")
            if (a5 < a1):
                print(30*"-")
                print("Pasara por el punto       = J")
                print(30*"-")
                print("Terminara por el punto    = F")
                print(30*"-")
            elif (a1 < a5):
                print(30*"-")
                print("Pasara por el punto       = F")
                print(30*"-")
                print("Terminara por el punto J")
                print(30*"-")
        elif (a6 < a3 )and(a6 < a4):
            print(30*"-")
            print("Terminara por el punto    = =  J")
            print(30*"-")
            if (a5 < a2 ):
                print(30*"-")
                print("Pasara por el punto       = B")
                print(30*"-")
                print("Terminara por el punto    = F")
                print(30*"-")
            elif (a2 < a5 ):
                print(30*"-")
                print("Pasara por el punto       = F")
                print(30*"-")
                print("Terminara por el punto    = B")
                print(30*"-")
</pre>

# Inicio por "B"

<p>Si el usuario decide iniciar por el punto "B" se ejecutara el siguinete código que compobara cada una de las rutas eligiendo la mas corta de punto a punto</p>
<pre>
    if inicio == 'B':
        print(30*"-")
        print("Iniciara por el punto     = B")
        print(30*"-")
        if (a1 <= a4 )and(a1<=a5):
            print(30*"-")
            print("Luego pasara por el punto =  F")
            print(30*"-")
            if (a2 <= a3):
                print(30*"-")
                print("Pasara por el punto       = J")
                print(30*"-")
                print("Terminara por el punto    = A")
                print(30*"-")
            elif (a3 < a2):
                print(30*"-")
                print("Pasara por el punto       = A")
                print(30*"-")
                print("Terminara por el punto    = J")
                print(30*"-")
        elif (a4 < a3 )and(a4 < a6):
            print(30*"-")
            print("Luego pasara por el punto = A")
            print(30*"-")
            if (a3 < a6):
                print(30*"-")
                print("Pasara por el punto       = F")
                print(30*"-")
                print("Terminara por el punto    = J")
                print(30*"-")
            elif (a6 < a3 ):
                print(30*"-")
                print("Pasara por el punto       = J")
                print(30*"-")
                print("Terminara por el punto    = F")
                print(30*"-")
        elif (a5 < a1 )and(a5 < a4):
            print(30*"-")
            print("Luego pasara por el punto =  J")
            print(30*"-")
            if (a2 < a6):
                print(30*"-")
                print("Pasara por el punto       = F")
                print(30*"-")
                print("Terminara por el punto    = A")
                print(30*"-")
            elif (a6 < a2 ):
                print(30*"-")
                print("Pasara por el punto       = A")
                print(30*"-")
                print("Terminara por el punto    =F")
                print(30*"-")
</pre>           

# Inicio por "A"

<p>Si el usuario decide iniciar por el punto "J" se ejecutara el siguinete código que compobara cada una de las rutas eligiendo la mas corta de punto a punto</p>

<pre>
    if inicio == 'J':
        print(30*"-")
        print("Iniciara por el punto     = J")
        print(30*"-")
        if (a2 <= a5 )and(a2<=a6):
            print(30*"-")
            print("Luego pasara por el punto = F")
            print(30*"-")
            if (a1 <= a3):
                print(30*"-")
                print("Pasara por el punto       = B")
                print(30*"-")
                print("Terminara por el punto    = A")
                print(30*"-")
            elif (a3 < a1 ):
                print(30*"-")
                print("Pasara por el punto       = A")
                print(30*"-")
                print("Terminara por el punto    = B")
                print(30*"-")
        elif (a5 < a2 )and(a5 < a6):
            print(30*"-")
            print("Luego pasara por el punto = B")
            print(30*"-")
            if (a1 < a4):
                print(30*"-")
                print("Pasara por el punto       = F")
                print(30*"-")
                print("Terminara por el punto    = A")
                print(30*"-")
            elif (a4 < a1 ):
                print(30*"-")
                print("Pasara por el punto       = A")
                print(30*"-")
                print("Terminara por el punto    = F")
                print(30*"-")
        elif (a6 < a2 )and(a6 < a5):
            print(30*"-")
            print("Luego pasara por el punto = A")
            print(30*"-")
            if (a3 < a4 ):
                print(30*"-")
                print("Pasara por el punto       = F")
                print(30*"-")
                print("Terminara por el punto    = B")
                print(30*"-")
            elif (a4 < a3 ):
                print(30*"-")
                print("Pasara por el punto       = B")
                print(30*"-")
                print("Terminara por el punto    = F")
                print(30*"-")
</pre>

# Hacemos el llamado a la funcion para ejecutarlo
<pre>
inicio()
</pre>

# Menú

<p>Por ultimo colocaremos un menú donde se dará opción al usuario si quiere o no seguir usando el algoritmo</p>

<pre>
def menu():
    S = input("Desea segir usando el programa S / N ")
    S =S.upper()
    if S =='S':
        print(129*"=")
        print(60*"=","RESTART",60*'=')
        print(129*"=")
        inicio()
    elif S == "N":
        print(50*'=')
        print(10*'-',"Fin del programa",10*'-')
        print(50*'=')
        exit(1)
    else:
        print("El valor ingresado no exisiste por favor vuelva a intentarlo ")
    menu()
menu()
</pre>


