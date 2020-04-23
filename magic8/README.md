Take Home Interview Exercise
============================

This is the technical portion of your interview. Please read the following instructions very carefully.

## Instructions

Take a look at the following wireframe.

![Magic 8-Ball Wireframe](https://user-images.githubusercontent.com/4664162/78293614-5ee5ba00-7518-11ea-9a44-38ce7c9ad193.png)

We want you to make a simple web app that creates that interface.

1. The project must contain a README.md that details instructions on how to start the web app, and if necessary, how to compile any assets/dependencies.
1. You have 5 business days to complete this project.
1. You will be judged on code layout, consistency, style, error handling, testing, simplicity, and functionality.
1. Create your work in a private GitHub repository under your own account (they're free for personal accounts). Add @defionscode and @shepdelacreme as a collaborators when your submission is ready.
1. Your final work should be reflective of the type of work you would give your employer if they were to ask you the same requierments.
    1. The one caveat is when shortcuts are taken due to this being a homework assignment and not a real-world situation. When pragmatism dictates this to be the case, make sure to note it in the README.

### Backend (required)

1. The backend should be in either nodejs or in python3 depending on the position you've applied for. You are free to use any framework or lack thereof. No framework is preferred.

1. The development webserver should run on port 21337.

### Front End (required)

1. Can use any front end framework, but vanilla javascript, css, and html is preferred.
1. The html title should be "Magic Eight Ball"
1. Pick any color scheme you feel is proper.
1. The title header of the page should be "Magic 8-Ball" which should be centered horizontally.
1. There should be a single image of an eight-ball underneath the title header, also centered horizontally. The image should be sized to be similar to that of the wireframe.
1. Underneath the eight-ball image, there should be empty space that will later be filled with text.
1. Underneath the empty space there should be an input box with placeholder text that reads "Enter your yes/no question..."
1. Underneath the input box there will be a button that reads "Shake the Magic 8-ball". It should be wide enough to fit the text.
1. Underneath the button there should be a table that starts empty but has a column title of "History of Luck" as seen in the wireframe.
1. The table, the button, and the input box should all be the same width.

### UX (required)

1. When a user inputs a question and clicks "Shake the Magic 8-ball", a request should be made to the API at https://8ball.delegator.com/. You can see a sample response here: https://8ball.delegator.com/magic/JSON/Will%20I%20ever%20give%20you%20up%3F
1. The request can be made _either_ on the client or server side, it's your call.
1. If a user fails to supply a question, an alert should occur notifying the user of the missing input. No request should be made to the api if the input is empty.
1. Errors should be handled gracefully and not cause JavaScript tracebacks in the browser console nor on the server unless for intentional logging.
1. When the button is clicked, the input box should be cleared, but _only_ if there was no error.
1. The "answer" in the response should appear in the blank space between the input and the image of the 8 ball. When the response is rendered, the position of all elements in the page should remain static and not shift at all. 
1. The "type" of the answer should be placed in the table underneath the button.
1. When a new question is supplied, and the button is clicked, the "answer" text between the input and 8-ball image should be replaced with the new response and the "type" should be _appended_ to the table underneath the button.


## Delivery

When you are complete, create a git tag in the repository for `v1.0.0` and contact us to let us know you've finished. Remember, this is will be our first-impression as to how you work professionally. 

## Bonus Items (optional)

The following are **optional** but if implemented would make your application more competitive, implement some or all. It's up to you.

1. Persist the "History of Luck" between browser refreshes or if the browser is closed/opened.
1. Basic user accounts with an account needed in order to use the 8 ball
1. In the History of Luck table, "Affirmative" should be green, "Neutral" grey, and "Contrary" red.
1. Any other feature you'd like to show off.

## FAQ

1. Can I use <INSERT TECHNOLOGY> for <INSERT USE CASE>? Yes, of course. Though remember, we are asking you to as few dependencies as possible (zero is ideal). The exception are devDependencies, but we'd still prefer minimalism there.
1. Can I get an extension? Maybe. Contact me to discuss.
1. Why is vanilla JavaScript preferred? Frameworks come and go, and even the ones that stay (think React) don't do _everything_. Comfort and familiarity with native browser APIs should be a fundamental skill for seasoned front end developers.
1. Will messing up something cause me to be disqualified? Not necessarily, if we find issue in your code and it appears to be superficial in nature then it's probably fine. If the problems are indicative of an underlying deficiency in your current skill level (using blocking Node APIs in the server, for example) then it likely could. Generally speaking, unless you've provided truly awful code, we'll let you proceed. However, keep in mind that other candidates are likely to provide quality work. All-else-equal, we would opt for the candidate that provided a solution to this assignment that meets the requirements. In the case of multiple candidates satisfying core requirements, we'd then look to see who did any of the bonus items.
