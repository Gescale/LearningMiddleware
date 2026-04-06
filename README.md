# Learning Middleware - ASP.NET Core 9

A practical repository exploring the ASP.NET Core middleware pipeline, built alongside the **ASP.NET Core [.NET 9] Deep-Dive** course by Frank Liu. 

This project demonstrates how HTTP requests and responses are handled, intercepted, and modified as they flow through the modern .NET application pipeline.

## 🚀 Overview

Middleware components are the core building blocks of an ASP.NET Core application's HTTP pipeline. This repository contains accurate, implementation-focused examples of configuring, creating, and ordering middleware to control application flow safely and efficiently.

### Key Concepts Explored
* **The Request Delegate Pipeline:** Understanding how the `HttpContext` passes through successive middleware components.
* **Terminal Middleware (`app.Run`):** Creating endpoints that return a response and prevent further pipeline execution.
* **Chaining Middleware (`app.Use`):** Intercepting requests, performing logic (such as logging or header manipulation), and calling `next()` to pass control down the chain.
* **Branching the Pipeline (`app.Map` & `app.MapWhen`):** Conditionally routing requests based on URL paths, query strings, or specific request headers.
* **Custom Middleware Classes:** Extracting inline anonymous functions into clean, reusable, and testable C# classes.
* **Short-circuiting:** Returning early from the pipeline (e.g., rejecting invalid or unauthorized requests before they hit the controllers).

## 🛠️ Tech Stack & Prerequisites
* **Framework:** [.NET 9.0 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)
* **IDE:** Visual Studio 2022 (v17.12+) or Visual Studio Code
* **Language:** C# 13

## ⚙️ Getting Started

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Gescale/LearningMiddleware.git](https://github.com/Gescale/LearningMiddleware.git)

2. **Navigate to the project directory:**
   ```bash
   cd LearningMiddleware

3. **Build and run the application:**
   ```bash
   dotnet build
   dotnet run
