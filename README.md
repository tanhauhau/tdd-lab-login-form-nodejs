# Login Form Demo

This repository contains a simple web application written in NodeJS.

## Workshop

The product owner is very happy with the application, but would like some enhancements.

### User Story

> As a **User**, <br>
**When** I login with password which is too short.<br>
**Then** I should see an alert telling me my password is too short.

Acceptance Criteria:

- Error alert should be visible when the password is too short.
- This should be a server-side implementation.
- There should be additional automated test coverage.

---

## Running the application

Open this folder in your terminal app. And run these commands in the terminal. This app was build with `v10.16.0`.

1. Install dependencies:

    ```
    npm install
    ```

2. Start the app:

    ```
    npm start
    ```
    
    You can open this url in your browser to view the app: <http://localhost:3000>
    
3. To run the test:

    ```
    npm test
    ```

4. To run the linter:

    ```
    npm run jslint
    ```

5. To fix linting issues:

    ```
    npm run jsfmt
    ```

## Architecture

- **[Express](https://expressjs.com/)** - Application framework in NodeJS.
- **[Pug](https://pugjs.org)** - Templating engine for displaying the HTML pages.
- **[Mocha](https://mochajs.org/)** - Testing framework.
- **[Chai](https://www.chaijs.com/)** - Test Assertion library.
- **[Supertest](https://github.com/visionmedia/supertest)** - Low-level testing library for HTTP services.
- **[Bootstrap](https://getbootstrap.com/)** - CSS framework for building websites.
- **[ESLint](https://eslint.org/)** - Find and fix problems in your JavaScript code.
    - This application uses the [StandardJS](https://standardjs.com/) coding style.

## Routes

1. `GET /`

    This is the home page. The login form is also here.

2. `POST /users`

    This is how you login to the app. You will need to login with `email` and `password`.

    The default email is `demo@example.com` and password is `demo1234`.

3. `GET /users/welcome`

    Landing page after you have successfully logged in with the correct credentials.

4. `GET /users/logout`

    URL for logging out of the application.