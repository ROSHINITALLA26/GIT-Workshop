# GIT-Workshop
<!DOCTYPE html>
<html>
<head>
    <title>peach</title>
</head>
<body>
    <label for="name">Name:</label>
    <input id="name"/><br>
    <select id="gender">
        <option value="Male">Male</option>
        <option value="female">Female</option>
    </select>
    <input type="submit" onclick="show()"/>

    <script>
        function show() {
            var nameInput = document.getElementById("name");
            var genderInput = document.getElementById("gender");
            var name = nameInput.value;
            var gender = genderInput.value;
            var message = '';
            if (gender === 'male') {
                message = 'Hello Mr. ' + name;
            } else if (gender === 'female') {
                message = 'Hello Miss. ' + name;
            } else {
                message = 'Hello ' + name;
            }
            console.log(message);
            alert(message);
        }
    </script>
</body>
</html>
