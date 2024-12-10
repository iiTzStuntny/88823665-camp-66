<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Workshop #HTML - FORM</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f9f9f9;
            color: #333;
            margin: 0;
            padding: 20px;
        }
        h1 {
            text-align: center;
            color: #007BFF;
        }
        form {
            max-width: 600px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            transition: background-color 0.3s;
        }
        form:hover {
            background-color: #f0f8ff;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        input[type="text"], input[type="number"], input[type="file"], textarea, select {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
            transition: border-color 0.3s, box-shadow 0.3s;
        }
        input[type="text"]:focus, input[type="number"]:focus, textarea:focus, select:focus {
            border-color: #007BFF;
            box-shadow: 0 0 5px rgba(0, 123, 255, 0.5);
            outline: none;
        }
        input[type="radio"], input[type="checkbox"] {
            margin-right: 10px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            background-color: #007BFF;
            color: white;
            transition: background-color 0.3s, transform 0.2s;
        }
        button:hover {
            background-color: #0056b3;
            transform: scale(1.05);
        }
        button[type="reset"] {
            background-color: #6c757d;
        }
        button[type="reset"]:hover {
            background-color: #5a6268;
        }
        textarea {
            resize: vertical;
        }
    </style>
</head>
<body>
    <h1>Workshop #HTML - FORM</h1>
    <form action="#" method="post">
        <label for="firstname">ชื่อ:</label>
        <input type="text" id="firstname" name="firstname">
        <label for="lastname">สกุล:</label>
        <input type="text" id="lastname" name="lastname">
        <label for="dob">วัน/เดือน/ปีเกิด:</label>
        <input type="text" id="dob" name="dob" placeholder="dd/mm/yyyy" pattern="\d{2}/\d{2}/\d{4}" title="กรุณาใส่รูปแบบ dd/mm/yyyy">
        <label for="age">อายุ:</label>
        <input type="number" id="age" name="age" min="0">
        <label>เพศ:</label>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">ชาย</label>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">หญิง</label>
        <label for="photo">รูป:</label>
        <input type="file" id="photo" name="photo">
        <label for="address">ที่อยู่:</label>
        <textarea id="address" name="address" rows="4" cols="50"></textarea>
        <label for="color">สีที่ชอบ:</label>
        <select id="color" name="color">
            <option value="red">สีแดง</option>
            <option value="blue">สีน้ำเงิน</option>
            <option value="green">สีเขียว</option>
        </select>
        <label>แนวเพลงที่ชอบ:</label>
        <input type="checkbox" id="forlife" name="music" value="เพื่อชีวิต">
        <label for="forlife">เพื่อชีวิต</label>
        <input type="checkbox" id="lukthung" name="music" value="ลูกทุ่ง">
        <label for="lukthung">ลูกทุ่ง</label>
        <input type="checkbox" id="other" name="music" value="อื่นๆ">
        <label for="other">อื่นๆ</label>
        <input type="checkbox" id="agree" name="agree">
        <label for="agree">ยินยอมให้เก็บข้อมูล</label>
        <div style="text-align: center;">
            <button type="reset">Reset</button>
            <button type="submit">Submit</button>
        </div>
    </form>
</body>
</html>