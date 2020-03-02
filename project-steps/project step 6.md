###### Josue Fuentes
*march 1st 2020*

***
## Use Case: weight loss
###### **Actors**
customer

###### **Trigger**
customer desires to lose weight

###### **Precondition**
customer must eat

###### **Postcondition**
customer must log food in app

---
###### **Normal Flow**
1. the user will create an account
2. the user will create a profile with their weight, age and height
2. the user will input their body mass index
3. the system will calculate the proper amount of calories needed to perform an action
4. the user will choose whether to lose, increase or maintain weight
5. the system will choose a workout routine based on the user's choice
6. the user will log information in the system until goal is reached

---
###### **Alternate Flow**
1. the user chooses to decrease weight
  * the system will calculate the calories needed a day to lose weight
  * the system will tailor the workout routine and diet around losing weight
2. the user chooses to increase weight
  * the system will calculate the calories needed a day to increase weight
  * the system will tailor the workout routine and diet around increasing weight
3. the user chooses to maintain weight
  * the system will calculate the calories needed to maintain current body weight
  * the system will tailor the workout routine and diet around maintaining current weight
