---
layout: default
---

# Software Design Document

## 1.0 Introduction 

The Software Design Document (SDD) is a crucial component in the software development lifecycle that helps guide the implementation process. The Software Design Document for the Mileage/Location Tracking application serves as a comprehensive guide outlining the functional and non-functional requirements, design considerations, architecture, and the implementation details of the software system being developed. The purpose of this document is to provide a clear understanding of the design principles, components and architecture within the system. The SDS describes design goals, considerations, and development methods, provides an overview of the architectural strategies as well as the systems architectures, and describes high-level detail about the systems design.  

### 1.1 Document Outline 
Here is the outline of the Software Design Document, listing each section and their respective subsections. 

- Introduction 
    - Document Description 
        - Introduction 
            - Purpose 
            - Scope: Project Goals  
            - Definitions 
        - System Overview 
            - Functionality and Design 
- Design Considerations 
    - Assumptions and Dependencies & General Constraints 
        - Assumptions and Dependencies 
        - General Constraints 
    -  Goals and Guidelines & Development Methods  
        - KISS Principles 
        - Agile Method 
        - Priority on Intuitive Records 
- Architectural Strategies 
    - Strategy – Agile Method 
- System Architecture 
    - Component – React Native 
    - Component – Firebase 
    - Component – Google Maps APIs 
- Detailed System Design 
    - Module - React Native 
    - Module - Firebase 
    - Module - Google Maps APIs 
- Bibliography  

### 1.2 Document Description 

The Software Design Document is broken up into different sections that will highlight the overall design and importance of our Mileage/Location Tracking application. In this section, the introduction, it details the purpose and scope of the document, as well as a lists important acronyms and their definitions that can be found throughout the document. In the second section, design considerations, it explains possible limitations or restrictions that the application may possess during the development process. In the third, the architectural strategies and system architecture, it details using the Agile method for our software development and the implementation of react native, firebase, and google maps APIs for our system architecture. The fourth section, detailed system designs, provides information on the primary components that will be used to implement our design. 

#### 1.2.1 Introduction 

##### 1.2.1.1 Purpose 

The purpose of the Software Design Document is to provide a clear understanding of the design principles, components and architecture within the system. This document acts as a guide for the reader to easily follow and understand the design of our application. It provides a clear layout of how the system should be implemented and possible elements that should be kept in mind while developing the application, while ensuring consistency and coherence in the development process. The SDS also serves as a way of communication. Overall, this document ensures the successful development, implementation, and maintenance of the software systems by providing a detailed and structured overview of the systems design and requirements, as well as aligning everyone involved in the project. 

##### 1.2.1.2 Scope: Project Goals 

All businesses require records of their mileage and time spent any time they travel to an offsite location. With our Mileage/Location Tracking mobile app, any employee can track the miles they travel for business record purposes. Our app will allow the user to have their starting and ending location tracked as well as the distance they travel. To determine those factors, we will utilize Google Maps APIs. Thus, they will be able to accurately record their mileage and time spent traveling. Additionally, the app will create easily digested weekly reports on total miles traveled and total time spent within that week. We conclude that this mobile app will be used by small business employees and owners for the sake of keeping records regarding mileage. 

Project Goals: 

* Integrate Google Maps APIs that tracks starting and ending locations, miles traveled, and time spent while traveling 
* Design a functional, user friendly, and readable user interface 
* Design a database using Firebase 
* Design a method to monetize the application through an advertisement system	 

##### 1.2.1.3 Definitions 

| Acronym      | Definition            
|:-------------|:-----
|API| Application Programming Interface     
|GPS| Global Positioning System   
|KISS| Keep It Simple, Stupid
|OS| Operating System
|SQL| Structured Query Language
|UI| User Interface
|UX| User Experience

#### 1.2.2 System Overview 

##### 1.2.2.1 Functionality  

The app will allow the user to have their starting and ending location tracked as well as the distance they travel. To determine those factors, we will utilize Google Maps APIs. Thus, they will be able to accurately record their mileage and time spent traveling. It will also account for general constraints such as, lack of wireless network connection, potential authentication requirements, data protection and privacy, and local storage capabilities. Additionally, the app will create easily digested weekly reports on total miles traveled and total time spent within that week. 

#### 1.2.2.2 Design 

During the development process, we will follow the KISS principle to create a simple and interactive user interface that is user friendly, readable and easy to navigate. The architectural strategy that will be employed is the Agile method. As for the system architecture, the three main components that will be implemented to develop the software are React Native, Firebase, and Google Maps APIs. 

## 2 Design Considerations 

This section describes many of the issues which need to be addressed or resolved before attempting to devise a complete design solution. 

