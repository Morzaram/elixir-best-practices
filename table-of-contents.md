Part I - Database

1. Many-to-Many Relationships with Ecto
2. Declarative Named Queries with Ecto
3. Connecting to Multiple Databases with Ecto
4. Setting Default Criteria for Model Operations with Ecto
5. Adding Behavior to Ecto Associations
6. Creating Polymorphic Associations with Ecto
7. Versioning Your Models with Ecto
8. Performing Calculations on Model Data with Ecto
9. DRY Configuration with Ecto
10. Using Models Safely in Migrations with Ecto
11. Creating Self-referential Many-to-Many Relationships with Ecto
12. Protecting Data from Accidental Mass Update with Ecto
13. Creating a Custom Model Validator with Ecto
14. Nesting Ecto Associations
15. Seeding Your Database with Starting Data with Ecto
16. Using Helpers in Models with Ecto
17. Avoiding Dangling Database Dependencies with Ecto

- Part II - Advanced Ecto

1. Creating Custom Repositories with Ecto
2. Using Ecto Changesets
3. Creating Custom Ecto Types
4. Using Ecto Enums
5. Constraining Queries with Ecto
6. Creating and Using Embedded Schemas with Ecto
7. Using Ecto Multi
8. Monitoring and Optimizing Ecto Performance
9. Creating and Using Ecto Associations in Raw SQL
10. Creating Ecto Schemas from Existing Databases

Part III - Working with Ecto and Phoenix

1. Using Ecto in Phoenix Controllers
2. Creating Ecto Schemas in Phoenix
3. Using Ecto in Phoenix Views
4. Using Ecto in Phoenix Tests
5. Using Ecto in Phoenix Migrations
6. Monitoring Ecto in Phoenix with Telemetry

Part II — Controller

22. Create Nested Resources with Phoenix 76
23. Create a Custom Action in a Phoenix Controller 80
24. Create a Helper Method to Use in Both Controllers and Views 83
25. Trim Your Phoenix Resources 85
26. Constrain Routes by Subdomain (and Other Conditions) 88
27. Add Web Services to Your Actions with Phoenix 90
28. Write Macros with Phoenix 94
29. Manage a Static HTML Site with Phoenix 98
30. Syndicate Your Site with RSS 100
31. Set Your Application’s Home Page with Phoenix 108

Part III — User Interface

32. Create a Custom Form Builder with Phoenix 112
33. Pluralize Words on the Fly (or Not) 116
34. Insert Action-Specific Content in a Layout with Phoenix 118
35. Add Unobtrusive Ajax with Phoenix and jQuery 120
36. Create One Form for Many Models with Phoenix 125
37. Cache Local Data with Phoenix and HTML5 Data Attributes 131

Part IV — Testing

38. Automate Tests for Your Models with ExUnit 136
39. Test Your Controllers with ExUnit 141
40. Test Your Helpers with ExUnit 145
41. Test Your Outgoing Mailers with ExUnit 148
42. Test Across Multiple Controllers with ExUnit 151
43. Focus Your Tests with Mocking and Stubbing 157
44. Extract Test Fixtures from Live Data with ExUnit 163
45. Create Dynamic Test Fixtures with ExUnit
46. Measure and Improve Your Test Coverage with ExCover 172
47. Create Test Data with Factories with ex_factory 176

Part V — Email

48. Send Gracefully Degrading Rich-Content Emails with Phoenix 182
49. Send Email with Attachments with Phoenix 185
50. Test Incoming Email with Phoenix 188

Part VI — Big-Picture

