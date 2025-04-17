<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ฟอร์มขอการเข้าถึงเว็ปไซต์ภายนอก</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f4f9;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            max-width: 500px;
            width: 100%;
        }
        h1 {
            font-size: 1.5em;
            color: #6c757d;
            text-align: center;
        }
        label {
            display: block;
            margin-top: 15px;
            font-size: 1em;
        }
        input, select, button {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            font-size: 1em;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            background-color: #d4a5bf;
            color: #fff;
            border: none;
            cursor: pointer;
            margin-top: 20px;
        }
        button:hover {
            background-color: #c48ab3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>ฟอร์มขอการเข้าถึงเว็ปไซต์ภายนอก</h1>
        <form action="[Google Form POST URL]" method="POST" target="hidden_iframe" onsubmit="submitted=true;">
            <label for="name">ชื่อ-นามสกุล</label>
            <input type="text" id="name" name="entry.XXXXXXX" required>

            <label for="department">หน่วยงาน</label>
            <select id="department" name="entry.YYYYYYY" required>
                <option value="กองจัดการหนี้ 1">กองจัดการหนี้ 1</option>
                <option value="กองจัดการหนี้ 2">กองจัดการหนี้ 2</option>
                <option value="กองนโยบายและแผนการบริหารหนี้สาธารณะ">กองนโยบายและแผนการบริหารหนี้สาธารณะ</option>
                <option value="กองบริหารการชำระหนี้">กองบริหารการชำระหนี้</option>
                <option value="กองพัฒนาตลาดตราสารหนี้">กองพัฒนาตลาดตราสารหนี้</option>
                <option value="กองบริหารการระดมทุนโครงการลงทุนภาครัฐ">กองบริหารการระดมทุนโครงการลงทุนภาครัฐ</option>
                <option value="กองประเมินผลโครงการ">กองประเมินผลโครงการ</option>
                <option value="สำนักงานเลขานุการกรม">สำนักงานเลขานุการกรม</option>
                <option value="ศูนย์ข้อมูลและเทคโนโลยีสารสนเทศ">ศูนย์ข้อมูลและเทคโนโลยีสารสนเทศ</option>
                <option value="กลุ่มพัฒนาระบบบริหาร">กลุ่มพัฒนาระบบบริหาร</option>
                <option value="กลุ่มตรวจสอบภายใน">กลุ่มตรวจสอบภายใน</option>
                <option value="กลุ่มกฎหมาย">กลุ่มกฎหมาย</option>
                <option value="กลุ่มบริหารความเสี่ยงหนี้สาธารณะ">กลุ่มบริหารความเสี่ยงหนี้สาธารณะ</option>
                <option value="กลุ่มบริหารและพัฒนาทรัพยากรบุคคล">กลุ่มบริหารและพัฒนาทรัพยากรบุคคล</option>
            </select>

            <label for="position">ตำแหน่ง</label>
            <input type="text" id="position" name="entry.ZZZZZZZ" required>

            <label for="website">เว็ปไซต์ที่ต้องการใช้งาน</label>
            <input type="text" id="website" name="entry.AAAAAAA" required>

            <button type="submit">Submit</button>
        </form>
        <iframe name="hidden_iframe" style="display:none;"></iframe>
    </div>
</body>
</html>
