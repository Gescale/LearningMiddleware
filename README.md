# Learning Middleware - ASP.NET Core 9

A practical repository exploring the ASP.NET Core middleware pipeline, built alongside the **ASP.NET Core [.NET 9] Deep-Dive** course by Frank Liu. 
Demonstrating how HTTP requests and responses are handled, intercepted, and modified as they flow through the modern .NET application pipeline.

### Concepts Explored
* **The Request Delegate Pipeline:** Understanding how the `HttpContext` passes through successive middleware components.
* **Terminal Middleware (`app.Run`):** Creating endpoints that return a response and prevent further pipeline execution.
* **Chaining Middleware (`app.Use`):** Intercepting requests, performing logic (such as logging or header manipulation), and calling `next()` to pass control down the chain.
* **Branching the Pipeline (`app.Map` & `app.MapWhen`):** Conditionally routing requests based on URL paths, query strings, or specific request headers.
* **Custom Middleware Classes:** Extracting inline anonymous functions into clean, reusable, and testable C# classes.
* **Short-circuiting:** Returning early from the pipeline (e.g., rejecting invalid or unauthorized requests before they hit the controllers).
