
# Module 7 Assignment
#### What is the Event loop?
The event loop is a mechanism that enables JavaScript to handle asynchronous code execution in a non-blocking manner, and ensures that the execution of tasks is ordered and does not block the main thread.

#### Explain the 6 phases of the event loop
timers: In this phase, the event loop checks if any setTimeout or setInterval callbacks have elapsed their specified time. If there are any callbacks that have elapsed, they are added to the task queue to be executed in the next phase.

pending callbacks: In this phase, any I/O or other system callbacks that were deferred to the next iteration of the event loop are executed.

idle, prepare: This is an internal phase that is not usually seen by developers. In this phase, the event loop prepares for the next poll phase.

poll: In this phase, the event loop waits for new events to arrive. If there are no pending timers or callbacks, the event loop will block until an event is received.

check: In this phase, any setImmediate() callbacks are executed.

close callbacks: In this phase, any close event callbacks, such as socket.on('close', ...), are executed.

#### List some best practices in server-side code development
Write modular and reusable code: Write code that can be easily modified, tested and reused in other parts of the application.

Follow a consistent code style: Consistency in code style makes the code easy to read, understand and maintain.

Use comments and documentation: Use comments and documentation to explain the code's purpose and usage.

Validate and sanitize input data: Validate all input data from users to ensure it is of the expected type and format. Also, sanitize the input data to prevent malicious code injections.

Use error handling and logging: Implement error handling to gracefully handle errors and avoid application crashes. Also, log errors and other important events to monitor the application's behavior and improve debugging.

Use secure coding practices: Implement secure coding practices, such as avoiding hardcoding sensitive data, using encryption to protect sensitive data, and validating user authentication and authorization.

Optimize application performance: Optimize code for performance by minimizing database queries, using caching where appropriate, and reducing the number of HTTP requests.

Write unit and integration tests: Write tests to ensure that the code works as expected and catches any potential issues before deploying it to the production environment.

Use version control and continuous integration: Use version control to keep track of changes made to the code, and use continuous integration to automate building, testing, and deployment of the application.

Stay up-to-date with security patches and updates: Regularly update server-side software and libraries to ensure that any security vulnerabilities are patched and the application stays secure.

### What is NPM5: How do you initialize a package in npm
NPM (Node Package Manager) is a package manager for the Node.js platform, used to install and manage dependencies (packages) required by a Node.js application. NPM5 is the fifth major release of NPM, which introduced several new features and improvements over its previous versions.

To initialize a package in NPM, follow these steps:

Open the command prompt or terminal and navigate to the root directory of your project.

Run the npm init command, which will start the process of creating a package.json file for your project. The package.json file is a metadata file that contains information about your project, including its name, version, dependencies, and scripts.

The npm init command will prompt you to answer a series of questions about your project, such as its name, version, description, entry point, test command, and author. You can either accept the default values by pressing enter or customize the values as per your project requirements.

Once you have answered all the questions, the npm init command will generate a package.json file in your project's root directory, which you can use to manage your project dependencies and scripts.

### How do you run a script in the package.json ?
npm run start