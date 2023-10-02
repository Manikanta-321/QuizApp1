# Quiz Application with HTML, CSS, and JavaScript 




 
## Project Introduction
Welcome to the Quiz Application!
Quiz applications are a fantastic way to engage and entertain users on websites. Whether you want to test knowledge, provide educational content, or simply offer a fun activity, building a quiz application using HTML, CSS, and JavaScript is an excellent choice.

   We will start by setting up the HTML structure, where we'll define the layout and elements required for the quiz. Then, we'll move on to designing the user interface using CSS, making the application visually appealing and engaging.Next, we'll dive into the JavaScript implementation, where we'll handle the logic behind displaying questions, capturing user responses, and calculating the score. JavaScript will be the backbone of our quiz application, allowing us to dynamically generate content, validate user inputs, and provide interactive feedback.

## Technologies used

HTML: The foundation of the application's structure and content.

CSS: Responsible for the application's stylish and responsive design.

JavaScript: Powers the interactive elements, such as quiz questions and real-time scoring.

## Steps



### Step 1 (HTML Code):

To get started, we will first need to create a basic HTML file. In this file, we will include the main structure for our quiz application.


After creating the files just paste the following codes into your file. Make sure to save your HTML document with a .html extension, so that it can be properly viewed in a web browser.


Here is an explanation of each element:


### <!DOCTYPE html>: 
This is a declaration that specifies the HTML version being used, in this case, HTML5.


### <html>: 
The root element of an HTML document. It encapsulates all other elements on the page.


### <head>: 
This element contains metadata and other information about the web page that is not directly displayed on the page itself.


### <title>: 
This element sets the title of the web page, which appears in the browser's title bar or tab.


### <link rel="stylesheet" href="quiz.css">: 
This line links an external CSS stylesheet file named "styles.css" to the HTML document. It is used to apply styles to the elements on the page.


### <body>: 
The main content of the web page is placed within this element.


### <div class="container">: 
This <div> element acts as a container for grouping and organizing other elements.


### <h1>Quiz App</h1>: 
This <h1> heading element displays the text "Quiz App" as the main heading of the web page.


### <div id="quiz"></div>: 
This <div> element with the id attribute "quiz" will serve as a placeholder for dynamically generated quiz questions.


### <div id="result" class="result"></div>: 
This <div> element with the id attribute "result" and class attribute "result" will be used to display the quiz result.


### <button id="submit" class="button">Submit</button>:
 This <button> element with the id attribute "submit" and class attribute "button" represents a button labeled "Submit." Users can click this button to submit their quiz answers.


### <button id="retry" class="button hide">Retry</button>: 
This <button> element with the id attribute "retry" and class attribute "button hide" represents a button labeled "Retry." It is initially hidden (hide class), and will be displayed when the user wants to retry the quiz.


### <button id="showAnswer" class="button hide">Show Answer</button>: 
This <button> element with the id attribute "showAnswer" and class attribute "button hide" represents a button labeled "Show Answer." It is initially hidden (hide class), and will be displayed to allow users to see the correct answers.


### <script src="quiz.js"></script>: 
This line includes an external JavaScript file named "script.js" that contains the logic and functionality for the quiz app. The JavaScript code will be executed when the browser encounters this script tag.

   
### Step 2 (CSS Code):

Once the basic HTML structure of the quiz application is in place, the next step is to add styling to the quiz application using CSS.


Next, we will create our CSS file. In this file, we will use some basic CSS rules to create our quiz application.

### 1. @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;700&display=swap');: 
This line imports the Poppins font from Google Fonts, with different font weights (400, 500, and 700). The display=swap ensures that the text is displayed using fallback fonts until the Poppins font is fully loaded.


### 2. body: 
This selector targets the element of the HTML document. It sets the following properties:


### font-family: 'Poppins', sans-serif;: 
It specifies the font family for the entire body text, using Poppins as the preferred font. If Poppins is not available, it falls back to the generic sans-serif font.
background: #b9b3a9;: It sets the background color of the body to a light grayish-brown color (#b9b3a9).
#### display: flex;: 
It makes the body a flex container.
justify-content: center;: It horizontally centers the flex items (content) within the body.

### 3. .container: 
This selector targets an element with the class "container". It sets the following properties:


### width: 450px;: 
It sets the width of the container to 450 pixels.
### padding: 20px;: 
It adds 20 pixels of padding around the content of the container.
### margin-top: 80px;: 
It creates a top margin of 80 pixels for the container.
### background-color: #ff6600; 
It sets the background color of the container to white (#fff).
box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);: It applies a box shadow to the container, creating a subtle shadow effect.
border-radius: 20px;: It adds rounded corners to the container, with a border radius of 20 pixels.

### 4. h1: 
This selector targets all <h1> elements. It sets the following property:


