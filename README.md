# Omnis Library - Sentry.io Integration

The **Omnis Library** is designed to provide seamless integration with [Sentry.io](https://sentry.io/), helping you capture and monitor errors, performance issues, and other events in your application with ease. This integration provides a direct link to Sentry, allowing for powerful tracking, error management, and reporting to enhance your application's reliability.

## Documenation
- **General Sentry Docs:** [Sentry Docs](https://docs.sentry.io/)
- **Docs about JSON structure:** [JSON structure](https://develop.sentry.dev/sdk/data-model/event-payloads/)

## Features
- **Error Tracking:** Capture and log errors in real-time to Sentry.
- **Customizable Event Data:** Configure the event payload to capture additional context about errors and performance issues.
- **Fetching Error Data:** Fetches all relevant stackinformation from Omnis

## How to setup Sentry in any existing Omnis Application:

1. Create a new project in Sentry.io (SDK needs to be set to "Other")
2. Copy the Objects OSentry and OSentryHL to your library
3. Create a Task Variable "tSentry" from the type "OSentryHL"
4. Inititalize your Object in your Startup Task using the Projects DSN; Do tSentry.$init('\<DSN\>')
5. Create a Testcall using "Do tSentry.$captureMessage('Hello World!')"
6. You should be done!
