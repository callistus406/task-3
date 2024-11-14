# Stigmi Learning Test Task

# Usage

1. Install Docker
2. Install docker-compose (not the compose plugin): https://docs.docker.com/compose/install/other/
3. Run `npm run docker:up` to start and `npm run docker:down` to stop
4. Run `npm i` to install dependencies
5. Run `npm run dev` and start with tasks

## Task 1

We want to clean up our code base and introduce our new coding schemes also to older routes. Therefore,
please refactor the /deletenewestmessage route that you find in /src/routes/chats.ts and add necessary test.
For the refactor we also want to move SQL logic out of the route and into our logics folder.

## Task 2

# Overview

We want to enable our product team to easily conduct user interviews regularly to get insights in user behavior and test out feature concepts.

## Overall Process

We want to create a route to store and get information about the user interviews.

## Database

The database gets newly set up and wiped when the docker container starts. All tables that need to be set up are in `/src/logic/db.sql`

## Authentication

The routes should only be available when the user has a valid token. You can use preexisting code to handle this logic. You can either generate a new token or use the existing one in `/test/routes/chats.test.ts`

### Route

Users submit their availability, their phone number and their birth date as text in a form. Store this information together with a unique id and the time the entry was created in the db.

The route is a `POST` route with the path `/userinterview` and `field1`, `field2`, `birthdate` as body parameters. Return a success response once the data was saved.

Please make sure your code looks and works just like it would in a real world production application.

**Note: IGNORE THE TYPESCRIPT AND WRITE CODE IN PLAIN JS, IF YOU CREATE A NEW FILE ADD "// @ts-nocheck" ON TOP OF IT, SO YOU DONT FACE ANY COMPILER ISSUES. YOU CAN WRITE CODE IN PLAIN JS BUT KEEP THE FILE EXTENSION AS .ts**
