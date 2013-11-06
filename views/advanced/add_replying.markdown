# Add Replying

## Requirements to advance

- The user should see a 'New Reply' link or button on a post's show page which takes them to a form. The form should include the title of the post being replied to.
- The user should be able to create a new reply to a post using the 'New Reply' form.
- The user should see all the replies to a post on the post’s show page.
- If the user doesn’t submit all required fields, they should see some error messaging, but they shouldn’t lose any of their work.

<div class="row">
  <div class="span6">
    <h4>Create View</h4>
    <img src="/images/advanced/create_post.png" alt="Create A Post"></img>
  </div>
  <div class="span6">
    <h4>Show View</h4>
    <img src="/images/advanced/show_post.png" alt="Show A Post"></img>
  </div>
</div>

## Discussion Items

- What is a nested resource? When is it appropriate and how does it help?
- How do the repliescontroller and postscontroller interact?
- What should happen to the routes file for this nesting business to work?

## Tools and References

- RailsGuides - Rails Routing from the Outside In http://guides.rubyonrails.org/routing.html

Next Step:
Go on to [Inline Replying On A Post](inline_replying_on_a_post)
