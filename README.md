# Homework Chat Room

## Help Students Collaborate on Assignments
A group of experienced teachers have an idea for a collaboration tool for students. Their first step is straightforward—create a chat room where students can work together on assignments.

Students should be able to easily create a new chat for their assignment groups and communicate with each other in real-time. This early prototype will serve as a foundation for future enhancements (which are outside the scope of this project).

## Task description
Develop a Phoenix application that allows any user to start a chat room powered by LiveView.

Your implementation should meet the following criteria:

- Follows idiomatic Elixir practices
- Is tested
- Is easily understandable and maintainable by other developers
  
## Preview

Watch this short clip to see the final result in action.

## Requirements

### Data model
- Users, chatrooms, and messages are stored in a database
- Each user has a name
- Each chatroom has a name
- Each message belongs to a chatroom
- Each message contains text content

### Permissions
- Users log in by email and password
- All pages require user authentication

> [!TIP]
> You can use the command `mix phx.gen.auth` ([documentation](https://hexdocs.pm/phoenix/mix_phx_gen_auth.html)) to inject a user authentication service into your Phoenix codebase. 

### Home page
- A button for creating a new chatroom

### Chatrooms
- A random name is assigned to each chatroom upon creation
- Users in a chatroom can change the name of the chatroom
- A form to write and submit new messages
- A chronological list of all the messages in the chatroom
- A unique, random chatroom identifier is included in the URL, allowing students to share it with their assignment group only

### Documentation
- A README.md that briefly explains how the application can be run and used

## Optional
Looking to take the project further? Consider adding one or more of these features:

- A teacher role that permits assigning students to chatrooms (rather than relying on URL sharing)
- Functionality to track and display who is currently online (see the [presence tracking](https://hexdocs.pm/phoenix/Phoenix.Presence.html) that is built into Phoenix)
- Not loading all chatroom messages on inital page load, but use infinite scrolling instead

However, keep in mind that the example implementation provided by Elixirland does not cover these features.
