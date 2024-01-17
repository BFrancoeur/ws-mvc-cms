# WebSapient MVC CMS
### A Content Management System based on the Model-View-Controller Architecture

## Project Summary
The primary purpose of this project is to demonstrate thinking like a programmer to break down what a basic CMS requires and translate my thinking into code. After sufficient development and testing, this CMS will be suitable for use in a production environment. 


## Project Languages and Technologies
- PHP
  - Composer
  - Symfony
- JavaScript
-  NodeJS
- HTML
- CSS/SCSS
- SQL/MySQL
  - MariaDB
- Apache
- Nginx (later on)


## Architecture
**Model** - The data layer. This will be the realm of classes and objects used in the CMS.

**View** - The public-facing web pages and admin panels

**Controller** - Manages and routes requests


## Modules
Ultimately, I want to take an atomic approach to building this project. As such, it will be a work in progress as I rethink and refactor the code during development. At first, I'll focus on making everything as modular as possible, with a focus on separation of concerns. 

Another aim of this project is to utilize design patterns where they make sense and simplify the codebase while delivering the outputs necessary for the CMS to function properly. 

As of right now, here is the breakdown of this project as I see it: 

- Demo Website
- Admin Area
- Users
  - User Roles
- Authentication
- Session Management
- Database
- HTTP Routing
- Internal Routing
- Templates
  - Core Templates
  - Template Partials
- Content Editor
  - Editor Interface
- Dynamic Content
- Forms
  - Contact
  - Email Subscription
  - Reviews
  - Testimonials

## Some Nice-To-Haves
- Technical SEO Optimization
  - Metadata
  - Keywords
  - Local SEO
  - On-Page SEO
 
- Memberships
- Ecommerce
  - Paid Subscriptions
  - Product and Service Purchases
 
- Automatic Image Optimization
  - Optimize to 1MB or less without visible loss of quality
 
- Automatic bundling of JS and CSS for fast page load speeds

- Convert front-end PHP to React once CMS is ready for production

- Convert CMS to a headless architecture

- SSO authentication

- Social Shares

- Social Posts by Content Author

- Design System
  - Reusable
  - Duplicable
  - Exportable (CMS agnostic?)
 
- Drag-and-Drop Page Builder

- Automatic Templating
- - For dynamic content, based on where it's to be displayed (website post, Facebook, Instagram, etc.)
 
## Strategy
1. Build out MVC architecture plus a web page to test and demo that the MVC core works
   A. Model
      1. Create an abstract Data class to interact with the database
         a. Create secure login with username and password
         b. Create methods to perform CRUD operations
      3. Create a Model class to interface with the Data class
         a. Manage all inputs to the database
         b. Manage all outputs to the front end or admin area
         c. Manage all CRUD database operations
     4. Create a database and connect to it
     5. Test database creation by adding some data and displaying it in a simple web page
   B. View
      1. Create a View class to manage front end display of web pages or admin area
      2. Create an interface to interact with the Model to get the data/content to be displayed
   C. Controller
      1. Create an abstract Router class to manage all routing requests
      2. Create a RouterManager class to manage all route requests and outputs
      3. Implement 'Pretty Links' by default
2. Create modules (as classes or objects) for additional features and functionalit  
3. Create a basic, three-page website for the front end
4. Create the admin area
   a. Dashboard
   b. Implement page editing
5. Create User Roles
   a. Subscriber
   b. Contributor
   c. Author
   d. Editor
   e. Admin
6. Test and debug. Make notes on structural and other changes to be made. Create Pull Requests to handle each item noted.
7. Let code sit for a week or two, then review it myself and make notes on any final changes. Submit PRs for each item and complete them.
8. Submit code for peer review (but where?)
9. Review feedback and distill accepted input into PRs to address.
10. Implement PRs and test.
11. Submit codebase for second round of reviews.
12. Make final changes.
13. Launch beta, open source version of CMS for public use.

## Conclusion
The core idea here is to create a CMS that is lean, fast, and secure. That's Phase I. Phase II will be the creation and implementation of select "Nice-To-Have" modules that would add value to the user experience of the CMS. 
