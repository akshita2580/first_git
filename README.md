# first_git
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Internship Application Form</title>
    <style>
        /* Your styles here */
    </style>
</head>
<body>

    <form id="internshipForm" action="#" method="post" onsubmit="return validateForm()">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" name="phone" required>

        <label for="coverLetter">Cover Letter:</label>
        <textarea id="coverLetter" name="coverLetter" rows="4" required></textarea>

        <button type="submit">Submit Application</button>
    </form>

    <script>
        function validateForm() {
            // Simple client-side validation for demonstration purposes
            var name = document.getElementById('name').value;
            var email = document.getElementById('email').value;
            var phone = document.getElementById('phone').value;
            var coverLetter = document.getElementById('coverLetter').value;

            if (!name || !email || !phone || !coverLetter) {
                alert('All fields must be filled out');
                return false;
            }

            // You can add more specific validation here

            return true;
        }
    </script>

</body>
</html>

