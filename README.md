# Module 3 Solo Project Guidelines

You're going to be building a **SPA** or Single Page Application.  Your frontend will be built with HTML, CSS, and JavaScript. You will construct your own backend using Rails as an API. The frontend application will communicate with the backend by making requests and receiving responses. This is a really exciting moment, the whole course up until this point is coming together!

Building out each feature you want for your application will be challenging, but you all are awesome and can do it. Remember to build iteratively and begin with a clear picture of an MVP.

## Requirements

### Do's

1. As a user of the application, I should be able to create, read, update, and delete the resource of your choosing. Choose from one of the domains below:
  + A photo sharing app
  + A ToDo List
  + A Craigslist-style app (users can perform CRUD actions on listings)
2. For MVP, your Rails backend should have one model (Photo, ToDo, Post, etc.). As a stretch goal you can add an associated item as a relationship (e.g., User). Your Rails backend will be the Single Source of Truth for your application. Your frontend will render the data it receives from the backend. The pattern will be that your frontend Fetches data from your server and then renders it. Then the user interacts with the data which may fire subsequent GET, POST or PATCH requests.
3. If your application requires a user model you can have users "sign in" or "sign up" by providing a username and/or email, but hold off on passwords for now.  

### Do Not's

1. **Do not try to implement a user authentication system with passwords.** When the page refreshes the current user will effectively be signed out. The way you learned this in the previous module relied on the fact that Rails was sending small pieces of data (cookies/sessions) back and forth along with every request and response. Now, we have two separate applications and need to use a slightly different pattern. We'll look at patterns for dealing with client-side auth later in the semester, so you'll have plenty of time to deal with this case.
