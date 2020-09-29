# Example of embedding Vaadin 17 apps via iframe

`embedded-v17-app` - a simple Vaadin 17 project. In this example it's embedded via an iframe into a static HTML page.

For saving traffic it uses the browser LocalStorage to cache the dashboard charts data. See `embedded-v17-app/frontend/views/dashboard/dashboard-view.ts` (lines 121-155).

`host-non-vaadin-app` - a simple static HTML page. It has some of its own content, and an iframe with an embedded V17 app.

## Running

- start the host app: `cd host-non-vaadin-app && npm install && npm start`
- start the embedded Vaadin 17 app: `cd embedded-v17-app && mvn spring-boot:run`