51. Roll Your Own Authentication with Comeonin 198
52. Protect Your Application with Basic HTTP Authentication with Plug 203
53. Authorize Users with Roles with Guardian 206
54. Force Your Users to Access Site Functions with SSL 211
55. Create Secret URLs with Guardian 212
56. Use Phoenix Without a Database 216
57. Create Your Own Elixir Package 221
58. Use Dependencies to Manage Per-Environment Dependencies with Mix 224
59. Package Tasks for Reuse with a Package 226
60. Explore Your Phoenix Application with the Interactive Elixir Shell 228
61. Automate Work with Your Own Tasks with Mix 230
62. Generate Documentation for Your Application with ExDoc 235
63. Render Application Data as Comma-Separated Values with Poison 236
64. Debug and Explore Your Application with the IEx.pry 239
65. Render Complex Documents as PDFs with Phoenix 244

Part VII — Extending Phoenix 66. Support Additional Content Types with a Custom Phoenix Renderer 250 67. Accept Additional Content Types with a Custom Phoenix Parameter Parser 253 68. Templatize Your Generators 256 69. Create a Custom Generator 261 70. Create a Custom Railtie 266

Part VIII — Advanced Elixir 71. Use Concurrency to Your Advantage with Elixir and OTP 270 72. Test Your Application’s Performance with Benchmarking with ExBench 273 73. Use Cachex to Cache Model Data and Actions 277 74. Use Multiple Databases with Ecto 283 75. Create a Search Engine with ElasticSearch 287 76. Use Phoenix.Email with Different Delivery Methods 290 77. Use Phoenix.Email with Different Email Backends 294 78. Create a Plug Middleware for Your Application 297 79. Use the Phoenix.Static Plug to Serve Static Assets 300 80. Use the Phoenix.Assets Plug to Manage JavaScript and CSS Dependencies 304 -->

---

     66. Create Custom Plugins for Phoenix to add custom functionality to your application.
     67. Use LiveView to add real-time, reactive components to your Phoenix application.
     68. Integrate GraphQL with Absinthe to provide a flexible, efficient way to access data from your Phoenix application.
     69. Implement Internationalization (i18n) and Localization (l10n) with Gettext to make your Phoenix application available in multiple languages.
     70. Use Broadcasters and Channels with Phoenix.PubSub to implement real-time, bidirectional communication in your application.
     71. Use Ecto.Multi to execute multiple database operations in a single, transactional block.
     72. Implement Caching with Phoenix.Cache to improve the performance of your Phoenix application.
     73. Use Phoenix.Presence to track online users and implement real-time presence notifications in your application.
     74. Implement Custom Error Pages with Phoenix.ErrorPages to provide a custom, user-friendly experience when errors occur in your application.
     75. Use Phoenix.Token to generate and verify secure, time-limited tokens for use in your application.
     76. Use Phoenix.Channels and Phoenix.Socket to implement real-time, bidirectional communication between client and server.
     77. Use Ecto.Schema and Ecto.Changeset to define and validate the data structures and constraints of your database models.
     78. Use Ecto.Repo to manage database connections and transactions in your Phoenix application.
     79. Use the Phoenix.HTML library to build and render HTML templates in your Phoenix application.
     80. Use Phoenix.Ecto.SQL to define and execute raw SQL queries in your Phoenix application.
     81. Use Phoenix.Router to define and manage the routes for your Phoenix application.
     82. Use Phoenix.Controller and Phoenix.View to implement the MVC pattern in your Phoenix application.
     83. Use Phoenix.Endpoint to configure and manage the entry points for your Phoenix application.
     84. Use Phoenix.Logger to log messages and events in your Phoenix application.
     85. Use Phoenix.Test to write and run automated tests for your Phoenix application. -->

