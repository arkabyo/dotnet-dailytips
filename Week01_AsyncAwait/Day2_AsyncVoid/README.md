﻿# Avoid async void — unless you're writing event handlers

Using `async void` may seem convenient, but it breaks exception handling and makes your code untestable. Use `async Task` instead for better control and reliability.

## 🚫 Why it's a trap

- Exceptions can't be caught via `try/catch`
- Async flow becomes unawaitable
- Breaks unit testing and flow control

📅 **Date:** June 24, 2025  
🔗 **Code:** [Program.cs](./Program.cs)  
🔗 **Author:** [Avijit Roy on LinkedIn](https://www.linkedin.com/in/heyavijitroy/)  
🏷 **Tags:** #dotnetdailytips #DotNetWithRoy #csharp #asyncawait #asyncvoid #Day2_DotNetWithRoy
