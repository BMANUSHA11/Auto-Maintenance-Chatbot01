# Auto-Maintenance-Chatbot01
chatbot
# 🚗 Auto Maintenance Chatbot (C++)

## 📘 Project Overview

The **Auto Maintenance Chatbot** is a C++-based intelligent console application that simulates a self-learning chatbot for automobile maintenance assistance.

It is designed to demonstrate strong **Object-Oriented Programming (OOP)** principles along with **file handling and dynamic learning capabilities**.

The chatbot can learn new responses from users and store them persistently, allowing it to improve over time.

---

## 🧠 Key Features

✅ **Self-Learning Chatbot**

* Learns new keyword–response pairs dynamically from user input

✅ **Persistent Memory System**

* Stores learned responses in a file (`MJ-details.txt`)
* Automatically loads saved data on startup

✅ **Object-Oriented Design**

* Implements:

  * Encapsulation
  * Inheritance
  * Polymorphism
  * Templates
  * Composition

✅ **Emergency Assistance**

* Provides roadside emergency contact support

✅ **Custom Greetings**

* Different chatbot classes override greeting behavior

---

## 🏗️ Class Architecture

### 🔹 `Response<T1, T2>` (Template Class)

* Stores keyword–response pairs
* Demonstrates **generic programming using templates**

---

### 🔹 `Chatbot` (Base Class)

Handles core chatbot functionality:

* File handling (load & save responses)
* Keyword matching
* Learning new responses

**Key Methods:**

* `respond()`
* `learn()`
* `loadResponses()`
* `saveResponseToFile()`
* `toLowerCase()`

---

### 🔹 `AutoMaintenanceChatbot` (Derived Class)

* Extends `Chatbot`
* Provides automobile-specific interactions
* Overrides greeting method

---

### 🔹 `EmergencyService` (Composition Class)

* Independent class for emergency contact handling
* Demonstrates **composition**

---

### 🔹 `WorkshopChatbot` (Advanced Derived Class)

* Inherits from `AutoMaintenanceChatbot`
* Integrates `EmergencyService`
* Handles both normal and emergency queries

---

## 🧩 How It Works

1. Loads saved responses from `MJ-details.txt`
2. Greets the user
3. Accepts user input
4. Matches input with known keywords

   * ✅ If found → returns response
   * ❌ If not → learns from user
5. Saves new responses for future use

**Commands:**

* `exit` / `bye` → End program
* `emergency` → Show emergency contact

---

## 💻 Example Interaction

```text
Hello! Welcome to the Auto Maintenance Workshop. I'm MJ's Bot.

You: hi  
Bot: I don't understand. Can you teach me a response?  

You: hi → Hello! How are you today?  
Bot: I've learned a new response!  

You: hi  
Bot: Hello! How are you today?  

You: emergency  
Bot: In case of roadside emergencies, contact support immediately.  

You: bye  
Bot: Goodbye! Have a great day!
```

---

## 🧰 Technologies Used

**Language:**

* C++

**Core Concepts:**

* Templates
* Inheritance
* Polymorphism
* Encapsulation
* Composition
* File Handling
* String Manipulation

---

## 🚀 Future Improvements

* Add Natural Language Processing (NLP) support
* Improve keyword matching using similarity algorithms
* Build GUI version (Qt / Web interface)
* Integrate real-time API for automobile services

---

## 📌 Author

**Anusha B M**

* AI/ML Enthusiast | Software Developer
* Passionate about building intelligent systems

---

