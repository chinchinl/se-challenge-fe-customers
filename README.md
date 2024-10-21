# Wave Front-end Challenge

The purpose of this exercise is to create something that we can work on together during the onsite interview. We do this so that you get a chance to
collaborate with Wavers during the interview in a situation where you know something better than us (it's your code, after all!)

There isn't a hard deadline for this exercise; take as long as you need to complete it. However, in terms of total time spent actively
working on the challenge, we ask that you not spend more than a few hours, as we value your time and are happy to leave things open to
discussion in the on-site interview.

Please use whatever tools or frameworks you feel the most comfortable with.

Feel free to email [dev.careers@waveapps.com](dev.careers@waveapps.com) if you have any questions.

**Table of Contents**

- [Project Background](#project-background)
- [Getting Started](#getting-started)
- [What I'm proud of](#what-Im-proud-of)
- [Requirements](#requirements)
  - [Functional Requirements](#functional-requirements)
  - [Technical requirements](#technical-requirements)
  - [Visual/UX Requirements](#visualux-requirements)
  - [Language requirement](#language-requirement)
- [Documentation](#documentation)
- [Submission Instructions](#submission-instructions)
- [Evaluation](#evaluation)

## Project Background

Imagine that this is the early days of Wave's history, and that **we are prototyping a new invoicing system** in Canada. Our users are small business owners who need to generate professional-looking invoices to send to their customers. For this code challenge, build out **the settings page where users (business owners) can manage their customers' information**. Our prototype will be entirely API-driven and use a Javascript single-page app as the interface to our APIs.

## What I'm proud of

I’m particularly proud of the approach I took for **data fetching** and **form validation**. For API interactions, I used `axios`, which simplifies handling asynchronous calls and improves code readability. For the edit form, I implemented an intermediate error message that appears when required fields are left empty, providing immediate feedback to users and enhancing the overall user experience.

I also took care to structure the project in a way that facilitates scalability. Key components, such as `CustomerList`, `CustomerEditForm` and `CustomerActionMenu`, are separated into individual modules, making the code more maintainable and easier to extend in future developments. Additionally, I organized the CSS styles into dedicated directories (`components`, `ui`, and `base`), ensuring the project is ready for future styling updates and can easily accommodate design refinements. This separation of concerns promotes both clarity and flexibility as the application grows.

## Getting Started

Make sure if NODEJS is installed on your computer.

### Install  Dependencies:

```sh
$ npm install
```
It will create `node_module` folder in this all dependency files will be install with this command.

### Update Next.js:

```sh
$ npm i next@latest react@latest react-dom@latest eslint-config-next@latest
```

check out [here](https://nextjs.org/docs/pages/building-your-application/upgrading)



### Run Project in development mode:

```sh
$ npm run dev
```
With is command file will be compiled and it will be loaded on local server [http://localhost:3000](http://localhost:3000).

## Requirements

### Functional Requirements

Customer information page should do the following:

- Retrieve the data from the GET endpoint: https://waveaccounting.github.io/se-challenge-fe-customers/settings.json
  - use fetch, XHR, JQuery or whatever library you're familiar with.
- Show a list of customers (in the JSON under the "customers" key).
- Let the user select a customer for editing, which shows a form with:
  - name
  - email
  - channel (value may be one of 'website', 'email', 'phone', 'word-of-mouth', 'other', 'unknown')
  - address
  - postal
  - city
  - province (For now this will be a Canada only product and all addresses are assumed to be in Canada, but we plan to roll this out to other countries later.)
- Name and email fields are required. Empty values should present an error message if submitted.
- On form submit, log the JSON payload to console (no need to mock out server calls!)

### Technical requirements

- Your application should be easy to run and browse, and should run on either Linux or Mac OS X.
- It should not require any non open-source software.
- Our desire is to approach this in a way that gives us composable, reusable code for use in later features and products. So some thought should be given to how this code could be expanded upon and repurposed.

### Visual/UX Requirements

There isn't a particular design we want you to recreate. The UI doesn't have to look beautiful, as long as:

- A user can easily differentiate different sections of the page
- A user can understand how to access and submit the customer edit form
- The page is useable on desktop and mobile devices
- It will be easy to add more styling later

### Language requirement

- Should be built in vanilla JS, Typescript or a JS-based framework (React, Angular, Vue etc).
  - Use any JS framework, tooling, scaffolding, starter-kits you are comfortable with that feels appropriate for this challenge. At Wave, we have used Backbone, Angular, React with the emphasis being heavily on React for current work.
- HTML/JSX: Should use semantic HTML tags
- CSS: Include at least ONE example of creating layout using CSS (or SASS, SCSS etc).
  - The page should be responsive.
  - But don't spend too much time making the app look pretty, we only expect the basics.

## Documentation

Please modify `README.md` to add:

1. Instructions on how to build/run your application
1. A paragraph or two about what you are particularly proud of in your implementation, and why.

## Submission Instructions

1. Clone the [repository](https://github.com/waveaccounting/se-challenge-fe-customers).
1. Complete your project as described above within your local repository.
1. Ensure everything you want to commit is committed.
1. Create a git bundle: `git bundle create your_name_front_end.bundle --all`
1. Email the bundle file to [dev.careers@waveapps.com](dev.careers@waveapps.com)

## Evaluation

Evaluation of your submission will be based on the following criteria.

1. Followed the instructions for submission
1. The submission met all the functional requirements
1. The submission met all the technical requirements
1. The various parts of the application and their usage are easily identifiable to the reviewer
1. The code can easily be repurposed, reused and expanded upon
