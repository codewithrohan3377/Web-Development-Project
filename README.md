@model _39_project.Models.hotel1
@{
    Layout = null;
}

<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width" />
    <title>Create</title>
    <style>
        /* CSS styles */
        /* CSS styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9; /* Light gray background */
        }

        h1 {
            text-align: center;
            margin-top: 20px;
            color: #333; /* Dark text color */
        }

        table {
            width: 50%;
            margin: 20px auto;
            border-collapse: collapse;
            background-color: #fff; /* White background for the table */
            border-radius: 10px; /* Rounded corners */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Box shadow for depth */
        }

        th, td {
            padding: 12px; /* Increased padding for better spacing */
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        th {
            background-color: #f2f2f2; /* Light gray background for table headers */
        }

        input[type="text"], input[type="submit"], input[type="number"] {
            width: calc(100% - 24px); /* Adjusted width for text inputs */
            padding: 10px; /* Adjusted padding for text inputs */
            margin: 5px 0;
            box-sizing: border-box;
            border: 1px solid #ccc; /* Gray border */
            border-radius: 5px; /* Rounded corners */
            transition: border-color 0.3s; /* Smooth transition for border color */
        }

            input[type="text"]:focus, input[type="number"]:focus {
                border-color: #4CAF50; /* Green border on focus */
            }

        input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s; /* Smooth transition for background color */
        }

            input[type="submit"]:hover {
                background-color: #45a049; /* Darker green on hover */
            }

        .back-button {
            display: block;
            width: 100px;
            margin: 20px auto;
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            text-align: center;
            text-decoration: none;
            transition: background-color 0.3s; /* Smooth transition for background color */
        }

            .back-button:hover {
                background-color: #555; /* Darker background on hover */
            }

        /* Additional hover effects */
        table tr:hover {
            background-color: #f5f5f5; /* Light gray background on hover */
        }

        /* CSS styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9; /* Light gray background */
        }

        h1 {
            text-align: center;
            margin-top: 20px;
            color: #333; /* Dark text color */
        }

        table {
            width: 50%;
            margin: 20px auto;
            border-collapse: collapse;
            background-color: #fff; /* White background for the table */
            border-radius: 10px; /* Rounded corners */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Box shadow for depth */
        }

        th, td {
            padding: 12px; /* Increased padding for better spacing */
textalign: left;
            border-bottom: 1px solid #ddd;
        }

        th {
            background-color: #f2f2f2; /* Light gray background for table headers */
        }

      input[type="text"], input[type="submit"], input[type="number"] {
            width: calc(100% - 24px); /* Adjusted width for text inputs */
            padding: 10px; /* Adjusted padding for text inputs */
            margin: 5px 0;
            box-sizing: border-box;
            border: 1px solid #ccc; /* Gray border */
            border-radius: 5px; /* Rounded corners */
            transition: border-color 0.3s; /* Smooth transition for border color */
        }

            input[type="text"]:focus, input[type="number"]:focus {
                border-color: #4CAF50; /* Green border on focus */
            }

        input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s; /* Smooth transition for background color */
        }

            input[type="submit"]:hover {
                background-color: #45a049; /* Darker green on hover */
            }

        .back-button {
            display: block;
            width: 100px;
            margin: 20px auto;
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            text-align: center;
            text-decoration: none;
            transition: background-color 0.3s; /* Smooth transition for background color */
        }

            .back-button:hover {
                background-color: #555; /* Darker background on hover */
            }

        /* Additional hover effects */
        table tr:hover {
            background-color:gold; /* Light gray background on hover */
        }

        input[type="text"]:hover, input[type="number"]:hover {
            border-color: red; /* Darker border on hover */
        }

        input[type="submit"]:hover {
            background-color: #45a049; /* Darker green on hover */
        }


	    </style>
	</head>
	<body>
    @Html.ActionLink("View All Customer", "Index")

    <h1>Create New Customer</h1>

    <div>
        @using (Html.BeginForm())
        {
            <table>
                <tr>
                    <th>Cust Id</th>
                    <td>@Html.TextBoxFor(e => e.custid)</td>
                </tr>
                <tr>
                    <th>Adhar no.</th>
                    <td>@Html.TextBoxFor(e => e.adhar)</td>
                </tr>
                <tr>
                    <th>First Name</th>
                   <td>@Html.TextBoxFor(e => e.fname)</td>
                </tr>
               <tr>
                   <th>Last Name</th>
                    <td>@Html.TextBoxFor(e => e.lname)</td>
                </tr>
                <tr>
                    <th>Date of birth</th>
                    <td>@Html.TextBoxFor(e => e.dob)</td>
                </tr>
                <tr>
                    <th>Customer Address</th>
                    <td>@Html.TextBoxFor(e => e.address)</td>
                </tr>
                <tr>
                    <th>Country</th>
                    <td>@Html.TextBoxFor(e => e.country)</td>
                </tr>
                 <th>Phone NO</th>
                   <td>@Html.TextBoxFor(e => e.phoneno)</td>
               </tr>
               <tr>
                   <th>Email Address</th>
                   <td>@Html.TextBoxFor(e => e.email)</td>
               </tr>
               <tr>
                   <th>No. of Rooms Require</th>
                   <td><input type="number" id="roomCount" name="room"onchange="calculateTotalAmount()"></td>
                </tr>
               <tr>
                   <th>Amount</th>
                    <td><span id="totalAmount">500</span></td>
                    <td>@Html.TextBoxFor(e => e.amount)</td>
                </tr>

                <tr>
                    <td colspan="2">
                        <input type="submit" value="Submit" />
                    </td>
                </tr>
            </table>
        }
    </div>

    <!-- Back Button -->
    <a href="~/homePage1.html" class="back-button">Back</a>

    <script>
        function calculateTotalAmount() {
            var roomCount = document.getElementById("roomCount").value;
            var amountPerRoom = 500;
            var totalAmount = roomCount * amountPerRoom;
            document.getElementById("totalAmount").innerText = totalAmount;
        }
    </script>
</body>
</html>
# Web-Development-Project
Web Development Project
