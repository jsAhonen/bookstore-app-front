# Bookstore App

This project will be a series of experiments with different software development technologies using a simple bookstore application as the basis for implementation of these technologies.

## Structure of the Project

The project will include frontend and backend projects separately, and each of these will have their respective implementations of the bookstore app design.

Each technology stack will have its own branch.

## Design

### User personas
* User: a book lover who wants to place some orders.
* Admin: a person who maintains the system.

### User Stories – User
* U1: As a user, I want to create an account so that I can order books.
* U2: As a user, I want to log in to my account so that I can start a session for ordering books.
* U3: As a user, I want to renew my forgotten or lost password, so that I can continue ordering books with my existing account even when I have lost or forgotten my password.
* U4: As a user, I want to view a list of most recently published books that fit my interests so that I can easily find out what titles there are to be bought in the fields of my interest.
* U5: As a user, I want to search books by title, author, category, price or description content, so that I can quickly find books that interest me.
* U6: As a user, I want to view a single book with its cover, description, technical details, preview and reviews so that I can know as much as possible about the book before I make my decision to buy it.
* U7: As a user, I want collect the books into a shopping cart before I place an order, so that I can freely shop around and make a batch of purchases before I proceed to the "bureaucracy" of placing the order.
* U8: As a user, I want to place the order by giving the specifications about how the order should be shipped, where, and which payment method should be used so that I can pay for the books I want to buy have them delivered to me.
* U9: As a user, I want to be able to give one review per books that I have demonstrably purchased so that others could learn from my own experiences about the book and have more information to decide by whether they are interested in the book or not.
* U10: As a user, I want to have a contact form so that I can send messages with questions, suggestions, feedback and whatever I need to inform the administrators.

### User Stories – Admin
* A1: As an admin, I want to log in and change my password, so that I can authenticate as an admin to administer this service.
* A2: As an admin, I want to create a book, so that it can be found and bought in the service.
* A3: As an admin, I want to update a book, so that I can fix and update any information that needs to be changed.
* A4: As an admin, I want to delete a book, so that I can manually remove an item in the store whenever it is needed.
* A5 As an admin, I want to view the list of users sorted by last names, so that I can browse the user information to find users.
* A6: As an admin, I want to search for users by first and last names and user ids, so that I can quickly find a user whose information I need at the moment.
* A7: As an admin, I want to delete a user so that I can block an unwanted user from using the service.
* A8: As an admin, I want to view error logs that have been generated by the service so that I know whenever there is something to be fixed in the service.
* A9: As an admin, I want to have an inbox where I receive messages from users, so that I can receive feedback from customers and reply to their messages.

### UI Views

#### User
* U1: Register form
* U2: Login form
* U3: Renew Password form
* U4: List and Search View
* U5: Search field and filter bar in List and Search View
* U6: Book Details
* U7
    * Add to shopping cart button in List and Search View (book item row or card) 
    * Add to shopping cart button in Book Details view, 
    * Shopping cart button and badge on the top bar, 
    * Shopping cart dropdown when top bar shopping cart button is hovered, 
    * Shopping Cart View when the shopping cart button is clicked.
* U8: Place order view, divided into steps with a stepper and Next/Previous buttons
* U9: Add review form, enabled if the user is logged in and has not yet given a review on the book
* U10: Contact form as a user view available when the user has logged in.

#### Admin
* A1
    * Login form
    * Renew password form
* A2
    * Create book button that leads to the create book form view
    * Create book form
* A3
    * List and Search Books view
    * Update book form (based on create book form)
* A4
    * List and Search Books view
    * Delete button in the update book form.
    * Delete button in the List and Search books view.
* A5 List and Search Users View
* A6: Search field in the List and Search Users View
* A7
    * User details
    * Delete button in User details
    * "Are you sure?" pop up window for confirming the choice and preventing accidental deletions
* A8
    * Deterine whether it makes sense to implement a separate view
    * Is an inbox message enough?
    * Depending on the environment, this can be implemented as a cloud service.
* A9: Inbox view
