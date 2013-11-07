# Make It Pretty (With Bootstrap)

## Requirements to advance
- The site should use Bootstrap for a superfun modern look.
- When logged in, the user's email address should appear in the upper-right corner of a navigation bar.

<img src="/images/advanced/header.png" alt="Header"></img>

<div class="alert alert-info">
<h4>Timebox It!</h4>
<p>The purpose of this section is to make your app a bit prettier and demonstrate how to add CSS frameworks like Bootstrap using the Gemfile. Don't get snagged on the details of getting your CSS exactly right, unless that's valuable to you.</p>
</div>

## Discussion Items

- Chrome developer tools / Firefox Firebug plugin — how to use ’em!
- What’s Bootstrap and (optional) why is everyone totally in love with it (or at least using it all over the place)?
- Maybe review the home/index.html.erb view file as it relates to the layouts/application.html.erb view file again, and where you might want to make some edits to take advantage of bootstrap.
- Someone should explain how erb works — you'll be using it to show the user email address in right side

## Tools and References

- A gem for Bootstrap!! Let’s use the gem [bootstrap-sass-rails](https://github.com/yabawock/bootstrap-sass-rails)
- [Bootstrap docs](http://getbootstrap.com/getting-started/)
- Here's a link to the [navbar section](http://getbootstrap.com/components/#navbar)
- Reference for [HTML and CSS](http://www.htmldog.com/)

## Hints

- Don't forget to read the readme!
- There are a couple of Bootstrappy ways to move text around — look for "Component alignment" in the docs.
- Devise has a helper method for accessing the current user - go back to the devise readme to find it.

## Really Big Hint

If you can't get the right HTML mojo for the Bootstrap nav bar, or want to move on quickly to the next page, here's some code you can drop into your layout (after installing Bootstrap!) that should work. The code should go immediately after your `<body>` tag.

```html
<div class="navbar navbar-inverse navbar-fixed-top" role="navigation">
  <div class="container">
    <div class="navbar-header">
      <a class="navbar-brand" href="#">Message Board</a>
    </div>
    <ul class="nav navbar-nav">
      <li class="active"><a href="/">Home</a></li>
    </ul>
    <p class="navbar-text pull-right">logged_in_user@email.com | <a href="log_out_link_here">Log Out</a></p>
  </div>
</div>
```

You still have to add code to show the real logged in user and add a real log out button!

Next Step:
Go on to [Add Pages To Create And Look At Individual Posts](add_pages_to_create_and_look_at_individual_posts)
