<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Student registration form">
  <title>Student Registration</title>
</head>

<body>
  <h1>Student Registration Form</h1>
  <form>
    Full name:<input type="text" name="name" placeholder="your name"><br><br>
    Email:<input type="email" name="email" placeholder="your email"><br><br>
    Phone no:<input type="tel" name="phone" pattern="[0-9]{10}" placeholder="10 digits"><br><br>
    Password:<input type="password" name="password" minlength="8" required>
  <h4>Select your Gender</h4>
    <input type="radio" name="gender" value="male"> Male
    <input type="radio" name="gender" value="female"> Female
    <input type="radio" name="gender" value="other"> Other
  <h4>Choose your Course</h4>
    Course: <select name="course">
        <option value="">-- Select --</option>
        <option>B.Tech CSE</option>
        <option>BCA-AI</option>
        <option>B.Sc</option>
      </select>
    <p>
      <input type="checkbox" name="terms" required> I agree to the terms and conditions.
    </p>
    <button type="submit">Register</button>
    <button type="reset">Clear</button>
  </form>
</body>

</html>