Part I - Database

    Many-to-Many Relationships with Ecto
    Declarative Named Queries with Ecto
    Connecting to Multiple Databases with Ecto
    Setting Default Criteria for Model Operations with Ecto
    Adding Behavior to Ecto Associations
    Creating Polymorphic Associations with Ecto
    Versioning Your Models with Ecto
    Performing Calculations on Model Data with Ecto
    DRY Configuration with Ecto
    Using Models Safely in Migrations with Ecto
    Creating Self-referential Many-to-Many Relationships with Ecto
    Protecting Data from Accidental Mass Update with Ecto
    Creating a Custom Model Validator with Ecto
    Nesting Ecto Associations
    Seeding Your Database with Starting Data with Ecto
    Using Helpers in Models with Ecto
    Avoiding Dangling Database Dependencies with Ecto

    Part II - Advanced Ecto

    Creating Custom Repositories with Ecto
    Using Ecto Changesets
    Creating Custom Ecto Types
    Using Ecto Enums
    Constraining Queries with Ecto
    Creating and Using Embedded Schemas with Ecto
    Using Ecto Multi
    Monitoring and Optimizing Ecto Performance
    Creating and Using Ecto Associations in Raw SQL
    Creating Ecto Schemas from Existing Databases

Part III - Working with Ecto and Phoenix

    Using Ecto in Phoenix Controllers
    Creating Ecto Schemas in Phoenix
    Using Ecto in Phoenix Views
    Using Ecto in Phoenix Tests
    Using Ecto in Phoenix Migrations
    Monitoring Ecto in Phoenix with Telemetry

Part IV - Controller

    Create Nested Resources with Phoenix
    Create a Custom Action in a Phoenix Controller
    Create a Helper Method to Use in Both Controllers and Views
    Trim Your Phoenix Resources
    Constrain Routes by Subdomain (and Other Conditions)
    Add Web Services to Your Actions with Phoenix
    Write Macros with Phoenix
    Manage a Static HTML Site with Phoenix
    Syndicate Your Site with RSS
    Set Your Application’s Home Page with Phoenix

Part V - User Interface

    Create a Custom Form Builder with Phoenix
    Pluralize Words on the Fly (or Not)
    Insert Action-Specific Content in a Layout with Phoenix
    Add Unobtrusive Ajax with Phoenix and jQuery
    Create One Form for Many Models with Phoenix
    Cache Local Data with Phoenix and HTML5 Data Attributes

Part VI - Testing

    Automate Tests for Your Models with ExUnit
    Test Your Controllers with ExUnit
    Test Your Helpers with ExUnit
    Test Your Outgoing Mailers with ExUnit
    Test Across Multiple Controllers with ExUnit
    Focus Your Tests with Mocking and Stubbing
    Extract Test Fixtures from Live Data with ExUnit
    Create Dynamic Test Fixtures with ExUnit
    Measure and Improve Your Test Coverage with ExCover

Part VII - Email

    Send Gracefully Degrading Rich-Content Emails with Phoenix
    Send Email with Attachments with Phoenix
    Test Incoming Email with Phoenix

Part VIII - Big-Picture

    Roll Your Own Authentication with Comeonin
    Protect Your Application with Basic HTTP Authentication with Plug
    Authorize Users with Roles with Guardian
    Force Your Users to Access Site Functions with SSL
    Create Secret URLs with Guardian
    Use Phoenix Without a Database
    Create Your Own Elixir Package
    Use Dependencies to Manage Per-Environment Dependencies with Mix
    Package Tasks for Reuse with a Package
    Explore Your Phoenix Application with the Interactive Elixir Shell
    Automate Work with Your Own Tasks with Mix
    Generate Documentation for Your Application with ExDoc
    Render Application Data as Comma-Separated Values with Poison
    Debug and Explore Your Application with the IEx.pry Debugger
    Use the Phoenix Router to Generate URLs
    Use the Phoenix Router to Handle Redirects
    Use the Phoenix Router to Handle Errors
    Set Up a Deployment Workflow with Distillery and Edeliver
    Use Docker to Simplify Development and Deployment
    Create a Systemd Service File to Run Your Phoenix Application as a Service
    Use Node.js to Build a Real-Time Web Interface with Phoenix Channels
    Use Phoenix Presence to Add Real-Time User Tracking to Your Application
    Use Phoenix PubSub to Create Real-Time Notifications
    Use the Ecto Sandbox to Avoid Data Corruption During Development
    Render Complex Documents as PDFs with Phoenix
