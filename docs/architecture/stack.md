# Stack

## Database

We will use PostgreML as our database.

## Front End

The system is designed to be uncoupled to the application enabling the technology used to be readily changed.

I am opting for a Django front end as this is a leading Python Content Management System and I am already familiar with the framework.

For client-side reactivity, HTMX and Alpine.js are used. These are more than sufficinet to recreate the React/Vue experience.

## Hosting

Ulimately, Microsoft Azure will be used to host the application and the database. It also has many Cognitive Search tools that we might include.

For now, we will use `render.com` to host the application. It is an industrial level hosting platform.

The database can be readily migrated to Azure.