### text-align: center;: 
It aligns the text within the <h1> element to the center.

### 5. .question: 
This selector targets an element with the class "question". It sets the following properties:


### font-weight: bold;: 
It makes the text within the element bold.
margin-bottom: 10px;: It adds a bottom margin of 10 pixels to the element.

### 6. .options: 
This selector targets an element with the class "options". It sets the following property:


### margin-bottom: 20px;: 
It adds a bottom margin of 20 pixels to the element.

### 7. .option: 
This selector targets an element with the class "option". It sets the following property:


### display: block;: 
It makes the element a block-level element, causing it to take up the full width available.

### 8. .button: 
This selector targets an element with the class "button". It sets the following properties:


### display: inline-block;: 
It makes the element an inline block.
### padding: 10px 20px;: 
It adds 10 pixels of padding on the top and bottom and 20 pixels of padding on the left and right.
### background-color: #428bca;: 
It sets the background color of the button to a shade of blue (#428bca).
### color: #fff;: 
It sets the text color of the button to white (#fff).
### border: none;: 
It removes the border around the button.
### cursor: pointer;: 
It changes the cursor to a pointer when hovering over the button.
### font-size: 16px;: 
It sets the font size of the button text to 16 pixels.
### border-radius: 4px;: 
It adds rounded corners to the button, with a border radius of 4 pixels.
### transition: background-color 0.3s;: 
It adds a transition effect to the background color property, with a duration of 0.3 seconds.
### margin-right: 10px;: 
It adds a right margin of 10 pixels to the button.

### 9. .button:hover: 
This selector targets the button when it is being hovered over. It sets the following property:


### background-color: #fff;: 
It changes the background color of the button to a darker shade of white when hovered.

### color:#0000cd;:
It changes the color of the font while hovered.

### cursor: pointer;:
Cursor becomes the pointer when hovered over it.

### 10. .result: 
This selector targets an element with the class "result". It sets the following properties:


### text-align: center;: 
It aligns the text within the element to the center.
#### margin-top: 20px;: 
It adds a top margin of 20 pixels to the element.
### font-weight: bold;: 
It makes the text within the element bold.

### 11. .hide: 
This selector targets an element with the class "hide". It sets the following property:


### display: none;: 
It hides the element by setting its display property to "none".

### 12. .option:hover:

### color:#fff;:
It changes the color of the font to white while hovered.

### cursor: pointer;:
Cursor becomes the pointer when hovered over it.

### Step 3 (JavaScript Code):

Finally, we need to create a function in JavaScript to sets up a simple quiz game. Let's go through the code step by step:


The code defines an array called quizData that contains multiple objects. Each object represents a question in the quiz and has properties such as question (the question itself), options (an array of answer options), and answer (the correct answer).


The code then defines variables to store references to various elements in the HTML document, such as the quizContainer, resultContainer, submitButton, retryButton, and showAnswerButton. These elements are identified using their respective IDs.


Two variables, currentQuestion and score, are initialized to keep track of the current question being displayed and the player's score, respectively. Additionally, an array called incorrectAnswers is created to store any incorrect answers provided by the player.


The code includes a function called shuffleArray, which takes an array as input and shuffles its elements randomly. This function is used to randomize the order of answer options for each question.


The displayQuestion function is defined to render the current question and its answer options on the page. It retrieves the question data from the quizData array based on the currentQuestion index. It creates HTML elements dynamically to display the question and options, and appends them to the quizContainer.


The checkAnswer function is responsible for validating the player's answer. It retrieves the selected option using a CSS selector, checks if an option is selected, compares the selected answer with the correct answer from quizData, and increments the score or adds the question to the incorrectAnswers array accordingly. It then updates the currentQuestion index, clears the selected option, and either displays the next question or the result if there are no more questions.


The displayResult function is called when all the questions have been answered. It hides the quiz container and submit button, and shows the retry and show answer buttons. It displays the player's score and the number of questions in the resultContainer.


The retryQuiz function is called when the player clicks the retry button. It resets the currentQuestion, score, and incorrectAnswers to their initial values, displays the quiz container and submit button, and hides the retry and show answer buttons. It also clears the result container and calls displayQuestion to start the quiz again.


The showAnswer function is called when the player clicks the show answer button. It hides the quiz container, submit button, and show answer button. It generates HTML to display the player's score and lists all the incorrect answers with the corresponding correct answers.


Event listeners are attached to the submit, retry, and show answer buttons, which call their respective functions when clicked.


Finally, the displayQuestion function is called initially to start the quiz by displaying the first question.

## Conclusion

In conclusion, the Quiz Application offers an engaging and educational experience for users of all backgrounds and interests. With its user-friendly interface, customizable quizzes, and interactive questions, it provides a platform to challenge your knowledge, learn new facts, and have fun while doing so.

