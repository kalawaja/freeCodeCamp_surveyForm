# Learn HTML Forms by Building a Registration Form, Completed

> `Certification Project`
> ## Survey Form
> - This is one of the required projects to earn your certification.
> - For this project, you will build a survey form to collect data from your users.

> ### **Instructions**
> **Build a Survey Form** <br>
> <br>
> **Objective:** Build an app that is functionally similar to [Survey Form](https://survey-form.freecodecamp.rocks) <br>
> <br>
> **User Stories:**
> 1. You should have a page title in an `h1` element with an `id` of `title`
> 2. You should have a short explanation in a `p` element with an `id` of `description`
> 3. You should have a `form` element with an `id` of `survey-form`
> 4.  Inside the form element, you are **required** to enter your name in an `input` field that has an `id` of `name` and a `type` of `text`
> 5. Inside the form element, you are **required** to enter your email in an `input` field that has an `id` of `email`
> 6. If you enter an email that is not formatted correctly, you will see an HTML5 validation error
> 7. Inside the form, you can enter a number in an `input` field that has an `id` of `number`
> 8. If you enter non-numbers in the number input, you will see an HTML5 validation error
> 9. If you enter numbers outs`id`e the range of the number input, which are defined by the `min` and `max` attributes, you will see an HTML5 validation error
> 10. For the name, email, and number input fields, you can see corresponding `label` elements in the form, that describe the purpose of each field with the following ids:<br>
`id="name-label"`, `id="email-label"` and `id="number-label"`
> 11. For the name, email, and number input fields, you can see placeholder text that gives a description or instructions for each field
> 12. Inside the form element, you should have a `select` dropdown element with an `id` of `dropdown` and at least two options to choose from
> 13. Inside the form element, you can select an option from a group of at least two radio buttons that are grouped using the `name` attribute
> 14. Inside the form element, you can select several fields from a series of checkboxes, each of which must have a `value` attribute
> 15. Inside the form element, you are presented with a `textarea` for additional comments
> 16. Inside the form element, you are presented with a button with `id` of `submit` to submit all the inputs <br>

> Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding! <br>

> **Note:** Be sure to add ```<link rel="stylesheet" href="styles.css">``` in your HTML to link your stylesheet and apply your CSS <br>

---

> ## **Solutions** <br>
> **Follow Step by Step** <br><br>

> **Step 1** <br>
You should have a page title in an `h1` element with an `id` of `title`

```html
#index.html
        <h1 id="title" class="text-center">freeCodeCamp Survey Form</h1>
```
```css
#styles.css
h1 {
  font-weight: 400;
  line-height: 1.2;
}
```
> **Step 2** <br>
You should have a short explanation in a `p` element with an `id` of `description`

```html
#index.html
        <p id="description" class="description text-center">
          Thank you for taking the time to help us improve the platform
        </p>
```
```css
#styles.css
p {
  font-size: 1.125rem;
}
```
```css
#styles.css
.description {
  font-style: italic;
  font-weight: 200;
  text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.4);
}
```
```css
#styles.css
.text-center {
  text-align: center;
}
```
> **Step 3** <br>
You should have a `form` element with an `id` of `survey-form`

```html
#index.html
        <form id="survey-form">
        </form>
```
```css
#styles.css
form {
  background: var(--color-darkblue-alpha);
  padding: 2.5rem 0.625rem;
  border-radius: 0.25rem;
}
```
```css
#styles.css
@media (min-width: 480px) {
  form {
    padding: 2.5rem;
  }
}
```
> **Step 4** <br>
Inside the form element, you are **required** to enter your name in an `input` field that has an `id` of `name` and a `type` of `text`

```html
#index.html
        <form id="survey-form">
          <input id="name" type="text" required>Name
        </form>
```
> **Step 5** <br>
Inside the form element, you are `required` to enter your email in an `input` field that has an `id` of `email`

```html
#index.html
        <form id="survey-form">
          <input id="name" type="text" required>Name
          <input id="email" type="email" required>Email
        </form>
```
> **Step 6** <br>
If you enter an email that is not formatted correctly, you will see an HTML5 validation error

```html
#index.html
        <form id="survey-form">
          <input id="name" type="text" required>Name
          <input id="email" type="email" required>Email
        </form>
```
```css
#styles.css
@import url('https://fonts.googleapis.com/css?family=Poppins:200i,400&display=swap');
```
```css
#styles.css
h1,
p {
  margin-top: 0;
  margin-bottom: 0.5rem;
}
```
> **Step 7** <br>
Inside the form, you can enter a number in an `input` field that has an `id` of `number`

```html
#index.html
        <form id="survey-form">
          <input id="name" type="text" required>Name
          <input id="email" type="email" required>Email
          <input id="number" type="number">Age (optional)
        </form>
```
> **Step 8** <br>
If you enter non-numbers in the number input, you will see an HTML5 validation error

```html
#index.html
        <form id="survey-form">
          <input id="name" type="text" required>Name
          <input id="email" type="email" required>Email
          <input id="number" type="number">Age (optional)
        </form>
```
```css
#styles.css
body {
  font-family: 'Poppins', sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.4;
  color: var(--color-white);
  margin: 0;
}
```
> **Step 9** <br>
If you enter numbers outs`id`e the range of the number input, which are defined by the `min` and `max` attributes, you will see an HTML5 validation error

```html
#index.html
        <form id="survey-form">
          <input id="name" type="text" required>
          <input id="email" type="email" required>
          <input id="number" type="number" min="10" max="99">  
        </form>
```
> **Step 10** <br>
For the name, email, and number input fields, you can see corresponding `label` elements in the form, that describe the purpose of each field with the following ids:<br>
`id="name-label"`, `id="email-label"` and `id="number-label"`

```html
#index.html
        <form id="survey-form">
          <label id="name-label">Name</label>
            <input id="name" type="text" placeholder="Enter your name" required>
          <label id="email-label">Email</label>
            <input id="email" type="email" placeholder="Enter your Email" required>
          <label id="number-label">Age (optional)</label>
            <input id="number" type="number" placeholder="Age" min=10 max=99>
        </form>
```
```css
#styles.css
label {
  display: flex;
  align-items: center;
  font-size: 1.125rem;
  margin-bottom: 0.5rem;
}
```
> **Step 11** <br>
For the name, email, and number input fields, you can see placeholder text that gives a description or instructions for each field

```html
#index.html
        <form id="survey-form">
          <label id="name-label">Name</label>
            <input id="name" type="text" placeholder="Enter your name" required>
          <label id="email-label">Email</label>
            <input id="email" type="email" placeholder="Enter your Email" required>
          <label id="number-label">Age (optional)</label>
            <input id="number" type="number" placeholder="Age" min=10 max=99>
        </form>
```
```css
#styles.css
/* mobile friendly alternative to using background-attachment: fixed */
body::before {
  content: '';
  position: fixed;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  background: var(--color-darkblue);
  background-image: linear-gradient(
      115deg,
      rgba(58, 58, 158, 0.8),
      rgba(136, 136, 206, 0.7)
    ),
    url(https://cdn.freecodecamp.org/testable-projects-fcc/images/survey-form-background.jpeg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
```
> **Step 12** <br>
Inside the form element, you should have a `select` dropdown element with an `id` of `dropdown` and at least two options to choose from

```html
#index.html
          <p>Which option best describes your current role?</p>
          <select id="dropdown" name="role" class="form-control" required>
            <option disabled="" selected="" value="">Select current role</option>
            <option value="student">Student</option>
            <option value="job">Full Time Job</option>
            <option value="learner">Full Time Learner</option>
            <option value="preferNo">Prefer not to say</option>
            <option value="other">Other</option>
          </select>
```
```css
#styles.css
.form-control {
  display: block;
  width: 100%;
  height: 2.375rem;
  padding: 0.375rem 0.75rem;
  color: #495057;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ced4da;
  border-radius: 0.25rem;
  transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}
```
```css
#styles.css
.form-control:focus {
  border-color: #80bdff;
  outline: 0;
  box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
}
```
> **Step 13** <br>
Inside the form element, you can select an option from a group of at least two radio buttons that are grouped using the `name` attribute

```html
#index.html
          <p>Would you recommend freeCodeCamp to a friend?</p>
          <label>
            <input
              name="user-recommend"
              value="definitely"
              type="radio"
              class="input-radio"
              checked/>Definitely
          </label>
          <label>
            <input
              name="user-recommend"
              value="maybe"
              type="radio"
              class="input-radio"/>Maybe
          </label>
          <label>
            <input
              name="user-recommend"
              value="not-sure"
              type="radio"
              class="input-radio"/>Not sure
          </label>
```
> **Step 14** <br>
Inside the form element, you can select several fields from a series of checkboxes, each of which must have a `value` attribute

```html
#index.html
          <p>What would you like to see improved?
            <span class="clue">(Check all that apply)</span>
          </p>
          <label>
            <input
              name="prefer"
              value="front-end-projects"
              type="checkbox"
              class="input-checkbox"/>Front-end Projects
          </label>
          <label>
            <input
              name="prefer"
              value="back-end-projects"
              type="checkbox"
              class="input-checkbox"/>Back-end Projects
          </label>
          <label>
            <input
              name="prefer"
              value="data-visualization"
              type="checkbox"
              class="input-checkbox"/>Data Visualization
          </label>
          <label>
            <input
              name="prefer"
              value="challenges"
              type="checkbox"
              class="input-checkbox"/>Challenges
          </label>
          <label>
            <input
              name="prefer"
              value="open-source-community"
              type="checkbox"
              class="input-checkbox"/>Open Source Community
          </label>
          <label>
            <input
              name="prefer"
              value="gitter-help-rooms"
              type="checkbox"
              class="input-checkbox"/>Gitter help rooms
          </label>
          <label>
            <input
              name="prefer"
              value="videos"
              type="checkbox"
              class="input-checkbox"/>Videos
          </label>
          <label>
            <input
              name="prefer"
              value="city-meetups"
              type="checkbox"
              class="input-checkbox"/>City Meetups
          </label>
          <label>
            <input
              name="prefer"
              value="wiki"
              type="checkbox"
              class="input-checkbox"/>Wiki
          </label>
          <label>
            <input
              name="prefer"
              value="forum"
              type="checkbox"
              class="input-checkbox"/>Forum
          </label>
          <label>
            <input
              name="prefer"
              value="additional-courses"
              type="checkbox"
              class="input-checkbox"/>Additional Courses
          </label>
```
```css
#styles.css
.clue {
  margin-left: 0.25rem;
  font-size: 0.9rem;
  color: #e4e4e4;
}
```
```css
#styles.css
.input-radio,
.input-checkbox {
  display: inline-block;
  margin-right: 0.625rem;
  min-height: 1.25rem;
  min-width: 1.25rem;
}
```
> **Step 15** <br>
Inside the form element, you are presented with a `textarea` for additional comments

```html
#index.html
          <p>Any comments or suggestions?</p>
          <textarea
            id="comments"
            class="input-textarea"
            name="comment"
            placeholder="Enter your comment here...">
          </textarea>
```
```css
#styles.css
.input-textarea {
  min-height: 120px;
  width: 100%;
  padding: 0.625rem;
  resize: vertical;
}
```
> **Step 16** <br>
Inside the form element, you are presented with a button with `id` of `submit` to submit all the inputs

```html
#index.html
          <button type="submit" id="submit" class="submit-button">Submit
          </button>
```
```css
#styles.css
button {
    border: none;
}
```
```css
#styles.css
input,
button,
select,
textarea {
  margin: 0;
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
```
```css
#styles.css
.submit-button {
  display: block;
  width: 100%;
  padding: 0.75rem;
  background: var(--color-green);
  color: inherit;
  border-radius: 2px;
  cursor: pointer;
}
```
> <br>
> Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding! <br>
> <br>

> **Note:** Be sure to add ```<link rel="stylesheet" href="styles.css">``` in your HTML to link your stylesheet and apply your CSS <br>
> <br>

```html
#index.html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css"/>
  </head>
  <body>
    <div class="container">
      <header class="header">
        <h1 id="title" class="text-center">freeCodeCamp Survey Form</h1>
        <p id="description" class="description text-center">
          Thank you for taking the time to help us improve the platform
        </p>
      </header>
      <form id="survey-form">
        <div class="form-group">
          <label id="name-label" for="name">Name</label>
          <input
            type="text"
            name="name"
            id="name"
            class="form-control"
            placeholder="Enter your name"
            required/>
        </div>
        <div class="form-group">
          <label id="email-label" for="email">Email</label>
          <input
            type="email"
            name="email"
            id="email"
            class="form-control"
            placeholder="Enter your Email"
            required/>
        </div>
        <div class="form-group">
          <label id="number-label" for="number">Age
            <span class="clue">(optional)</span>
          </label>
          <input
            type="number"
            name="age"
            id="number"
            min="10"
            max="99"
            class="form-control"
            placeholder="Age"/>
        </div>
        <div class="form-group">
          <p>Which option best describes your current role?</p>
          <select id="dropdown" name="role" class="form-control" required>
            <option disabled selected value>Select current role</option>
            <option value="student">Student</option>
            <option value="job">Full Time Job</option>
            <option value="learner">Full Time Learner</option>
            <option value="preferNo">Prefer not to say</option>
            <option value="other">Other</option>
          </select>
        </div>
        <div class="form-group">
          <p>Would you recommend freeCodeCamp to a friend?</p>
          <label>
            <input
              name="user-recommend"
              value="definitely"
              type="radio"
              class="input-radio"
              checked/>Definitely
          </label>
          <label>
            <input
              name="user-recommend"
              value="maybe"
              type="radio"
              class="input-radio"/>Maybe
          </label>
          <label>
            <input
              name="user-recommend"
              value="not-sure"
              type="radio"
              class="input-radio"/>Not sure
          </label>
        </div>
        <div class="form-group">
          <p>What is your favorite feature of freeCodeCamp?</p>
          <select id="most-like" name="mostLike" class="form-control" required>
            <option disabled="" selected="" value="">Select an option</option>
            <option value="challenges">Challenges</option>
            <option value="projects">Projects</option>
            <option value="community">Community</option>
            <option value="openSource">Open Source</option>
          </select>
        </div>
        <div class="form-group">
          <p>What would you like to see improved?
            <span class="clue">(Check all that apply)</span>
          </p>
          <label>
            <input
              name="prefer"
              value="front-end-projects"
              type="checkbox"
              class="input-checkbox"/>Front-end Projects
          </label>
          <label>
            <input
              name="prefer"
              value="back-end-projects"
              type="checkbox"
              class="input-checkbox"/>Back-end Projects
          </label>
          <label>
            <input
              name="prefer"
              value="data-visualization"
              type="checkbox"
              class="input-checkbox"/>Data Visualization
          </label>
          <label>
            <input
              name="prefer"
              value="challenges"
              type="checkbox"
              class="input-checkbox"/>Challenges
          </label>
          <label>
            <input
              name="prefer"
              value="open-source-community"
              type="checkbox"
              class="input-checkbox"/>Open Source Community
          </label>
          <label>
            <input
              name="prefer"
              value="gitter-help-rooms"
              type="checkbox"
              class="input-checkbox"/>Gitter help rooms
          </label>
          <label>
            <input
              name="prefer"
              value="videos"
              type="checkbox"
              class="input-checkbox"/>Videos
          </label>
          <label>
            <input
              name="prefer"
              value="city-meetups"
              type="checkbox"
              class="input-checkbox"/>City Meetups
          </label>
          <label>
            <input
              name="prefer"
              value="wiki"
              type="checkbox"
              class="input-checkbox"/>Wiki
          </label>
          <label>
            <input
              name="prefer"
              value="forum"
              type="checkbox"
              class="input-checkbox"/>Forum
          </label>
          <label>
            <input
              name="prefer"
              value="additional-courses"
              type="checkbox"
              class="input-checkbox"/>Additional Courses
          </label>
        </div>
        <div class="form-group">
          <p>Any comments or suggestions?</p>
          <textarea
            id="comments"
            class="input-textarea"
            name="comment"
            placeholder="Enter your comment here...">
          </textarea>
        </div>
        <div class="form-group">
          <button type="submit" id="submit" class="submit-button">Submit
          </button>
        </div>
      </form>
    </div>
  </body>
</html>
```
```css
#styles.css
:root {
  --color-white: #f3f3f3;
  --color-darkblue: #1b1b32;
  --color-darkblue-alpha: rgba(27, 27, 50, 0.8);
  --color-green: #37af65;
}
```
```css
#styles.css
.container {
  width: 100%;
  margin: 3.125rem auto 0 auto;
}
```
```css
#styles.css
@media (min-width: 576px) {
  .container {
    max-width: 540px;
  }
}
```
```css
#styles.css
@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}
```
```css
#styles.css
.header {
  padding: 0 0.625rem;
  margin-bottom: 1.875rem;
}
```
```css
#styles.css
.form-group {
  margin: 0 auto 1.25rem auto;
  padding: 0.25rem;
}
```
```css
#styles.css
*,
*::before,
*::after {
  box-sizing: border-box;
}
```
