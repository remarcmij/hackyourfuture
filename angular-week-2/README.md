# Homework assignment Week 2

This assignment assumes that you already have **node** installed on your machine. If not the case, head to [nodejs.org](https://nodejs.org/en/) and run the installer for your operating system.

With **node** is installed run the following command:

```
npm install -g json-server
```

This installs a node module that sets up a simple HTTP server implementing a RESTful API backed by a JSON data file. Some of these buzzwords will be covered in later modules.

Change the current directory by cd-ing into the `angular-week-2` that holds this README and the `data.json` file. Then type the following command:

```
json-server -w data.json
```

You should see a response similar to this:

```
\{^_^}/ hi!

  Loading data.json
  Done

  Resources
  http://localhost:3000/persons

  Home
  http://localhost:3000

  Type s + enter at any time to create a snapshot of the database
  Watching...
```

Now point your browser to the following address:

```
http://localhost:3000/persons
```

Examine the returned JSON and compare it with the `data.json` file. Add your own data to the file, reload the browser and check that your data is included.

This weeks Angular assignment is as follows:

1. Use the `$http` service to retrieve the person data from the json-server.
2. Write an Angular component that lists the name, role and organisation of each person as well a picture given by the `pictureUrl` property. Don't bother with the other fields. We will deal with them in next week's assignment.
3. Create an HTML unordered list and `ng-repeat` the component to show all persons retrieved from the server.

