# HTML-FORMS
HTMLS AND CSS CODES FOR HTML FORMS
body {
  width: 100%;
  height: 100vh;
  margin: 0;
  background-color: #1b1b32;
	color: #f5f6f7;
  font-family: Tahoma;
	font-size: 16px;
}
h1, p {
  margin: 1em auto;
  text-align: center;
}
form {
  width: 60vw;
	max-width: 500px;
	min-width: 300px;
	margin: 0 auto;
  padding-bottom: 2em;
}
fieldset {
  border: none;
	padding: 2rem 0;
}
fieldset:not(:last-of-type) {
  border-bottom: 3px solid #3b3b4f;
}
label {
  display: block;
	margin: 0.5rem 0;
}
input,
textarea,
select {
  margin: 10px 0 0 0;
	width: 100%;
  min-height: 2em;
}
input,
textarea,
select {
  margin: 10px 0 0 0;
	width: 100%;
  min-height: 2em;
}
input, textarea {
  background-color: #0a0a23;
  border: 1px solid #0a0a23;
  color: #ffffff;
}

.inline {
  width: unset;
  margin: 0 0.5em 0 0;
  vertical-align: middle;
}

input[type="submit"] {
  display: block;
  width: 60%;
  margin: 1em auto;
  height: 2em;
  font-size: 1.1rem;
  background-color: #3b3b4f;
  border-color: white;
  min-width: 300px;
}

input[type="file"] {
  padding: 1px 2px;
}
a{
  color: #dfdfe2;
}
<!DOCTYPE html>
<html>
  <head>
    <title>freeCodeCamp Registration Form Project</title>
	  <link rel="stylesheet" type="text/css" href="styles.css" />
  </head>
 <body>
    <h1>Registration Form</h1>
    <p>Please fill out this form with the required information</p>
    <form action='https://fcc-registration-form.com'>
      <fieldset>
        <label>Enter Your First Name: <input type="text" name="first-name" required /></label>
        <label>Enter Your Last Name: <input type="text" name="last-name" required /></label>
        <label>Enter Your Email: <input type="email" name="email" required /></label>
        <label>Create a New Password: <input type="password" name="password" pattern="[a-z0-5]{8,}" required /></label>
      </fieldset>
	    
 <fieldset>
        <label><input type="radio" name="account-type" class="inline" /> Personal Account</label>
        <label><input type="radio" name="account-type" class="inline" /> Business Account</label>
        <label>
          <input type="checkbox" name="terms" class="inline" required /> I accept the <a href="https://www.freecodecamp.org/news/terms-of-service/">terms and conditions</a>
			  </label>
      </fieldset>
 <fieldset>
        <label>Upload a profile picture: <input type="file" name="file" /></label>
        <label>Input your age (years): <input type="number" name="age" min="13" max="120" />
			  </label>
        <label>How did you hear about us?
          <select name="referrer">
            <option value="">(select one)</option>
            <option value="1">freeCodeCamp News</option>
            <option value="2">freeCodeCamp YouTube Channel</option>
            <option value="3">freeCodeCamp Forum</option>
            <option value="4">Other</option>
          </select>
        </label>
        <label>Provide a bio:
          <textarea name="bio" rows="3" cols="30" placeholder="I like coding on the beach..."></textarea>
			  </label>
      </fieldset>
	    
   <input type="submit" value="Submit" />
    </form>
  </body>
</html>
















