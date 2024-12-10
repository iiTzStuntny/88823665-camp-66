<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Form</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>สมัครสมาชิก</h1>
        <form action="#" method="post">
            <div class="form-group">
                <label for="firstname">ชื่อ:</label>
                <input type="text" id="firstname" name="firstname" placeholder="ชื่อของคุณ">
            </div>
            <div class="form-group">
                <label for="lastname">สกุล:</label>
                <input type="text" id="lastname" name="lastname" placeholder="สกุลของคุณ">
            </div>
         <div class="form-group">
                <label for="dob">วัน/เดือน/ปีเกิด:</label>
                <input type="text" id="dob" name="dob" placeholder="dd/mm/yyyy">
            </div>
             <div class="form-group">
                <label for="age">อายุ:</label>
                <input type="number" id="age" name="age" placeholder="อายุ">
            </div>
            <div class="form-group">
                <label>เพศ:</label>
                <div class="radio-group">
                    <input type="radio" id="male" name="gender" value="male">
                    <label for="male">ชาย</label>
                    <input type="radio" id="female" name="gender" value="female">
                    <label for="female">หญิง</label>
                </div>
            </div>
        <div class="form-group">
                <label for="photo">รูป:</label>
                <input type="file" id="photo" name="photo">
            </div>
                    <div class="form-group">
                <label for="address">ที่อยู่:</label>
                <textarea id="address" name="address" rows="4" placeholder="ที่อยู่ของคุณ"></textarea>
            </div>
            <div class="form-group">
                <label for="color">สีที่ชอบ:</label>
                <select id="color" name="color">
                    <option value="red">สีแดง</option>
                    <option value="blue">สีน้ำเงิน</option>
                    <option value="green">สีเขียว</option>
                </select>
            </div>
            <div class="form-group">
                <label>แนวเพลงที่ชอบ:</label>
                <div class="checkbox-group">
                    <input type="checkbox" id="forlife" name="music" value="เพื่อชีวิต">
                    <label for="forlife">เพื่อชีวิต</label>
                    <input type="checkbox" id="lukthung" name="music" value="ลูกทุ่ง">
                    <label for="lukthung">ลูกทุ่ง</label>
                    <input type="checkbox" id="other" name="music" value="อื่นๆ">
                    <label for="other">อื่นๆ</label>
                </div>
            </div>
<div class="form-group">
                <input type="checkbox" id="agree" name="agree">
                <label for="agree">ยินยอมให้เก็บข้อมูล</label>
            </div>
            <div class="form-buttons">
                <button type="reset" class="btn-reset">Reset</button>
                <button type="submit" class="btn-submit">Submit</button>
            </div>
        </form>
    </div>
</body>
</html>