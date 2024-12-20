# TEST

**TEST** เป็นโปรเจกต์สำหรับการทดสอบ end-to-end ใน ...... ใช้ **Robot Framework** และเครื่องมืออื่นๆ เพื่อให้แน่ใจว่าการทำงานของแอปพลิเคชันเป็นไปตามที่คาดหวัง

## การตั้งค่าโปรเจกต์

### 1. สร้าง Virtual Environment

แต่ละคนในทีมควรสร้าง **virtual environment** บนเครื่องของตนเองเพื่อแยก dependencies ของโปรเจกต์จากระบบโดยรวม:

```bash
python3 -m venv venv
```

### 2. เปิดใช้งาน Virtual Environment

หลังจากที่คุณสร้าง virtual environment แล้ว คุณต้องเปิดใช้งานมัน:

```bash
source venv/bin/activate
```

### 3. ติดตั้ง Dependencies

เมื่อเปิดใช้งาน virtual environment แล้ว ให้ติดตั้ง dependencies ที่จำเป็นทั้งหมดจากไฟล์ requirements.txt:

```bash
pip3 install -r requirements.txt
```

### 4. วิธีรันไฟล์ test 

ใช้คำสั่ง
```bash
robot --listener allure_robotframework:results --outputdir results tests/test_file.robot
```

### 5. วิธีรัน Test Report

ใช้คำสั่ง
```bash
brew install allure
```

ใช้คำสั่ง
```bash
allure serve results
```

## เอกสารเพิ่มเติม

- [Robot Framework Documentation](https://robotframework.org/)

