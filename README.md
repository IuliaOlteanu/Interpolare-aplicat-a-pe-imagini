# Interpolare-aplicata-pe-imagini
Olteanu Iulia,314CC

  Pentru fiecare cerinta am urmat instructiunile din fiecare functie , dar si indicatiile din enuntul temei.Cea mai mare parte din tema a fost solutionata tinand cont de formulele si explicatiile regasite in descrierea acesteia.Pentru functiile in care se cere realizarea interpolarilor pe o imagine RGB, am urmat exclusiv indicatiile din scheletul de cod , am extras fiecare canal al imaginii(rosu,verde,albastru) si am apelat functia 
creata anterior,urmand la final a forma imaginea finala cu cele 3 canale de culori.Formulele din pdf au fost folosite modificand intr-o oarecare masura indicii.

**Interpolare nearest-neighbour**
\
➢ Pentru functiile nn_2x2 si nn_resize am determinat cel mai apropiat vecin cu functia predefinita round,care rotunjeste parametrul primit ca argument catre cel mai apropiat numar intreg,iar TO DO-urile au fost extrem de bine explicate pentru a putea rezolva task-urile cerute

**Interpolare biliniara**
\
➢ Am folosit functia surrounding_points pentru a determina cele 4 puncte ce contin (x,y) cu ajutorul functiei floor,care rotunjeste parametrul primit ca argument catre cel mai apropiat numar intreg mai mic sau egal cu parametrul.Am modificat putin formula din pdf referitoare la calculul coeficientilor a, deoarece a(3) si a(4) sunt inversate.Functiile de rotate si resize sunt oarecum similare din punct de vedere al codului,iar in cazul functiei rotate am mai verificat daca un indice se afla in afara imaginii,punand 0 in acesta situatie

**Interpolare bicubica**
\
➢ Functia surrounding_points este identica cu cea de la interpolarea biliniara,calculul derivatelor a fost realizat tinand cont de formulele din pdf , cu mici modificari pentru fx si fy, schimband doar x cu y .Pentru calculul matricelor Ix,Iy,Ixy am observat din testele ref ca Ix are valori ale primei si ultimei coloane 0, Iy contine valori de 0 pe  prima si ultima linie, iar Ixy are prima si ultima linie 0 si prima si ultima coloana 0.Pentru coeficientii de interpolare bicubica am interschimbat x cu y din formula enuntata in pdf-ul temei.

