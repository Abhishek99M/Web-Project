# Web-Project
<!DOCTYPE html>
<html>
<head>
    <title>Registration Form</title>
    <link rel="stylesheet" href="js-form-validation.css" type="text/css" />
    <script src="sample-registration-form-validation.js"></script>
</head>
<style>
    body{
            font-family: latha;
            color: white;
            background: linear-gradient(
                rgba(0,0,0,0),rgba(0, 0, 0, 0),rgba(0,0,0,0),rgba(0,0,0,0))
            ,url(PP.jpg)no-repeat;
            background-size: cover;
}
</style>
<body onload="document.ragistration.userid.focus();">
    <h1>
        Registration Form
    </h1>
    <p>Required fill all the information (*) related</p>
    <form name="registration" onsubmit="return formValidation();">
        <ul>
            <li><p>*User Id: <input type="text" required></p></li>
            <li><p>*Password: <input type="text" required></p></li>
            <li><p>*Name: <input type="text" required></p></li>
            <li><p>*Address: <textarea name="Address" id="Address" cols="40" rows="-5"></textarea required></p></li>
            <li><label for="country">Country:</label></li>
            <li><select name="country">
            <option selected="" value="Default">(Please select a country)</option>
            <option value="AF">Australia</option>
            <option value="AL">Canada</option>
            <option value="DZ">India</option>
            <option value="AS">Russia</option>
            <option value="AD">USA</option>
            </select></li>
            <li><p>*Zip code: <input type="number" name="pincode" id="pincode" required></p></li>
            <li><p>*Email: <input type="email" name="email" id="email" required></p></li>
            <li>
                <legend>*Gender</legend>
                <p>
                    Male <input type="radio" name="gender" id="Male">
                    Female <input type="radio" name="gender" id="Female">
                </p>
            
            </li>
            <li><label>Language:</label></li>
            <li><input type="checkbox" name="en" value="en" checked /><span>English</span></li>
            <li><input type="checkbox" name="nonen" value="noen" /><span>Non English</span></li>
            <li><label for="desc">About:</label></li>
            <li><textarea name="desc" id="desc"></textarea></li>
            <li><input type="submit" name="submit" value="Submit" /></li>
            </ul>
    </form>
</body>
</html>
