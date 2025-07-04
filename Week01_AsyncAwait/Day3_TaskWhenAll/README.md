# Task.WhenAll vs await foreach — Know the Difference

Just because a method is async doesn’t mean it's concurrent.  
Use `Task.WhenAll()` when you need true parallelism across multiple tasks — otherwise, you might be waiting unnecessarily.

## ⚡ Key Differences

- `await foreach` runs sequentially — one item at a time
- `Task.WhenAll()` runs all tasks at once and waits for all to finish
- Use parallelism wisely for network calls, background processing, or fan-out patterns

📅 **Date:** June 25, 2025  
🔗 **Code:** [Program.cs](./Program.cs)  
🔗 **Author:** [Avijit Roy on LinkedIn](https://www.linkedin.com/in/heyavijitroy/)  
🏷 **Tags:** #dotnetdailytips #DotNetWithRoy #csharp #asyncawait #taskparallelism #Day3_DotNetWithRoy
