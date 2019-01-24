---
title: 'Project 1: Wellness Tracker'
date: '2019-01-24T00:00:00.000Z'
---

Let's start with something small, shall we? We are going to build a wellness tracker. 

Here are the requirements: 

1. The user should only be able to log their mood and see their history (and no one else's)
2. The user should be able to select one of three moods and type notes for how they are doing that day
3. Only one submission is allowed per day
4. The user should be able to see a visual representation of how they have been doing for the past month

## Mockups

Here's what we will be building: 

[TODO]


## Arch

This arch is definetely overkill for a small app - BUT! we are starting from something small and trivial with the intention of building something big, complex, _and maintainable_. 

1. The app will be comprised of a API server and a client-side single page app.
2. The API server will be hosted on a cheap linux VM on the public cloud. 
3. The SPA will be served from the same server as the API server.
4. The code will be hosted on Github in a monorepo.
5. Every push will trigger a build and deploy. 
6. The app will be built on the CI server and synced to the production host
7. The CI server will then run a deploy script on the production server to finalize the deployment (this will be improved on in future posts).
6. The API server will consist of a Rust (Rocket) webapp using Diesel to talk to a SQLite database.
7. The client-side SPA will be written in Elm and talk to the API server using HTTP.

## Task list

Now that we see what we are building, let's think through the steps of how to get there: 

### High level

Setup

- Create a new repository with Rust/Rocket/Diesel application setup for SQLite
- Create a new SPA using create-elm-app
- Get the API server to serve the elm app
- ....

TO BE CONTINUED.
