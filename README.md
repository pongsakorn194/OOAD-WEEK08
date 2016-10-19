# OOAD-WEEK08

## Use Case Diagram 

###Usecase Diagram 1


Code
```
@startuml

User -> (Withdraw Cash)
User -> (Check Balance)
User -> (Transfer)
User -> (Make Donation)

@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK08/blob/master/Homework/usecase%20diagram01.png?raw=true">


###Usecase Diagram 2

Code
```
@startuml
skinparam handwritten true

skinparam usecase {
	BackgroundColor yellow
	BorderColor DarkSlateGray

	ArrowColor Olive
	ActorBorderColor black
	ActorFontName Courier

	ActorBackgroundColor<< Human >> Gold
}
(log on) as (Use) 

teacher -> (maintain question)
teacher --> (Use)
teacher -> (maintain user)
teacher -> (difficulty)

child --> (Use)
child --> (game)

@enduml

```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK08/blob/master/Homework/usecase%20diagram02.png?raw=true">


###Usecase Diagram 3

Code
```
@startuml
left to right direction
skinparam packageStyle rect
actor representative
actor passenger
rectangle service {
  representative -- (checkin)
  (checkin) -- passenger
  passenger -- (automatedcheckin)
  passenger -- (expresscheckin)
  passenger -- (boarding)
}
@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK08/blob/master/Homework/usecase%20diagram03.png?raw=true">


###Usecase Diagram 4

Code
```
@startuml
left to right direction
skinparam packageStyle rect
actor tradingmanager
actor trader
actor salesperson
actor accountingsystem
rectangle tradingsystem {
  tradingmanager -- (setlimit)
  trader -- (analyzerisk)
  trader -- (capturedeal)
  trader -- (pricedeal)
  salesperson -- (capturedeal) 
  salesperson -- (pricedeal)
  accountingsystem -- (updateaccounts)
  
  (analyzerisk) .> (valuedeal) : include
  (pricedeal) .> (valuedeal) : include
}
@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK08/blob/master/Homework/usecase%20diagram04.png?raw=true">


###Usecase Diagram 5

Code
```
@startuml
left to right direction
skinparam packageStyle rect

actor customer
actor clerk
actor salesperson
actor manager

rectangle telephoneorder {

  customer -- (checkstatus)
  customer -- (priceorder)
  customer -- (buildcredit)
  clerk -- (fillorder)
  salesperson -- (checkstatus) 
  salesperson -- (priceorder)
  manager-- (buildcredit) 
}
@enduml
```
Diagram
<img src="https://github.com/pongsakorn194/OOAD-WEEK08/blob/master/Homework/usecase%20diagram05.png?raw=true">

