# Cloud To-Do List — Micro Project Starter

## What is included?
- Add tasks and optional due dates
- Mark tasks completed or pending
- Filter All / Pending / Completed
- Delete tasks and clear completed tasks
- Summary cards showing total, completed, and pending tasks
- Responsive layout for laptop and mobile screens

## Run it in Firefox
1. Extract the ZIP file.
2. Open the extracted folder.
3. Double-click `index.html`, or right-click it and choose Firefox.
4. Add a task and test the buttons.

## Important: demo vs real cloud app
This starter uses `localStorage`, so tasks are saved only in the current browser profile on that device. It is a front-end prototype, not yet a shared cloud database application.

For a genuinely cloud-based version on Microsoft Azure, use:
- **Azure Static Web Apps** to host the website
- **Azure Functions** to provide API endpoints (for example, GET/POST/DELETE tasks)
- **Azure Cosmos DB** to store tasks online
- **Microsoft Entra ID** (optional for a student demo) for sign-in

## Suggested Azure architecture
User's Firefox browser → Azure Static Web Apps (HTML/CSS/JavaScript) → Azure Functions API → Azure Cosmos DB (task data)

## Suggested development steps
1. Test this prototype in Firefox.
2. Create an Azure account and an Azure Static Web App.
3. Publish the front-end files to Azure Static Web Apps.
4. Create an Azure Function API for task operations.
5. Configure Azure Cosmos DB and connect the function to it.
6. Replace the `localStorage` calls in `app.js` with API requests.
7. Test add, complete, delete, and filtering after deployment.

## Project explanation for presentation
**Objective:** Build a simple task management application that helps users record, organize, and track daily tasks.

**Problem:** People may forget tasks or have difficulty tracking what is completed.

**Solution:** The application lets users add tasks, set due dates, mark tasks complete, and view pending tasks.

**Technologies:** HTML, CSS, JavaScript, Firefox for testing, and Microsoft Azure for cloud hosting/backend in the full version.

**Current prototype limitation:** Data is saved in the browser only. Azure Functions and Cosmos DB must be connected for tasks to be available across devices.
