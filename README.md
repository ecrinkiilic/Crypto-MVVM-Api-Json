# Crypto MVVM API & JSON

A simple cryptocurrency listing application built with **Swift** using the **MVVM (Model-View-ViewModel)** architecture. The app fetches cryptocurrency data from a REST API, parses JSON responses, and displays the information in a clean and maintainable structure.

## Features

* Fetch cryptocurrency data from an API
* Parse JSON responses using `Decodable`
* MVVM architecture implementation
* Display cryptocurrency names and prices
* Clean and scalable project structure

## Technologies Used

* Swift
* UIKit
* MVVM Architecture
* URLSession
* JSONDecoder



  ## Screenshot

<p align="center">
  <img src="https://github.com/user-attachments/assets/9289c29b-b8ee-4a10-9147-8da852319638" width="300" alt="App Screenshot">
</p>


## Project Structure

```text
Crypto-MVVM-Api-Json
├── Model
│   └── CryptoCurrency.swift
├── Service
│   └── WebService.swift
├── View
├── ViewModel
│   └── CryptoViewModel.swift
└── Assets.xcassets
```

## Installation

1. Clone the repository:

```bash
git clone https://github.com/ecrinkiilic/Crypto-MVVM-Api-Json.git
```

2. Open the project in Xcode.

3. Build and run the application on a simulator or a physical device.

## MVVM Architecture

### Model

The `CryptoCurrency` model represents the data received from the API.

```swift
struct CryptoCurrency: Decodable {
    let currency: String
    let price: String
}
```

### Service

The `WebService` layer is responsible for making network requests and converting JSON data into Swift models.

### ViewModel

The `CryptoViewModel` prepares and manages the data that will be presented in the user interface.

### View

The View layer displays cryptocurrency information and interacts with the ViewModel without directly accessing the data source.

## Purpose

This project was created to practice:

* Consuming REST APIs in Swift
* JSON parsing with `Decodable`
* Implementing the MVVM design pattern
* Building clean and maintainable iOS applications

## Author

**Ecrin Kılıç**
