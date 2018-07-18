# ASPNETCoreWebAPIDispatcherWithAsyncAwait
A simple ASP .NET Core Web API App which presents work of airline dispatchers using EF Core and async await

### In the created project (ASPNETCoreWebAPIDispatcher), you need to add asynchrony using async / await (you can not use Wait or Result). All operations must work with the Task.

### What should be done:

* All possible database queries must be performed asynchronously

* All requests to the controller must be performed asynchronously

* Write a new API method that will load the first 10 Crew with the remote API and:

      asynchronously write them to the database;
      
      asynchronously write data to log_date_time.csv (the date must be stored in the name of the synchronization);
      
      To implement parallelism, you can use Task.WhenAll ().
* Write a helper method that will simulate a lengthy operation:

      implement a fictitious delay using System.Timers.Timer and event Elapsed;;
      
      wrap the work with the event in the Task using TaskCompletionSource;
      
      Use a helper with an asynchronous interface (Returns Task) when fetching data from a table.