### 2.1 Assumptions, Dependencies & General Constraints 

#### 2.1.1 Assumptions and Dependencies 

There are multiple dependencies that are required for this software to work, including: 

* Android OS 13 or Later 
* iOS 16 or Later 
* GPS Compatible Device. 
* Wireless Network Capable Device. 
With these dependencies, this provides us with the very essentials for our software to perform its basic functions. 

#### 2.1.2 General Constraints 

General constraints for this software mainly involve the user’s device, and the constraints that arise therein. Our general constraints are as follows: 

* Lack of a Wireless Network Connection. 
* Potential Authentication Requirements based on Customer Needs. 
* General Standards of Data Protection and Privacy, as we will be tracking users' location data. 
* Local Storage Capability and Availability before Storing Data to Cloud. 

### 2.0 Goals and Guidelines & Development Methods 

#### 2.2.1 KISS principle 

Our app will strive to create a simple and interactive UI that is intuitive and easy to navigate. Small business owners are, typically, busy people without the time to train themselves in fields that are not related to their business. Therefore, we want small business owners to have the ability to use our app without the need for training or any specialty in technology.	 

#### 2.2.2 Agile Method 

During our development process, we will be using the agile method. More particularly, we will be using the aspect of the process that allows for frequent deliveries as well as change being available throughout the entire process. 

#### 2.2.3 Priority on Intuitive Records 

Our app will prioritize clear and concise records that will be stored in the database. This is so that there will not be much time searching through records when retrieving them. This is important to us due to our main audience being small business owners, thus our priority is to cater to the audience who has less time to search through their records. 	 

## 3.0 Architectural Strategies & System Architecture 

### 3.1 Architectural Strategies 

While there are many strategies for designing software in a team environment such as the waterfall and spiral methods, our team has decided to employ the Agile method of software development.  We have chosen this method for two main reasons.  The first is that Agile usually is mainly focused on smaller teams and shorter development times (Agile Manifesto).  The second is that agile is commonly used throughout the entire industry (Agile Manifesto).  This means that any experience using this method for our project should give us insight and experience for real-world development lifecycles. 

### 3.2 System Architecture 

There are three main components that we will be using for our system architecture.  The first is React Native.  React Native will give us the tools to create a UI for our app that will work on both the iPhone and android platforms.  The second of these components is Firebase.  Firebase is a no SQL database that will allow us to store app information on the cloud.  This will be useful for storing reports for the admin to see and storing the driver's locations.  Lastly, there is the Google Maps API.  This will allow us to use some of the features of Google Maps in our app such as geolocation.  By using these features, we can track the location of the drivers to get a better idea of how far they have traveled for gas milage calculations.   

## 4.0 Detailed System Design 

### 4.1 React Native 
    React Native will serve as the primary user interface component for our mobile app. Specifically designed to create a consistent and intuitive user experience, React Native components will be organized to fulfill requirements outlined in the specifications. The primary responsibility of these components is to render various screens, capture user input, and facilitate smooth navigation within the app. Assumptions include adherence to the specified design guidelines and constraints on UI/UX. Subcomponents will encompass individual screens, navigation elements, and UI elements like buttons and forms. Collaborations involve interaction with Firebase for data retrieval and storage and interaction with Google Maps API for presenting map views. React Native manages resources such as memory for rendering UI components and interacts with device APIs for basic native functionalities. 

### 4.2 Firebase 

    Firebase will play a crucial role in managing the backend data storage and authentication processes of the app. The primary responsibility includes real-time data synchronization, user authentication, and cloud functions for server-side logic execution. Assumptions involve secure data transmission and adherence to Firebase's data structure constraints. Subcomponents encompass Firestore for data storage, Firebase Authentication for user management, and Cloud Functions for server-side logic. Collaborations include interactions with React Native for data presentation, data storage, and user authentication. Firebase manages resources such as server space for data storage and processing power for cloud functions. 

### 4.3Google API 

    Google Maps API will be integrated to handle mapping and geolocation functionalities within the app. The primary responsibility includes rendering maps, tracking locations, and providing accurate mileage data. Assumptions involve reliable internet connectivity for map rendering. Subcomponents include map rendering, geocoding, and reverse geocoding elements. Collaborations encompass interactions with React Native for presenting map views and Firebase for storing location data. Google Maps API manages resources like map tiles, geolocation services, and rendering capabilities. The API uses algorithms for efficient map rendering, geocoding, and reverse geocoding, with considerations for handling exceptional conditions like invalid coordinates. 

## Bibliography 
The Four Values of the Agile Manifesto 
https://www.productboard.com/glossary/agile-values/ 

[back](./)
