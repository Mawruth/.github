# AR for Museum Guide (Mawruth Application) ​

![image](https://github.com/mwrooth/.github/assets/105928025/9de9ea61-8da7-4020-aecf-3956e325ea7b)

**Mawruth is a mobile app specified in the tourism field and museums, it uses Augmented Reality to create outstanding visual solutions and experiments for tourists during their visits**

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [AI Feature](#ai-feature)
- [Tools](#tools)
- [Android Architecture](#android-architecture)
- [Backend](#backend)
- [Future features and updates](#future-features-and-updates)
- [Team members](#team-members)



## Introduction
Museums have traditionally used static displays and guided tours to showcase cultural heritage, but these methods offer limited interactivity and contextual information. With AI and AR technologies, museums can now create more engaging and immersive experiences. This project aims to enhance museum visits by integrating AI for object identification and AR for real-time display, along with virtual tours for remote exploration. The motivation is to offer a more interactive and informative experience compared to traditional methods. Visitors often struggle to choose destinations and make the most of their visits without guides, and traditional museums lack interactive visual experiences. While offering such experiences at home is desirable, the high cost of necessary hologram technology makes it prohibitive for both museums and visitors.


## Features
- User Management
  - User Registration: Sign up with a valid email and password, with email verification.
  - User Login: Secure login for registered users.
  - User Profile: Update personal information.
  - Password Reset: Reset password via email link.
  - Profile Editing: Edit profile information including name, password, and photo.

- Museum Information
  - View All Museums: List of all available museums.
  - Search Museums: Search by name, category, or location.
  - Museum Details: Detailed information about each museum, including description, sections, and available pieces.
  - Museum Categories: List of museum categories for easy navigation.

- Additional User Features
  - Piece Listings: View and filter museum pieces by category, name, or popularity.
  - Access AR Content: Access AR content like 3D models, animations, or audio guides by scanning pieces.
  - Rate and Review: Review museum pieces and museums, and share feedback with other users.
  - Virtual Tours: Integrated with the Islamic Museum site to provide a VR-like tour inside the museum.
 

## AR Feature


## AI Feature

Integrated AI interfaces to provide an image classification model. Built with Python, FastAPI, Tensorflow

## Tools

### Backend 
  - TypeScript
  - Node.Js
  - Nest.Js
  - PostgreSQL
  - Prisma
  - Docker
  - Azure for cloud

### Android 
  - Kotlin
  - XML
  - Unity Vuforia Activities
  - ARCore

### Frontend (Dashboard)
  - HTML
  - CSS
  - TypeScript
  - React.Js

## Android Architecture

### Architectural Patterns
  -  MVVM (Model-View-ViewModel):
      -  Model: Data layer, including repository and data sources.
      - View: UI layer, displaying data and handling user interactions.
      - ViewModel: Bridge between View and Model, managing UI-related data and logic.
  
  - Clean Architecture:
      - Presentation Layer: UI components and ViewModels.
      - Domain Layer: Business logic and use cases, independent of other layers.
      - Data Layer: Manages data sources and includes the repository.

  - Repository Pattern
      - Purpose: Abstracts data sources, providing a clean API for data access.
      - Implementation: Acts as a single source of truth, coordinating between domain layer and data sources.

  - Importance of Concurrency
      - Performance: Keeps the app responsive during intensive tasks like AR rendering and data fetching.
      - User Experience: Maintains smooth UI operations by handling background tasks without blocking the main thread. 

  - Concurrency Mechanisms in Kotlin
      - Coroutines: The main concurrency tool in Kotlin for writing asynchronous code in a sequential style.

  - Key Techniques
      - Coroutines Launch: For tasks that don't return a result.
      - Async: For tasks that return results and can run in parallel.
      - Dispatchers: Control thread execution (Main for UI, IO for network/disk).
      - Structured Concurrency Manages coroutines to prevent memory leaks and ensure proper task cancellation.
      - Coroutine Scope: Defines the lifecycle of coroutines, like viewModelScope in MVVM.
      - Suspending Functions Functions with suspend keyword for long-running operations without blocking threads.
   
  - Example Use Cases Data
      - Fetching Use Dispatchers.IO for network requests.
      - Perform parallel operations with async.
      - Database Operations Use Dispatchers.IO for read/write tasks.
      - AR Processing Handle AR tasks in background threads for a responsive UI.


  ### Key Features
  **ARCore**: developed by Google, is a robust augmented reality (AR) platform for Android applications. It enables developers to integrate immersive AR experiences into their apps using various features and tools.

  **OpenGL**: ARCore uses OpenGL for rendering graphics, leveraging its capabilities to process and display 3D models efficiently.
  
  **Sceneform (Deprecated in 2021)**: Previously, Sceneform served as a high-level framework built on top of OpenGL, simplifying the rendering of 3D models in ARCore applications. However, it was deprecated in 2021.
  
  **TensorFlow**: Use TensorFlow to recognize museum pieces and retrieve relevant data, Enhances the app’s ability to provide detailed information and interactive experiences
  
  **Vuforia engine**: Vuforia is an AR platform that enables the creation of immersive AR experiences by recognizing images, objects, and environments.
  
  **Deep Link Functionality**: Deep linking allows users to navigate directly to specific app content from external sources like other apps, emails, or web pages.
  
  

## Backend

### Database Schema

![IMG-20240625-WA0009](https://github.com/mwrooth/.github/assets/105928025/19f6760e-defe-44e9-ab2f-9c2b4839d519)



## Future features and updates
- Enhance performance
- Add more data and museums
- Add more functions to the admin dashboard
- Apply multi-tenancy architecture 

## Team members

Meet the amazing team behind this project:

| ![Ahmed Mabrouk](https://github.com/AhmedMabrouk22.png?size=100) | ![Abdullah Aly](https://github.com/PandaX185.png?size=100) | ![Mohamed Elsharaky](https://github.com/Elsharaky.png?size=100) |
|:--:|:--:|:--:|
| [**Ahmed Mabrouk**](https://github.com/AhmedMabrouk22) | [**Abdullah Aly**](https://github.com/PandaX185) | [**Mohamed Elsharaky**](https://github.com/Elsharaky) |
| Backend Developer | Backend Developer | Backend Developer |

| ![MohamedElattar22](https://github.com/MohamedElattar22.png?size=100) | ![Abdelrahman Mohamed](https://github.com/abdelrahmanz3z3.png?size=100) | ![Asem Hisham](https://github.com/asemhisham20.png?size=100) |
|:--:|:--:|:--:|
| [**Mohamed Elattar**](https://github.com/MohamedElattar22) | [**Abdelrahman Mohamed**](https://github.com/abdelrahmanz3z3) | [**Asem Hisham**](https://github.com/asemhisham20) |
| Android Developer | Android Developer | Android Developer |
