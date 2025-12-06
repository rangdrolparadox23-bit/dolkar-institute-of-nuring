# dolkar-institute-of-nuring
Admission Portal for Dolkar’s Institute of Nursing
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dolkar’s Institute Of Nursing - Admissions</title>

    <style>
        body {
            font-family: "Segoe UI", Arial, sans-serif;
            background: #eef4fa;
            margin: 0;
            padding: 0;
        }

        header {
            background: linear-gradient(90deg, #003f72, #006bb3);
            color: white;
            padding: 30px;
            text-align: center;
            font-size: 30px;
            font-weight: bold;
            letter-spacing: 1px;
        }

        .subheader {
            text-align: center;
            color: #003f72;
            font-size: 18px;
            margin-top: -10px;
            margin-bottom: 20px;
            font-weight: 500;
        }

        .container {
            width: 90%;
            max-width: 850px;
            background: white;
            margin: 20px auto;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 0 18px rgba(0,0,0,0.12);
        }

        h2 {
            color: #003f72;
            border-left: 6px solid #006bb3;
            padding-left: 12px;
            font-size: 22px;
            margin-top: 30px;
        }

        label {
            font-weight: 600;
            display: block;
            margin-top: 12px;
            color: #003f72;
        }

        input, textarea, select {
            width: 100%;
            padding: 12px;
            margin-top: 5px;
            border-radius: 8px;
            border: 1px solid #b4c7d9;
            font-size: 16px;
            background: #f9fcff;
        }

        input[type="file"] {
            padding: 6px;
            background: #ffffff;
        }

        button {
            background: linear-gradient(90deg, #003f72, #006bb3);
            color: white;
            padding: 15px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 18px;
            margin-top: 25px;
            width: 100%;
            font-weight: 600;
        }

        button:hover {
            opacity: 0.92;
        }

        #successMessage {
            display: none;
            background: #e6ffef;
            border-left: 6px solid #00a53c;
            padding: 20px;
            margin-top: 25px;
            border-radius: 10px;
            font-size: 18px;
            color: #007a2f;
            font-weight: 600;
        }
    </style>
</head>

<body>

<header>Dolkar’s Institute Of Nursing</header>
<div class="subheader">Admission Registration Portal</div>

<div class="container">
    <h2>Admission Form</h2>

    <form id="admissionForm">

        <!-- Personal Info -->
        <label>Name</label>
        <input type="text" required>

        <label>Personal Information</label>
        <textarea required placeholder="Write about yourself..."></textarea>

        <label>Contact Number</label>
        <input type="number" required>

        <label>Present Address</label>
        <textarea required></textarea>

        <label>Permanent Address</label>
        <textarea required></textarea>

        <label>CID Number</label>
        <input type="number" required>

        <label>Qualification</label>
        <input type="text" required>

        <h2>Upload Documents</h2>

        <label>Class 10 Pass Certificate</label>
        <input type="file" required>

        <label>Class 10 Marksheet</label>
        <input type="file" required>

        <label>Class 12 Pass Certificate</label>
        <input type="file" required>

        <label>Class 12 Marksheet</label>
        <input type="file" required>

        <label>Transfer Certificate</label>
        <input type="file" required>

        <h2>Guardian Details</h2>

        <label>Guardian Name</label>
        <input type="text" required>

        <label>Guardian Address</label>
        <textarea required></textarea>

        <label>Relation to Guardian</label>
        <input type="text" required>

        <label>Guardian Contact Number</label>
        <input type="number" required>

        <button type="submit">Submit Application</button>
    </form>

    <div id="successMessage">
        🎉 <strong>You have been successfully registered!</strong><br><br>
        Thank you for showing interest in us.<br>
        <strong>The result will be declared soon!</strong>
    </div>
</div>

<script>
    document.getElementById("admissionForm").addEventListener("submit", function(event) {
        event.preventDefault();
        document.getElementById("successMessage").style.display = "block";
        window.scrollTo(0, 0);
        document.getElementById("admissionForm").reset();
    });
</script>

</body>
</html>
