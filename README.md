# Alpha JS
A front-end framework with KISS in mind. Alpha JS is a page-centric and event-driven way to build web apps. We believe this is intuitive and simpler. After all, any web app consists of 'pages' that display relevant data and allow the user to perform relevant operations.

# The Approach

Your web app is split into global and page spaces. The global space defines global events and holds the 'state' of your entire app. Page space consists of components and state data relevant to the page. Components are defined independentally of pages, but can be used in any page. Components don't have a state, and are one way bound to data in the page state or global state. Actions on components can fire events (in global/page space). The page listens for events, and each event triggers its listeners that can in turn affect the page state and its components. Page state is destroyed once the page changes, but the global state persists.
