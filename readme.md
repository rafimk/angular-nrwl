Angular - Frontend SPA framework
Nrwl - Bootstrap angular project. Generate modules as libraries. Used for project scaffolding
ngx-pipes - UI library for commonly used pipes & filters
Syncfusion - UI library used for all visual layouts, components and styles.
Keycloak - IAM library used fot authentication and authorization
Header - Web component library to display application header, menu and notification.

Project Guidelines:
===================
    UI broken down into multiple components & containers for better scalability and maintenance.
    Modules are broken down into small libraries to reduce overall bundle size and lazy load the modules on demand.
    Components are reused as and when required to minimize duplicate codes and redundancy.
    Angular application bootstraps only after successful authentication from Keycloak. Application redirects users to Keycloak login page to attempt authentication
    Once the Keycloak validates and authenticates the user, it then redirects to angular application.
    Angular application then utilizes the Bearer token to receive from Keycloak to make API service calls to read/write data to the backend servers.
    Header library is used to display the header and menu items. 
    
