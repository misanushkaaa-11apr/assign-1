<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Job application form">
  <title>Job Application</title>
</head>

<body>
  <h1>Job Application – Front-End Developer</h1>
  <form>
    <h3>Personal details:-</h3>
    Full name: <input type="text" name="name" placeholder="enter your name"><br><br>
    Email: <input type="email" name="email" placeholder="your your email"><br><br>
    Phone no:<input type="tel" name="phone" pattern="[0-9]{10}" placeholder="10 digits"><br><br>
    Date of birth: <input type="date" name="dob"><br><br>
    Portfolio URL: <input type="url" name="website" placeholder="https://"><br><br>
    Create password <input type="password" name="password" minlength="8"><br><br>

    <hr>

    <h3>Job details:-</h3>
      Position: <select name="course">
        <option value="">-- Select --</option>
        <option>Front-End Developer</option>
        <option>UI Designer</option>
        <option>QA Tester</option>
      </select><br><br>
      Earliest joining date: <input type="date" name="join"><br><br>
      Interview slot: <input type="datetime-local" name="slot"><br><br>
      Preferred start month: <input type="month" name="month"><br><br>
      Preferred week: <input type="week" name="week"><br><br>
      Best call time: <input type="time" name="time"><br><br>
      Years of experience: <input type="number" name="exp" min="0" max="40"
            value="0"><br><br>
      Expected salary: (₹ LPA) <input type="range"  name="salary" min="2" max="30" value="6"
            oninput="out.value=this.value"> <output id="out">6</output><br><br>
      Favourite colour: <input type="color" name="colour" value="#3366ff"><br><br>
      Skills: (type or pick)
          <input list="skills" name="skill">
          <datalist id="skills">
          <option value="HTML"></option>
            <option value="CSS"></option>
            <option value="JavaScript"></option>
            <option value="Git"></option>
          </datalist><br><br>
    
    <hr>

    <h3>Work mode:-</h3>
      <input type="radio" name="mode" value="onsite" checked> On-site
      <input type="radio" name="mode" value="remote"> Remote
      <input type="radio" name="mode" value="hybrid"> Hybrid

    <hr>

    <h3>Technologies known:-</h3>
      <input type="checkbox"  value="html"> HTML
      <input type="checkbox"  value="css"> CSS
      <input type="checkbox"  value="js"> JavaScript
    
    <hr>

    <h3>Resume:-</h3>
    Upload resume: (PDF) <input type="file" id="cv" name="resume" accept=".pdf"><br><br>
    <textarea id="cover" name="cover" rows="5" cols="50" maxlength="500"></textarea><br><br>

    <input type="checkbox" name="agree" required> I confirm that the information is correct.<br><br>

    <button type="submit">Apply now</button> 
    <button type="reset" >Reset</button>
    <button type="print" >Print</button>
  </form>
</body>

</html>
