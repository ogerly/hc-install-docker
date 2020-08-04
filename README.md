# Der erste Start! The first start!


## Wir benötigen zum localen betreiben von Human Connection :: We need the following to run Human Connection  
Open source code: https://github.com/Human-Connection/Human-Connection

Dokumentation: https://docs.human-connection.org/human-connection/

- ## GIT                         

      $ sudo install git

- ## DOCKER               
       
      $ sudo install docker && sudo install docker-compose

### Hinweis für Windows Nutzer ( nutzt endlich Linux! ;) :: Note for Windows users ( finally uses Linux! ;)
!! Bei Rechnern mit Vorinstalliertem Windows: Stelle sicher, dass "Virtualization Technology" und "Execute Disable Bit" im BIOS aktiviert sind.!!
!! For computers with preinstalled Windows: Make sure that "Virtualization Technology" and "Execute Disable Bit" are activated in the BIOS.
___

# Schritt für Schritt ... :: Step by step ... 
VideoTutorial in german: https://www.youtube.com/watch?v=RxsAfKbObVI

## 1.  GIT Repositorie in einen Ordner deiner Wahl herunterladen. :: Download 1st GIT repository to a folder of your choice

        $  git clone https://github.com/Human-Connection/Human-Connection.git
 
## 2.  In den neu angelegten Ordner „Human Connection“ wechseln. :: switch to the newly created folder "Human Connection".

        $  cd Human Connection

## 3.   jetzt machen wir ein Build von Human Connection :: Now we're making a build of Human Connection
        
        $  docker-compose up --build

## 4.  dann setzen wir die Indizes in die neo4j Datenbank :: then we put the indexes into the neo4j database

        $  docker-compose exec neo4j db_setup

## 5.   jetzt füllen wir die Datenbank mit Testdaten :: now we fill the database with test data

        $ docker-compose exec backend yarn run db:seed



## 6. Diese vier seite sollten jetzt abrufbar sein. :: These four pages should be available now.

      http://localhost:3000
      http://localhost:4000
      http://localhost:7474  (Übersicht Neo4j Befehle https://github.com/ogerly/hc_neo4j_commands)
      http://localhost:1080


 ___
 
 # Der zweite Start! :: The second start!
 
## Das erneute starten von Human Connnection auf deinem Rechner: 
Das _docker-compose up --build_ ist nur bei einer einrichtung nötig. 
## Restarting Human Connection on your computer: 
The _docker-compose up --build_ is only necessary for one setup. 


Für das starten von Human Connection reicht dann folgender Ablauf. 
For starting Human Connection the following procedure is sufficient. 

 1.     $  cd Human Connection


 1.     $  docker-compose up
 
 
 
 1.     $  docker-compose exec backend yarn run db:seed
 
 1.     
            http://localhost:3000
            http://localhost:4000
            http://localhost:7474
            http://localhost:1080

 
  ___
 
 
 
 ## Programme ;) 
  ![img1](https://user-images.githubusercontent.com/1324583/64679177-74f83400-d47b-11e9-8f15-8477a3f82ee6.png)


 ___
 
 

## Alles Weitere findet ihr bei GitHub @Human-Connection :: Everything else you can find at GitHub @Human-Connection
https://github.com/Human-Connection/Human-Connection


## Die Dokumentation :: The documentation:
https://docs.human-connection.org/human-connection/


## Zum Discord Channel von "Human Connection":
https://human-connection.org/discord/
Hier könnt ihr fragen stellen und mit den Entwicklern reden. 



## Zum Projekt "Human Connection":
https://human-connection.org/
