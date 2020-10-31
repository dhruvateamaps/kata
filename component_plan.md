# This file contains the various components and their responsibilities

## Component
### User Interface

#### Responsibilities
Provides interactive session to the users to communicate with Farmacy Foods  
Means for the user to find closest fridges  
Calculates closest fridge to user  
Functionality to key in information like health, goals, payment  
Communicates with Smart Fridge module to get active fridge locations  
Provides information on available food by interfacing with Inventory module  
Provides most appropriate meals by interfacing with the Diet Advisor module  
Options to order personalised food or select from Menu  
Handles payments by interfacing with Sales and Payments module  
Permit placing of future order by interfacing with inventory  
Handle refunds by interfacing with Sales and Payments  
Enable feedback capturing post customer consuming the meal through notifications  
Enables proxy pickup by providing a user code  


## Component
### Inventory

#### Responsibilities
Handles inventory tracking and enables replenishment of low stock by notifying Kitchen and Ops staff through Cheftec  
Handles inventory replenishment of stock older than 3 days by notifying Kitchen and Ops staff through Cheftec  
Uses notification service to communicate replenishement requirements for the fridge  
Uses Internal Smart Fridge component APIs to pull the information for inventory and captures in data store  


## Component
### Sales and payments  

#### Responsibilities
Handles payment received events  
Captures purchase activity across the network of fridges and Kiosks  
Interfaces with the Cheftec financial system for accounts  
Handles refund events  


## Component
### Diet Advisor  

#### Responsibilities
Provides diet plans based on health, goals and personal goals  


## Component
### Fridge Communicator  

#### Responsibilities
Communicates with the network of smart fridges to gather inventory and purchase data  
Enables adding new fridge details upon fridge installation  
Enables notifying vendor for maintainence and lifecycle  


## Component
### Customer profile  

#### Responsibilities
Creates new user profile  
Collects and stores PHI information  
Collects and stores Personal health goals  
Collects and Stores payment information securely  
Creates temp user profile for walk-in customers  
Integrates with identity providers like Facebook, Gmail etc  
Integrate with lifestyle devioces like smartwatches to consume health information  


##  Component
### Loyalty program  

#### Responsibilities
Creates special offers for existing customers based on usage  


## Component
### Notifications  

#### Responsibilities
Handles end-to-end notifications for all external entities (SMS, Push, Email)  


## Component
### Monitoring and logging  

#### Responsibilities
Enables monitoring across the application based on generated events  
Generates IT events for all the components, modules and infrastructure and stores locally  
Handles log rotation based on configuration  
Pushes logs to external syslog servers  
Uses notification service to push critical system events to admins  
