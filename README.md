# Northwind-Flow


<img width="926" alt="image" src="https://github.com/user-attachments/assets/fe5cb1ab-9730-4cb2-abbe-0abb5e490eb3" />


Here's a quick look at the flow. 
This integration starts with a SOAP request, fetches data from the Northwind OData service, transforms it, and finally sends the result via email using a Mail adapter. Also included an exception subprocess to handle errors cleanly.

 🔹 SOAP Sender: Accepts incoming requests.
 🔹 Content Modifier: Prepares request payload.
 🔹 Request Reply: Calls Northwind OData service.
 🔹 Message Mapping: Transforms the OData response.
 🔹 Groovy Script: Applies custom logic before output.
 🔹 Mail Adapter (Receiver): Sends the final message via email.
 🔹 Exception Subprocess: Handles errors and sends alternate flow if needed.

