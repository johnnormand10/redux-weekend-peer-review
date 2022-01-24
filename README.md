# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [] Able to add feedback
    - [] Data collected on individual pages & components
    - [] Click on next takes you to the next page in sequence
    - [] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [] Thank you page takes you back to the first view
    - [] Old Data is cleared on form completion

- Client code:
  - []  Individual components for each form part
  - []  Redux setup complete
    - [] Store linked to react with `<Provider>`
    - [] Store setup with reducer(s) and logger middleware 
  - [] Reducers & Actions Working
    - [] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [] Actions have a `type` key, and `payload` if sending data
    - [] Reducers are returning a new state, or the old state (not mutating)
    - [] Reducers are using spread correctly (to keep old data, while adding new)
  - [] Review Component shows at all times with current redux state
  - [] React-Redux Working
    - [] Dispatching actions onClick
    - [] Grabbing data from the redux store with `useSelector`
  - [] Axios POST request to add feedback


- Server code:   
  - [Yes] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [Yes] Multiple git commits showing incremental progress
  - [Yes] Commits are descriptive of the changes made or feature added 
  - [Yes] Has .gitignore with node_modules
  - [Yes] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [Yes] Appropriate amount of code comments
  - [Yes] Code is consistently formatted
- Client
  - [Yes] Appropriate use of HTML tags
  - [Yes] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [Yes] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [Yes] user can upate their score for a step
    - [Yes] new score is validated to not be empty
    - [Yes] redux is updated with new score
  - [Yes] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [Yes] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey Andre,

General Feedback.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | Yes |
| Data stored in Redux when navigating from page to page | Yes |
| User is notified when trying to leave a blank score | Yes |
| Review Component displays scores and comments from current redux state | Yes |
| Submit button sends data to the server via Axios | Yes |
| Confirmaion Page displays after data is POSTed to the server | Yes |
| Button on Confirmation Page clears Redux and starts a new survey | Yes |
| Views are broken down into components | Yes |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | Yes - 41 |
| Commits are descriptive of the changes made or feature added | Yes |
| Readme file updated | Yes |
| Appropriate amount of code comments | Yes |
| Code is consistently formatted | Yes |
| Server code organized with router & module files | Yes |

---
### Notes:

Notes on General Items

- Don't be afraid to add more comments around.
- Make sure you set a value to your useState(). Ex. useState(0) .... useState(null) .... useState('')
- Great work, keep it up!

```
