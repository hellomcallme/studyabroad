# studyabroad
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Study Abroad Tips</title>
    <style>
        /* Add your CSS styles here */
        body {
            font-family: Arial, sans-serif;
            background-color: #f3f3f3;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #007BFF;
            color: #fff;
            text-align: center;
            padding: 20px;
        }

        h1 {
            margin: 0;
            font-size: 36px;
        }

        .content {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        /* Add more styles as needed */

    </style>
</head>
<body>
    <header>
        <h1>Study Abroad Tips</h1>
        <p>Your one-stop destination for studying abroad information</p>
    </header>
    <div class="content">
        <h2>Choose a Country</h2>
        <p>Select a country below to get detailed information:</p>
        <form id="countryForm">
            <select id="countrySelect">
                <option value="usa">United States</option>
                <option value="uk">United Kingdom</option>
                <option value="canada">Canada</option>
                <!-- Add more countries as needed -->
            </select>
            <button type="button" onclick="showCountryInfo()">Get Info</button>
        </form>
        <div id="countryInfo">
            <!-- Country information will be displayed here -->
        </div>
    </div>

    <script>
        // Add JavaScript code here
        function showCountryInfo() {
            const countrySelect = document.getElementById("countrySelect");
            const selectedCountry = countrySelect.value;
            const countryInfo = document.getElementById("countryInfo");

            // You can replace these placeholders with actual information about each country
            const countryData = {
                usa: "Information about studying in the United States.",
                uk: "Information about studying in the United Kingdom.",
                canada: "Information about studying in Canada."
                // Add more information for other countries
            };

            countryInfo.innerHTML = countryData[selectedCountry] || "Country information not found.";
        }
    </script>
</body>
</html>
