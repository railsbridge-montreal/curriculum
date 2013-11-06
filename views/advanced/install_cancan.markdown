# User Roles with CanCan

Maybe you want your application to have an admin user who can delete offensive or spam-ridden comments. You can manage user privileges with a gem called CanCan.

## Feature ideas
- Create an administrator role and allow the administrator to delete replies.
- Allow users to delete their own replies.
- Even more censorship! Allow post authors to delete replies (authored by any user) on their own posts.
- If you are comfortable with JavaScript and implemented the [ajax replying](inline_replying_with_ajax) challenge, you could make deletion happen inline!

## Questions to think about
- If you're deploying your site, how would you make sure there is always an admin user?
- What are some ways to combat spam on your message board? Can you use Devise to keep the spam under control to some extent?

## Tools and References

- CanCan on [Github](https://github.com/ryanb/cancan)
- [ASCIIcast on CanCan](http://railscasts.com/episodes/192-authorization-with-cancan?view=asciicast)
