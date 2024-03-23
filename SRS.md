---
layout: default
---
[Back](./)

# Software Requirements Specifications

## 1.0 Introduction 

The Software Requirements Specification document is broken up into different sections that will highlight the overall design and importance of our Mileage/Location Tracking application. In this section, the introduction, it details the purpose and goals of the application, as well as the possible assumptions or factors that could affect its development. It also lists important acronyms and their definitions that could be found throughout the document. In the second section, design constraints, it explains possible limitations or restrictions that the application may possess during the development process. In the third and fourth section, functional requirements and non-functional requirements, describes certain features and functionalities that should be present within the application. The fifth section, the external interface requirements, provides information to ensure that the system will communicate properly with users and with external hardware or software elements. 

### 1.1 Overview 

All businesses require records of their mileage and time spent any time they travel to an offsite location. With our Mileage/Location Tracking mobile app, any employee can track the miles they travel for business record purposes.  

Our app will allow the user to have their starting and ending location tracked as well as the distance they travel. To determine those factors, we will utilize Google Maps APIs. Thus, they will be able to accurately record their mileage as well as time spent traveling. Additionally, the app will create easily digested weekly reports on total miles traveled and total time spent within that week. We conclude that this mobile app will be used by small business employees and owners for the sake of keeping records regarding mileage. 

Mobile app Mileage/Location Tracking app development using React Native, JavaScript and Firebase. 

React Native is an open-source UI software framework created by Meta Platforms, Inc. It allows the development of iOS/Android apps and uses JavaScript as the programming language. React Native also allows the UI of the IOS and Android apps to be platform specific allowing for a native feel to the app on each platform. JavaScript is an Open-Source, client-side programming language. It is easy to learn, stable, and creates high-performance applications. Firebase is a set of backend cloud computing services and application development platforms provided by Google. It hosts databases, services, authentication, and integration for a variety of applications, including Android, iOS, and JavaScript. 

### 1.2 Project Goals 

* Integrate Google Maps APIs that tracks starting and ending locations, miles traveled, and time spent while traveling 
* Design a functional, user friendly, and readable user interface 
* Design a database using Firebase 
* Design a method to monetize the application through an advertisement system 

### 1.3 Definitions and Acronyms 

| Acronym      | Definition            
|:-------------|:-----
|API| Application Programming Interface     
|GPS| Global Positioning System   
|IOS| iPhone Operating System 
|UI| User Interface

### 1.4 Assumptions 

Using Google Maps APIs or other third-party components may cause issues pinpointing accurate locations and calculations 

Using React Native allows different features for different platforms. When developing, certain features may cause issues on one platform and not the other 

Internet connectivity may cause GPS tracking to stop altogether if the user is offline. Thus, calculating and receiving traveling data may be incorrect. Another issue is, internet connection is needed to upload and download information to the database, without proper connection that information could be lost or incorrect. 

## 2.0 Design Constraints 

While our project will not have many design constraints, certain limitations should be considered.  The first is react native. React native will allow us to code an app for both iPhone and Android with one framework.  This is possible due to react native having components that take advantage of the corresponding native features found on the Apple platform and the Android platform (which is why it is called react native).  However, when developing, there may be certain features that are exclusive to one platform that are not on the other platform.  If an issue like this comes up during development, we must keep in mind possible alternative methods of implementation that can work on both platforms. 

Another possible limitation is internet connectivity.  While geolocation should be possible using the built in GPS chip of the phone, an internet connection is still needed for the app to upload and download information to the database.  This may be an issue if the driver is in a location with a bad cellular connection.  While this is not ideal, there are several solutions to take on this problem such as having the driver's app only upload information to the database while in a place with a good cellular or Wi-Fi connection. 

## 3.0 Functional Requirements 

* Login and Password 
* Authentication 

### 3.1 Track Start and End of Trip 
The app should be able to detect when a trip begins and when a trip ends. This is necessary for the calculation of mileage and time spent on any given trip. The app will use Google Maps API to determine this based on speed traveled. 
High Priority 

### 3.2 Weekly Reports 
The app will report your total miles traveled and total time spent on a weekly basis. This information will be stored in a database for the sake of the business’ security and safekeeping as well as to revisit data as needed. 
High Priority 

### 3.3 Trip Continuity when Offline 
The app should be able to understand that a driver may lose internet connection while driving so the trip should still be tracked even when offline. The app will use the Google Maps API and recognize that a driver is still moving or has moved at high speed between two points when already driving. 
High Priority 

### 3.4 Home Page Navigates to In Progress Week and Day Report 
The app will have pages that will have the current days and week’s report in progress and be navigable by the user from the homepage.  
Medium Priority 

## 4.0 Non-Functional Requirements 

### 4.1 Security 

Security is a paramount non-functional requirement for the app. The system will implement robust measures to safeguard user data, ensuring confidentiality, integrity, and availability. User authentication and authorization will be handled securely, with Firebase Authentication used to manage user access. Additionally, data transmission between the mobile app and Firebase will be encrypted by Firebase to prevent unauthorized access. Access controls will be implemented at both the user and administrator levels, ensuring that only authorized personnel can access sensitive information and reports. 

### 4.2 Capacity 

Capacity requirements are crucial to ensure the app can handle a scalable number of users and data. The backend infrastructure, powered by Firebase, will be capable of scaling dynamically to accommodate an increasing number of users and their respective data entries. The app will be designed to handle potential peaks in user activity, particularly during periods of heavy usage. Firebase Cloud Functions are optimized for efficient execution, and the database will be able to handle a growing volume of location and mileage data. Regular performance testing will be conducted to identify and address any bottlenecks in the system, ensuring optimal performance under various usage scenarios. 

### 4.3 Usability 

The React Native-based frontend will adhere to design principles that prioritize user-friendly navigation, clear layouts, and easy data input. The app will feature responsive design elements to cater to various device sizes and orientations. User interfaces for tracking data and report generation should be straightforward and well-documented. Usability testing will be conducted to gather feedback and iteratively improve the app's overall usability. 

### 4.4 Other 

The app will prioritize maintainability, ensuring that code is well-documented, modular, and follows good coding standards. Regular backups of user data will be performed to prevent data loss. The app will have offline capabilities for data to save to the device, allowing users data to be saved even when there is no internet connection, with automatic synchronization once connectivity is restored. Load balancing mechanisms should be implemented to distribute traffic evenly across server resources. Regular monitoring and logging should be in place to track system performance, identify issues, and enable proactive maintenance. 

## 5.0 External Interface Requirements 

### 5.1 Hardware Interface Requirements 

Regarding hardware requirements, users must have a standard issue Apple iOS or Android OS capable phone. User’s devices must have wireless internet capability, either via SIM cards providing cellular connectivity or via WiFi. User’s devices must also have built in GPS and Gyroscopic capabilities (this is generally in built into a majority of consumer smartphones and tablets) 

### 5.2 Software Interface Requirements 

It is recommended that user’s devices have up-to-date firmware and software images on devices using this app. With the ever-changing nature of technology, we ask that  

[back](./)