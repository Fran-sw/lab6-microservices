In the following is shown how the diferent objectives of the 6th laboratory have been completed:
* The two microservices are running and registered (two terminals, logs screenshots).
    * Accounts - port 2222 **gradle :accounts:bootRun**
    ![accounts log](accounts.png)
    * Web - port 3333 **gradle :web:bootRun**
    ![web log](web.png)

------------------------------
para ver como y donde arranca todo -> fichero aplication 
para arrancar -> gradle :web:bootRun    (puerto 3333)
                 servidor eureka -> gradle :registration:bootRun (puerto 1111)
                 account service -> gradle :accounts:bootRun    (puerto 2222)

¿Que pasa si tiramos una maquina de backend, y la abrimos en otra terminal?
- La nueva instancia se registrara en eureka
- Se lo comunicara al front end para que cambie a quien se dirije