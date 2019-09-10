# Der erste Start!

## Wir benötigen zum Localen betreiben von Human Connection  
https://github.com/Human-Connection/Human-Connection

- ### GIT                         

      $ sudo install git

- ### YARN                     

      $ sudo install yarn
      
- ### DOCKER               
       
      $ sudo install docker && sudo install docker-compose



___

# Schritt für Schritt ... 


## 1.  GIT Repositorie in einen Ordner deiner Wahl herunterladen.

        $  git clone https://github.com/Human-Connection/Human-Connection.git
 
## 2.  In den neu angelegten Ordner „Human Connection“ wechseln.

        $  cd Human Connection

## 3.   Jetzt machen wir ein Build von Human Connection
        
        $  docker-compose up --build

## 4.  dann setzen wir die Indizes in die neo4j Datenbank

        $  docker-compose exec neo4j db_setup

## 5.   jetzt füllen wir die Datenbank mit Testdaten

        $ docker-compose exec backend yarn run db:seed





      http://localhost:3000
      http://localhost:4000
      http://localhost:7474
      http://localhost:1080


 
## Alles Weitere findet ihr bei @Human-Connection
https://github.com/Human-Connection/Human-Connection

https://docs.human-connection.org/human-connection/

https://human-connection.org/
