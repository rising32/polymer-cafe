Progressive Web App with full offline capabilities

This is an example project for how you can build a [Progressive Web Application](https://infrequently.org/2015/06/progressive-apps-escaping-tabs-without-losing-our-soul/, https://developers.google.com/web/progressive-web-apps/checklist) with Polymer and PouchDB.

The application uses a ServiceWorker to cache the Application Shell. A WebApp Manifest file ensures that the browser identifies our app as a Progressive Web Application and offers the user to install the application through an install banner.

Data is maintained in a local PouchDB database on the client, which can be synchronized to a CouchDB server. The app remains fully functional regardless of connection status.

Running locally

Install local CouchDB (optional)

If you want to work on the same data in several browsers, you can install a local CouchDB. Just follow the instructions here.

Once installed, make sure that the location attribute is correct on the <pouch-db> element in overview-page.html. Note If you do not use a database to sync with, omit the location attribute.

Install dependencies

You need polymer-cli installed to build the app npm install -g polymer-cli. Install all bower dependencies with bower install.

Run development server

polymer serve will run the application locally

Other build targets

You can build the app with polymer build. Other options are listed in the Polymer CLI documentation.