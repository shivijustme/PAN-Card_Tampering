# PAN-Card-Tampering-Detection #

UCS757 - Building Innovative Systems
Project - 1
Name - Shivansh Kumar
Roll No. - 101803103
PAN Card Tampering Detection

## Overview: ##
The purpose of this project is to detect tampering of PAN card using computer vision. This project will help different organization in detecting whether the Id i.e. the PAN card provided to them by thier employees or customers or anyone is original or not.

### Novelty: <br/>
●	The application will have two types of users - Admin Users and Customer Users.<br/>
●	Both these user types will be child classes of User class and inherit properties such as Id, UserName, Password, UserType. The difference between the two users will be that Customers Users will also have additional properties - Name, Address, Phone, hasRented. hasRented will be False when the account is created and it will be set to True once a customer user rents a vehicle.<br/>
●	Customer Users will only be able to View Data but Admin Users will be able to Add/Edit/Delete/View all data.<br/>
Vehicles:<br/>
●	The parent Vehicle Class will have properties such as -  Id, Brand, Model, Year, Color, Type, Base Cost, Mileage and isRented.<br/>
●	isRented property will be set to False by default and will only switch to True if that specific vehicle is currently Rented by a user.<br/>
●	Mileage is not a required property. Admin may or may not provide a value for this. All other properties are required. The Admin should not be able to Add a vehicle if any of the required properties are not specified.<br/>
●	The Child Classes will be - Sedan, SUV, Coupe. These will inherit all properties of Vehicle Class but the Base Cost will be different. Base cost will be in addition to the base cost entered by the Admin when creating the object. Additional base cost for Sedan = 50, Coupe = 75, SUV = 100.<br/>
Rental/RentalAgreement:<br/>
●	This object/class will store the information about which vehicle was rented to which user, at what date/time and for how much.<br/>
●	Properties will include - RentalId, RentalDateTime, RentalPrice, VehicleId, UserId, isActive. isActive will be set to True when a vehicle is rented and set to False when the rental is returned (will work on this part later, if time permits)<br/>

