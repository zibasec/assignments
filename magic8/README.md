Take Home Interview Exercise
============================

This is the technical portion of your interview. Please read the following instructions very carefully.

## Instructions

Take a look at the following wireframe.

![Magic 8-Ball Wireframe](https://user-images.githubusercontent.com/4664162/78293614-5ee5ba00-7518-11ea-9a44-38ce7c9ad193.png)

We want you to make a simple web app that creates that interface. You will be judged on code layout, consistency, style, error handling, testing, simplicity, and functionality.

Your final work should be reflective of the type of work you would give your employer if they were to ask you the same requierments.

### Repository

1. The project must contain a README.md that details instructions on how to start the web app, and if necessary, how to compile any assets/dependencies.

### Backend

1. The backend should be in either nodejs or in python3 depending on the position you've applied for. You are free to use any framework or lack thereof. No framework is preferred.

1. The development webserver should run on port 21337.

### Front End

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

### UX

1. When a user inputs a question and clicks "Shake the Magic 8-ball", a request should be made to the API at https://8ball.delegator.com/. You can see a sample response here: https://8ball.delegator.com/magic/JSON/Will%20I%20ever%20give%20you%20up%3F
1. The request can be made _either_ on the client or server side, it's your call.
1. If a user fails to supply a question, an alert should occur notifying the user of the missing input. No request should be made to the api if the input is empty.
1. Errors should be handled gracefully and not cause JavaScript tracebacks in the browser console nor on the server unless for intentional logging.
1. When the button is clicked, the input box should be cleared, but _only_ if there was no error.
1. The "answer" in the response should appear in the blank space between the input and the image of the 8 ball. When the response is rendered, the position of all elements in the page should remain static and not shift at all.
1. The "type" of the answer should be placed in the table underneath the button.
1. When a new question is supplied, and the button is clicked, the "answer" text between the input and 8-ball image should be replaced with the new response and the "type" should be _appended_ to the table underneath the button.

## Bonus Items (optional)

The following are **optional** but if implemented would make your application more competitive, implement some or all. It's up to you.

1. Persist the "History of Luck" between browser refreshes or if the browser is closed/opened.
1. Basic user accounts with an account needed in order to use the 8 ball
1. In the History of Luck table, "Affirmative" should be green, "Neutral" grey, and "Contrary" red.
1. Any other feature you'd like to show off.

## Delivery

Find instructions for [submitting your homework here](https://github.com/zibasec-recruiting/assignments#submission).
