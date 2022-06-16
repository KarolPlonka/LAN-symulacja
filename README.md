# LAN-symulacja
Przykładowy projekt lokalnej sieci komputerowej. Symulacja została stworzona przy użyciu oprgoramowania Cisco Packet Tracer 8.1.



## 1.Topologia sieci
<img align="left" src="images/image-000.png">
<br clear="all" />
<br/>
<br/>

## 2.Użyte technologie i rozwiązania:


### Routery centralne + RIPv2
<img align="left" src="images/image-001.png">
Routery komunikują się między sobą w ramach czterech sieci. Każde połączenia dwóch routerów to osobna sieć, do której należy jeden z interfejsów routera. W tym przypadku routery połączone są złączem Serial DTE.

<br/>
<br/>

We wszystkich routerach aktywna jest usługa RIPv2, która wyznacza ścieżkę pakietom przesyłanym pomiędzy różnymi sieciami, do poprawnego działania tej usługi należy w każdym routerze przypisać tej usłudze wszystkie podsieci, którym chcemy umożliwić komunikację, jak i sieci pośredniczące w komunikacji między nimi (podsieci, które stoją na drodze połączenia między którymiś z podsieci, które mają się komunikować).


<br clear="all" />
<br/>


### Pojedynczy VLAN
<img align="left" src="images/image-002.png">
Adresy IP komputerów ustawione są statycznie. Komputery połączone ze switchem oraz router należą do jednego VLANu, w ramach którego się komunikują. Gdy adres docelowy pakietu jest adresem spoza sieci bramka sieciowa wskaże by wysłać go do routera, który następnie przekaże go dalej.
<br clear="all" />
<br/>


### Serwer DHCP
<img align="left" src="images/image-003.png">
Dany przykład podobnie jak powyższy z tą różnicą że do switcha podłączony jest serwer DHCP. Serwer DHCP posiada statyczne IP i przypisuje adresy urządzeniom w sieci, adresy pula adresów wyklucza 10 pierwszych adresy, które może użyć na podłączenie ewentualnych urządzeń preferujących statyczny adres IP.
<br clear="all" />
<br/>


### Access Point
<img align="left" src="images/image-004.png">
Do switcha został podłączony Access Point, który pozwala na przyłączenie do sieci urządzeń za pomocą technologii bezprzewodowej (w tym przypadku WIFI). Urządzenia połączone bezprzewodowo również uzyskują adresy z obecnego w sieci serwera DHCP. 
<br clear="all" />
<br/>



### Serwer HTTP
<img align="left" src="images/image-004.png">
Do switcha został podłączony serwer HTTP o statycznym adresie IP, hostowaną przez niego stronę internetową można przeglądać z każdego miejsca w sieci wpisując w wyszukiwarkę jego adres IP.
<br clear="all" />
<br/>


### Access Point
<img align="left" src="images/image-004.png">
Do switcha został podłączony serwer HTTP o statycznym adresie IP, hostowaną przez niego stronę internetową można przeglądać z każdego miejsca w sieci wpisując w wyszukiwarkę jego adres IP.
<br clear="all" />
<br/>

<sup><sub>Reszta elementów sieci nie opisanych w powyższych przykładach jest tożsama lub zawiera się w którymś z powyższych przykładów.</sub></sup>
<br/>

### SSH
<img align="left" src="images/image-004.png">
Do switcha został podłączony serwer HTTP o statycznym adresie IP, hostowaną przez niego stronę internetową można przeglądać z każdego miejsca w sieci wpisując w wyszukiwarkę jego adres IP.
<br clear="all" />
<br/>


### Access Point
<img align="left" src="images/image-004.png">
Do switcha został podłączony serwer HTTP o statycznym adresie IP, hostowaną przez niego stronę internetową można przeglądać z każdego miejsca w sieci wpisując w wyszukiwarkę jego adres IP.
<br clear="all" />
<br/>
