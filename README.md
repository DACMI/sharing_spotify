<script>
        function authenticate() {
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;

            // Hardcoded username-password pairs
            var users = {
                "binh": "1",
                "nam": "1"
            };

            // Check if the entered username exists and the password matches
            if (users.hasOwnProperty(username) && users[username] === password) {
                window.location.href = "dashboard.html"; // Redirect to dashboard
                return false; // Prevent form submission
            } else {
                alert("Invalid username or password."); // Show error message
                return false; // Prevent form submission
            }
        }
    </script>
