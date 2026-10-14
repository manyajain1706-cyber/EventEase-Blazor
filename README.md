# EventEase — Blazor Event Management

A learning project demonstrating event cards, navigation, two-way data binding, registration validation, session state, and attendance tracking using C# and Blazor.

## Features
- Reusable Event Card component with event title, location, date, capacity, and registration count.
- Routing to Events, Registration, and Attendance pages.
- Two-way binding with Blazor form inputs and attendance checkboxes.
- Data annotation validation for names and email addresses.
- Duplicate-registration and event-capacity checks.
- Scoped session state for a simple current-user display.
- Attendance tracking with a present/not-marked checkbox.
- Responsive CSS styling.

## Requirements
Install the .NET 8 SDK or a compatible newer SDK.

## Run locally
Open a terminal in this folder and run:

```bash
dotnet restore
dotnet run
```

Open the local URL shown in the terminal.

## Copilot assistance summary
Use Microsoft Copilot to help review and explain the implementation at each stage. In your submitted summary, describe only assistance you actually used:
1. **Foundation:** generating and reviewing the reusable Event Card component and event model.
2. **Data binding:** understanding `@bind`, parameters, and Blazor form components.
3. **Routing:** checking page routes and navigation links.
4. **Debugging and optimization:** reviewing validation, duplicate-registration checks, capacity checks, and error handling.
5. **Advanced features:** reviewing the registration form, session state service, and attendance tracker.
6. **Documentation:** improving the README and checking that descriptions match the implementation.

## Limitations
This is a demo. Events and registrations are stored in memory and reset when the application restarts. The session service is not secure authentication. A production application would need persistent storage, authentication, authorization, and more comprehensive testing.

## Manual test checklist
- Open each navigation link.
- Submit the registration form with missing fields and an invalid email.
- Register a valid attendee and check the Attendance page.
- Try registering the same email twice for the same event.
- Mark an attendee present.
- Open an unknown URL and check the not-found page.
