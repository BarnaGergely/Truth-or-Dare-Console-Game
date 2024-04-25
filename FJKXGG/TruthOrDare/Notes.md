# Documentation and Notes for the project

- The project is a simple CRUD application with a console user interface
- The user interface is designed to be easily replaceable with a REST API

## Project structure, architecture:

- The software architecture is a weird mixture of ports and adapters and layered
	- The UI and the Infrastructure is connected with ports and adapters
	- The main logic is in the UI's controller
	- Rest of the application is doing CRUD
- Not DDD based namespace and folder structure

## Exception handling method:

- Catch as low as possible the exceptions and throw custom exceptions with user friendly message to the upper layers
- Flow control based on the built in exceptions or custom exceptions if layer crossing is needed

## Used design principles:

- Single responsibility
- Interface segregation
- Open/closed
- Liskov substitution
- Dependency inversion
- Dependency injection
- Don't repeat yourself
- CQRS
- CQS
- Keep it stupid simple -> Obviously I'm Failed in this point X)
- Write access modifiers everywhere

## Used Design Patterns:

- Repository
- Controller
- Service (not needed so finnaly not used)
- Entity
- Ports and Adapters

## Future improvements:

- Result pattern
- Better Exception handling
- Logging
- Usage of reflections

## K�rd�seim:

- Access modifiers:
	- Hogy v�lasztja sz�t az assembly-ket a ford�t�? Egy m�sik projekt ugyan abban a solution-ben m�sik assembly?
	- ha egy internal oszt�ly implement�l egy internal interface-t, ami egy m�sik namespace-ben van, akkor az oszt�ly met�dusainak mi�rt kell public-nek lenni�k?
- Hiba kezel�s
	- Hogyan �rdemes megoldani a hiba kezel�st egy egyszer� adatb�zis lek�rdez�st v�grehajt� met�dusban?
	- Result pattern:
		- t�nylegesen elterjedt a gyakorlatban a Result Pattern?									
- Mennyire kell a Single Responsibility �s interface segregation elvet k�vetni? - Pl. CRUD m�veleteket sz�t kell bontani?
