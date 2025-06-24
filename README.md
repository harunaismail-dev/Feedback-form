
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Student Feedback Form</title>
  <style>
    body {
      background: linear-gradient(to right, #00b09b, #96c93d);
      font-family: 'Segoe UI', sans-serif;
      color: #fff;
      padding: 40px;
      margin: 0;
    }

    .form-container, .thank-you-message {
      max-width: 600px;
      margin: auto;
      background: rgba(0, 0, 0, 0.2);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
    }

    h1 {
      text-align: center;
      margin-bottom: 20px;
    }

    fieldset {
      border: none;
      margin-bottom: 20px;
    }

    legend {
      font-size: 1.2em;
      font-weight: bold;
      margin-bottom: 10px;
    }

    label {
      display: block;
      margin: 10px 0 5px;
    }

    input[type="text"],
    input[type="email"],
    textarea {
      width: 100%;
      padding: 10px;
      border: none;
      border-radius: 8px;
      margin-bottom: 10px;
    }

    input[type="radio"],
    input[type="checkbox"] {
      margin-right: 8px;
    }

    button {
      background-color: #004d00;
      color: white;
      padding: 12px 20px;
      font-size: 1em;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      width: 100%;
      transition: background 0.3s ease;
    }

    button:hover {
      background-color: #006600;
    }

    .thank-you-message {
      display: none;
      text-align: center;
    }

    .thank-you-message h2 {
      font-size: 2em;
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

  <div class="form-container" id="formContainer">
    <h1>Student Feedback</h1>
    <form id="feedbackForm">
      <!-- Personal Info -->
      <fieldset>
        <legend>Personal Information</legend>
        <label for="name">Full Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email Address:</label>
        <input type="email" id="email" name="email" required>
      </fieldset>

      <!-- Course Experience -->
      <fieldset>
        <legend>Course Experience</legend>

        <label>Rate the course:</label>
        <label><input type="radio" name="rating" value="Excellent" required> Excellent</label>
        <label><input type="radio" name="rating" value="Good"> Good</label>
        <label><input type="radio" name="rating" value="Average"> Average</label>
        <label><input type="radio" name="rating" value="Poor"> Poor</label>

        <label>What did you find helpful?</label>
        <label><input type="checkbox" name="useful" value="Lectures"> Lectures</label>
        <label><input type="checkbox" name="useful" value="Assignments"> Assignments</label>
        <label><input type="checkbox" name="useful" value="Projects"> Projects</label>
        <label><input type="checkbox" name="useful" value="Discussions"> Discussions</label>
      </fieldset>

      <!-- Comments -->
      <fieldset>
        <legend>Additional Comments</legend>
        <textarea name="comments" rows="5" placeholder="Enter your feedback here..."></textarea>
      </fieldset>

      <!-- Submit -->
      <button type="submit">Submit Feedback</button>
    </form>
  </div>

  <div class="thank-you-message" id="thankYouMessage">
    <h2>Thank you for your feedback!</h2>
    <p>Redirecting you shortly...</p>
  </div>

  <script>
    document.getElementById("feedbackForm").addEventListener("submit", function(e) {
      e.preventDefault(); // prevent real form submit

      // Hide form and show thank-you message
      document.getElementById("formContainer").style.display = "none";
      document.getElementById("thankYouMessage").style.display = "block";

      // Redirect to download link after 3 seconds
      setTimeout(function() {
        window.location.href = "https://example.com/download"; // Replace with your link
      }, 3000);
    });
  </script>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Student Feedback Form</title>
  <style>
    body {
      background: linear-gradient(to right, #00b09b, #96c93d);
      font-family: 'Segoe UI', sans-serif;
      color: #fff;
      padding: 40px;
      margin: 0;
    }

    .form-container, .thank-you-message {
      max-width: 600px;
      margin: auto;
      background: rgba(0, 0, 0, 0.2);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
    }

    h1 {
      text-align: center;
      margin-bottom: 20px;
    }

    fieldset {
      border: none;
      margin-bottom: 20px;
    }

    legend {
      font-size: 1.2em;
      font-weight: bold;
      margin-bottom: 10px;
    }

    label {
      display: block;
      margin: 10px 0 5px;
    }

    input[type="text"],
    input[type="email"],
    textarea {
      width: 100%;
      padding: 10px;
      border: none;
      border-radius: 8px;
      margin-bottom: 10px;
    }

    input[type="radio"],
    input[type="checkbox"] {
      margin-right: 8px;
    }

    button {
      background-color: #004d00;
      color: white;
      padding: 12px 20px;
      font-size: 1em;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      width: 100%;
      transition: background 0.3s ease;
    }

    button:hover {
      background-color: #006600;
    }

    .thank-you-message {
      display: none;
      text-align: center;
    }

    .thank-you-message h2 {
      font-size: 2em;
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

  <div class="form-container" id="formContainer">
    <h1>Student Feedback</h1>
    <form id="feedbackForm">
      <!-- Personal Info -->
      <fieldset>
        <legend>Personal Information</legend>
        <label for="name">Full Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email Address:</label>
        <input type="email" id="email" name="email" required>
      </fieldset>

      <!-- Course Experience -->
