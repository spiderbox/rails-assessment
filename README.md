# SpiderBox Design Ruby on Rails Assessment

## 1. THE URL SHORTENER CHALLENGE

Your mission is to make a URL shortener full-stack application using any database engine, Ruby On Rails, (bonus points if the frontend is a SPA in ReactJS).
Create one repo if you work entirely with RoR, or two repos if you work with Rails + React. Send us the links of both repositories.

+kudos If you use docker, that would be great and give extra points.



### CORE REQUIREMENTS
- As a visitor, I want to create an account for the app, so that I become an active user.
    Acceptance Criteria:
      - Application needs my name, email, and password.
      - Duplicated emails are not allowed.
      - Validates email input.
- As an active user I must be able to put a URL into the home page and get back a URL of the shortest possible length.

      AC:
        - You shouldn't use any gem or library that provides the short url algorithm
        - Inputting a valid URL should result in displaying the new shortened URL to the user.
        - Inputting an invalid URL should result in displaying errors to the user.

- As an active user I must be able to manage my links, edit, create, destroy, etc.

- As an active user, every time I share this link, I must be redirected to the full URL when we enter the short URL (ex: [http://app.com/aSdF](http://app.com/aSdF)​ =>​ [​https://google.com​](​https://google.com​)).
- As an active user I want to see a list of my links, ordered by creation date.
- As an active user I want to click on my links to see details and stats.

      AC:
        - I want to see how many times my link was clicked.

- There must be a README that explains how to set up the application and the algorithm used for generating the URL shortcode.

- As an active user I want an API key to access and integrate any other platform with this shortener.

      AC:
        - I want an endpoint to access all my links.
        - All endpoint results must be paginated.
        - I want an endpoint to shorten new URLs.

- Bonus point if you test all your code with RSpec.


> \* Research and understand how [Bit.ly](http://bit.ly) and [TinyURL](https://tinyurl.com/) work before you decide on how to generate URLs of the shortest possible length.
There must be a view for the Top 100 most frequently accessed URLs.
<br />
<br />
<br />

## 2. THE PROJECT MANAGEMENT TOOL CHALLENGE

<br />

Your mission is to make a project management full-stack application using Postgres DB, Ruby On Rails (bonus points if the frontend is a SPA in ReactJS).

Create one repo if you work entirely with RoR or two repos if you work with Rails + React. Send us the links of both repositories.

<br />

*+extra points If you use docker.*

<br />

### CORE REQUIREMENTS
- As a visitor, I want to create an account for the app so that I become an active user.

  Acceptance Criteria:
    - Application needs my name, username, email.
    - Duplicated emails are not allowed.
    - Validates email input.
    - Authentication must be passwordless (by email)

- As an active user I want to be able to create multiple projects so that I can scope my tasks with a common topic.

  AC:
    - This is a multitenant application, which means I can create multiple projects and invite other users to join them.
    - Project must-have title, slug, description, and status attributes.
    - Membership role of the user who created the project is Owner.

- As an active user I want to see a list of projects where I have a membership.

  AC:
    - Users must have and belong to many projects.
    - Users must have a role inside a project, roles are owner, admin, member.
    - Owner and admin can invite more users by email.

- As a project owner, I want to create columns for my kanban board.

  AC:
    - Columns in my board must-have title, description, sort_order (integer).
    - columns must be ordered by sort order column
    - project details view must show the kanban board.

      PROJECT NAME

      |Backlog [+]|ToDo [+]|Doing [+]|Done [+]|Closed [+]|
      |-|-|-|-|-|
      |task title x|task title x|task title x|task title x|task title x|
      |task title x|task title x|Task namedsds|task title x||
      |task title x|||||
      |task title x|||||

- As a project owner, admin, or member, I can add tasks to any column I want.

  AC:
    - I can see a [+] button in the column header.
    - When I click on the [+] button, I see a form where I can write the title, description, and assigned user.

- As a project owner, admin, or member I can assign a task to a project member.

- As a project member I want to open the project board so that I can see the tasks.

  AC:
    - I want to see columns with tasks.

- As a project member I want to move tasks between columns so that I can organize myself.

  AC:
    - I want to move tasks from one column to any other column I want.

- As a project member I want to track activity in my project so that I can see a newsfeed.

  AC:
    - I want to track changes in columns, tasks, and projects.
    - I want to see who created the project.
    - I want to see who updated the project.
    - I want to see who created a column.
    - I want to see who edited a column.
    - I want to see who deleted a column.
    - I want to see who created/edited/deleted a task.
    - I want to see who moved a task to another column.

<br />

_This is a challenge for a backend position, there is no need to details design and interactions, as long as it works, it is fine for us._

