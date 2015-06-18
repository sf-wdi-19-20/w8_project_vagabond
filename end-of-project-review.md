#Project Vagabond Peer Review

####Objectives:

* Peer-review Project Vagabond
    - Steal good ideas
* Create several Github Issues
    - If you have time, fork it, fix the issue, and submit a pull request!

####Peer Projects

Keep in mind you may need to look at the most recent / active branch (i.e. `develop`, and not necessarily `master`).

1. https://github.com/danlyg/ProjectVagabond
1. https://github.com/justinldiaz/Vagabond_app
1. https://github.com/wdi18vagabond/Vagabond
1. https://github.com/SpencerCornelia/VagabondApp
1. https://github.com/smallhaxe/vagabond/tree/working
1. https://github.com/cachrisman/Project-Vagabond/

### Instructions

* Clone a project and set it up locally
    * Don't forget the database: `rake db:create db:migrate`
    * Don't forget to run the server: `rails s`

####Questions to ask as you explore:
* Take a look at the **README**
    - Does it tell you how to setup/install the project in development?
    - Are there any custom rake tasks?
    - Is there any seed data? (`rake db:seed`)
* Take a look at the **commit history** / branches.
    - Try `git log --reverse`
    - What story does it tell?
    - How were tasks divided?
* Take a look at the **database schema**
    - What's the relationship between a user / city / post?
        + Where are the foreign keys?
    - How is this reflected in the routes?
        + Are the routes RESTful?
    - How is this reflected in the **model**?
        + Is there a convenient way to ask for...
            * `user.posts`?
            * `post.city.name`?
            * `city.latest_posts`?
* Take a look at the **form** in the LogPosts#edit view
    - How was the form created / generated?
    - How do you add a city? Are the cities hard coded?
    - How are validations / flash errors handled?
* Take a look at the Users#show controller & view
    - How is `join date` implimented / formatted?
    - How are a users' posts displayed?
        - How would you find a posts' city name?
    - Is there proper **seperation of concerns** between the view and the controller?
        + Is there view (presentation) logic in the controller?
            * e.g. Are values being _formatted_ in the controller?
        + Is there controller logic in the view?
            * e.g. Is the database being queried directly from the view?
        + Are there too many instance variables / globals floatting around?
* Take a look at the **google map** in the Cities#show view
    - How is the maps integrated?
        + Is it inside the html, in a `script` tag?
        + Is it in a seperate javascript file?
        + How does the map know where to center? Where does the latitude/longitude come from?
* Take a look at the **partials** in the views folder.
    - What partials did the team create?
        + Are there form partials?
        + Is there a basic page layout?
        + What about the navigation bar?

####Finally:

* What **gems** did the team use? (Gemfile)
* How much **test coverage** is there? (Rspec)
* How **dry** is the code? Are methods clearly named? Is there repetition?


Don't forget: Create several Github issues & fix 'em!
