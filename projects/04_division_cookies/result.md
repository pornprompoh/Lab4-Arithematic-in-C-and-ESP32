# โปรเจค 4: การหาร - คุกกี้แบ่งกัน 🍪

## 🎯 โจทย์
มีคุกกี้ 12 ชิ้น จะแบ่งให้เพื่อน 4 คน  
**คำถาม:** แต่ละคนได้กี่ชิ้น?

## 🧮 การคิด
- คุกกี้ทั้งหมด = 12 ชิ้น
- จำนวนเพื่อน = 4 คน
- คุกกี้ต่อคน = 12 ÷ 4 = 3 ชิ้น

## 💻 การเขียนโปรแกรม

### สิ่งที่จะเรียนรู้:
- การหารเลข (Division)
- การตรวจสอบการหารด้วยศูนย์
- การหารที่หารลงตัวและไม่ลงตัว
- การแสดงเศษที่เหลือ (Remainder)

### โครงสร้างโปรแกรม:
```c
1. ประกาศตัวแปรจำนวนคุกกี้และคน
2. ตรวจสอบว่าไม่หารด้วยศูนย์
3. คำนวณการหารและเศษที่เหลือ
4. แสดงผลทั้งกรณีหารลงตัวและไม่ลงตัว
```

## 🚀 วิธีรัน

```bash
cd projects/04_division_cookies/
idf.py build
idf.py qemu monitor
```

## 🚪 วิธีออกจาก Qemu
``` c
    หากต้องการออกจาก QEMU monitor ให้กด Ctrl+]
``` 


## 🎓 ท้าทาย

ลองแก้ไขโค้ดในไฟล์ `main/main.c`:

### 📝 แบบฝึกหัดที่ 1: เปลี่ยนจำนวนคุกกี้
```c
// หาบรรทัดนี้ในโค้ด:
int total_cookies = 20;    // คุกกี้ทั้งหมด
int friends = 4;           // จำนวนเพื่อน

// ลองเปลี่ยนเป็น:
int total_cookies = 24;    // เพิ่มเป็น 24 ชิ้น
int friends = 6;           // เพิ่มเป็น 6 คน
```
### ผลการรัน
```
I (17613) COOKIES_MATH: 🧮 ขั้นตอนการคิด:
I (17613) COOKIES_MATH:    คุกกี้ทั้งหมด ÷ จำนวนเพื่อน
I (17613) COOKIES_MATH:    = 24 ÷ 6
I (17623) COOKIES_MATH:    = 4 ชิ้นต่อคน
I (17623) COOKIES_MATH: 
I (17623) COOKIES_MATH: ✅ คำตอบ:
I (17623) COOKIES_MATH:    แต่ละคนได้คุกกี้ 4 ชิ้น
I (17633) COOKIES_MATH:    แบ่งได้พอดี ไม่มีเหลือ
I (17633) COOKIES_MATH: 
I (17633) COOKIES_MATH: 🎨 ภาพประกอบการแบ่ง:
I (17633) COOKIES_MATH:    คุกกี้ทั้งหมด: 🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪 (24 ชิ้น)
I (17633) COOKIES_MATH: 
I (17633) COOKIES_MATH:    เพื่อนคนที่ 1: 
I (17633) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17633) COOKIES_MATH:    เพื่อนคนที่ 2: 
I (17633) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17643) COOKIES_MATH:    เพื่อนคนที่ 3: 
I (17643) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17643) COOKIES_MATH:    เพื่อนคนที่ 4: 
I (17643) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17643) COOKIES_MATH:    เพื่อนคนที่ 5: 
I (17643) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17643) COOKIES_MATH:    เพื่อนคนที่ 6: 
I (17643) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17643) COOKIES_MATH: 
I (17643) COOKIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (17643) COOKIES_MATH:    คุกกี้ 15 ชิ้น แบ่งให้ 3 คน
I (17643) COOKIES_MATH:    = 15 ÷ 3 = 5 ชิ้นต่อคน, เหลือ 0 ชิ้น
I (17643) COOKIES_MATH: 
I (17643) COOKIES_MATH:    คุกกี้ 13 ชิ้น แบ่งให้ 4 คน
I (17643) COOKIES_MATH:    = 13 ÷ 4 = 3 ชิ้นต่อคน, เหลือ 1 ชิ้น
I (17643) COOKIES_MATH:    (หารไม่ลงตัว)
I (17653) COOKIES_MATH: 
I (17653) COOKIES_MATH: ⚠️  กรณีพิเศษ - หารด้วยศูนย์:
I (17653) COOKIES_MATH:    ถ้าไม่มีเพื่อนมาแบ่ง (หารด้วย 0)
I (17653) COOKIES_MATH:    ไม่สามารถคำนวณได้ในทางคณิตศาสตร์
I (17653) COOKIES_MATH:    ในชีวิตจริง: คุกกี้จะเหลือทั้งหมด
I (17653) COOKIES_MATH: 
I (17653) COOKIES_MATH: 🔄 ความสัมพันธ์กับการคูณ:
I (17653) COOKIES_MATH:    การหาร: 24 ÷ 6 = 4
I (17653) COOKIES_MATH:    การคูณ: 4 × 6 = 24
I (17663) COOKIES_MATH:    การหารและการคูณเป็นการดำเนินการตรงข้ามกัน
I (17663) COOKIES_MATH: 
I (17663) COOKIES_MATH: 📊 สรุปการดำเนินการทั้งหมด:
I (17663) COOKIES_MATH:    การบวก (+): เพิ่มจำนวน
I (17663) COOKIES_MATH:    การลบ (-): ลดจำนวน
I (17663) COOKIES_MATH:    การคูณ (×): บวกซ้ำๆ หลายชุด
I (17663) COOKIES_MATH:    การหาร (÷): แบ่งออกเป็นกลุ่มเท่าๆ กัน
I (17673) COOKIES_MATH: 
I (17673) COOKIES_MATH: 🎓 แนวคิดขั้นสูง:
I (17673) COOKIES_MATH:    1. การหารจะได้ผลหาร (quotient) และเศษ (remainder)
I (17673) COOKIES_MATH:    2. ในภาษา C:
I (17673) COOKIES_MATH:       ผลหาร = a / b
I (17673) COOKIES_MATH:       เศษ = a % b
I (17673) COOKIES_MATH:    3. การตรวจสอบการหารด้วยศูนย์เป็นสิ่งสำคัญ
I (17673) COOKIES_MATH:    4. การหารด้วย 1 จะได้ตัวเลขเดิม
I (17673) COOKIES_MATH:    5. การหารตัวเลขด้วยตัวมันเองจะได้ 1
I (17683) COOKIES_MATH: 
I (17683) COOKIES_MATH: 📚 สิ่งที่เรียนรู้:
I (17683) COOKIES_MATH:    1. การหารเลข (Division): a ÷ b = c
I (17683) COOKIES_MATH:    2. การใช้ Modulo operator (%) หาเศษ
I (17683) COOKIES_MATH:    3. การตรวจสอบการหารด้วยศูนย์
I (17683) COOKIES_MATH:    4. ความแตกต่างระหว่างหารลงตัวและไม่ลงตัว
I (17683) COOKIES_MATH:    5. ความสัมพันธ์ระหว่างการหารและการคูณ
I (17683) COOKIES_MATH:    6. การจัดการกรณีพิเศษ (Error Handling)
I (17683) COOKIES_MATH: 
I (17683) COOKIES_MATH: 🎉 จบโปรแกรมแบ่งคุกกี้!
I (17693) COOKIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 05_mixed_shopping
I (19693) main_task: Returned from app_main()
```
### 📝 แบบฝึกหัดที่ 2: เพิ่มการตรวจสอบหารลงตัว
เพิ่มการตรวจสอบว่าหารลงตัวไหม:
```c
int cookies_per_person = total_cookies / friends;
int remaining_cookies = total_cookies % friends;

if (remaining_cookies == 0) {
    ESP_LOGI(TAG, "✅ หารลงตัว! ทุกคนได้เท่ากัน");
} else {
    ESP_LOGI(TAG, "⚠️ หารไม่ลงตัว! เหลือ %d ชิ้น", remaining_cookies);
}
```
### ผลการรัน
```
I (19666) COOKIES_MATH: 🧮 ขั ้นตอนการคิด:
I (19666) COOKIES_MATH:    คุกกี้ทั้งหมด ÷ จำนวนเพื่อน
I (19666) COOKIES_MATH:    = 24 ÷ 6
I (19666) COOKIES_MATH:    = 4 ชิ้นต่อคน
I (19666) COOKIES_MATH: 
I (19666) COOKIES_MATH: ✅ คำตอบ:
I (19666) COOKIES_MATH:    แต่ละคนได้คุกกี้ 4 ชิ้น
I (19666) COOKIES_MATH:    แบ่งได้พอดี ไม่มีเหลือ
I (19666) COOKIES_MATH: 
I (19666) COOKIES_MATH: 🎨 ภาพประกอบการแบ่ง:
I (19666) COOKIES_MATH:    คุกกี้ทั้งหมด: 🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪 (24 ชิ้น)
I (19676) COOKIES_MATH: 
I (19676) COOKIES_MATH:    เพื่อนคนที่ 1: 
I (19676) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (19676) COOKIES_MATH:    เพื่อนคนที่ 2: 
I (19676) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (19676) COOKIES_MATH:    เพื่อนคนที่ 3: 
I (19676) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (19676) COOKIES_MATH:    เพื่อนคนที่ 4: 
I (19676) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (19676) COOKIES_MATH:    เพื่อนคนที่ 5: 
I (19676) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (19676) COOKIES_MATH:    เพื่อนคนที่ 6: 
I (19676) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (19676) COOKIES_MATH: 
I (19676) COOKIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (19686) COOKIES_MATH:    คุกกี้ 15 ชิ้น แบ่งให้ 3 คน
I (19686) COOKIES_MATH:    = 15 ÷ 3 = 5 ชิ้นต่อคน, เหลือ 0 ชิ้น
I (19686) COOKIES_MATH: 
I (19686) COOKIES_MATH:    คุกกี้ 13 ชิ้น แบ่งให้ 4 คน
I (19686) COOKIES_MATH:    = 13 ÷ 4 = 3 ชิ้นต่อคน, เหลือ 1 ชิ้น
I (19686) COOKIES_MATH:    (หารไม่ลงตัว)
I (19686) COOKIES_MATH: 
I (19686) COOKIES_MATH: ⚠️  กรณีพิเศษ - หารด้วยศูนย์:
I (19686) COOKIES_MATH:    ถ้าไม่มีเพื่อนมาแบ่ง (หารด้วย 0)
I (19686) COOKIES_MATH:    ไม่สามารถคำนวณได้ในทางคณิตศาสตร์
I (19696) COOKIES_MATH:    ในชีวิตจริง: คุกกี้จะเหลือทั้งหมด
I (19696) COOKIES_MATH: 
I (19696) COOKIES_MATH: 🔄 ความสัมพันธ์กับการคูณ:
I (19706) COOKIES_MATH:    การหาร: 24 ÷ 6 = 4
I (19706) COOKIES_MATH:    การคูณ: 4 × 6 = 24
I (19706) COOKIES_MATH:    การหารและการคูณเป็นการดำเนินการตรงข้ามกัน
I (19706) COOKIES_MATH: 
I (19706) COOKIES_MATH: ✅ หารลงตัว! ทุกคนได้เท่ากัน
I (19706) COOKIES_MATH: 📊 สรุปการดำเนินการทั้งหมด:
I (19706) COOKIES_MATH:    การบวก (+): เพิ่มจำนวน
I (19706) COOKIES_MATH:    การลบ (-): ลดจำนวน
I (19706) COOKIES_MATH:    การคูณ (×): บวกซ้ำๆ หลายชุด
I (19706) COOKIES_MATH:    การหาร (÷): แบ่งออกเป็นกลุ่มเท่าๆ กัน
I (19716) COOKIES_MATH: 
I (19716) COOKIES_MATH: 🎓 แนวคิดขั้นสูง:
I (19716) COOKIES_MATH:    1. การหารจะได้ผลหาร (quotient) และเศษ (remainder)
I (19716) COOKIES_MATH:    2. ในภาษา C:
I (19716) COOKIES_MATH:       ผลหาร = a / b
I (19716) COOKIES_MATH:       เศษ = a % b
I (19716) COOKIES_MATH:    3. การตรวจสอบการหารด้วยศูนย์เป็นสิ่งสำคัญ
I (19716) COOKIES_MATH:    4. การหารด้วย 1 จะได้ตัวเลขเดิม
I (19716) COOKIES_MATH:    5. การหารตัวเลขด้วยตัวมันเองจะได้ 1
I (19716) COOKIES_MATH: 
I (19716) COOKIES_MATH: 📚 สิ่งที่เรียนรู้:
I (19716) COOKIES_MATH:    1. การหารเลข (Division): a ÷ b = c
I (19716) COOKIES_MATH:    2. การใช้ Modulo operator (%) หาเศษ
I (19716) COOKIES_MATH:    3. การตรวจสอบการหารด้วยศูนย์
I (19726) COOKIES_MATH:    4. ความแตกต่างระหว่างหารลงตัวและไม่ลงตัว
I (19726) COOKIES_MATH:    5. ความสัมพันธ์ระหว่างการหารและการคูณ
I (19726) COOKIES_MATH:    6. การจัดการกรณีพิเศษ (Error Handling)
I (19726) COOKIES_MATH: 
I (19736) COOKIES_MATH: 🎉 จบโปรแกรมแบ่งคุกกี้!
I (19736) COOKIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 05_mixed_shopping
I (21736) main_task: Returned from app_main()
```
### 📝 แบบฝึกหัดที่ 3: หาจำนวนเพื่อนที่เหมาะสม
ลองหาว่าคุกกี้ 30 ชิ้น จะแจกให้กี่คนได้หารลงตัว:
```c
int cookies = 30;
ESP_LOGI(TAG, "🔍 คุกกี้ %d ชิ้น หารลงตัวกับ:", cookies);

for (int people = 1; people <= 10; people++) {
    if (cookies % people == 0) {
        ESP_LOGI(TAG, "   ✅ %d คน → คนละ %d ชิ้น", 
                 people, cookies / people);
    }
}
```
### ผลการรัน
```
I (17848) COOKIES_MATH: 🧮 ขั้นตอนการคิด:
I (17848) COOKIES_MATH:    คุกกี้ทั้งหมด ÷ จำนวนเพื่อน
I (17848) COOKIES_MATH:    = 24 ÷ 6
I (17848) COOKIES_MATH:    = 4 ชิ้นต่อคน
I (17848) COOKIES_MATH: 
I (17848) COOKIES_MATH: ✅ คำตอบ:
I (17848) COOKIES_MATH:    แต่ละคนได้คุกกี้ 4 ชิ้น
I (17848) COOKIES_MATH:    แบ่งได้พอดี ไม่มีเหลือ
I (17848) COOKIES_MATH: 
I (17848) COOKIES_MATH: 🎨 ภาพประกอบการแบ่ง:
I (17848) COOKIES_MATH:    คุกกี้ทั้งหมด: 🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪🍪 (24 ชิ้น)
I (17848) COOKIES_MATH: 
I (17848) COOKIES_MATH:    เพื่อนคนที่ 1: 
I (17848) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17848) COOKIES_MATH:    เพื่อนคนที่ 2: 
I (17858) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17858) COOKIES_MATH:    เพื่อนคนที่ 3: 
I (17858) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17858) COOKIES_MATH:    เพื่อนคนที่ 4: 
I (17858) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17858) COOKIES_MATH:    เพื่อนคนที่ 5: 
I (17858) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17858) COOKIES_MATH:    เพื่อนคนที่ 6: 
I (17858) COOKIES_MATH: 🍪🍪🍪 (4 ชิ้น)
I (17858) COOKIES_MATH: 
I (17858) COOKIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (17858) COOKIES_MATH:    คุกกี้ 15 ชิ้น แบ่งให้ 3 คน
I (17858) COOKIES_MATH:    = 15 ÷ 3 = 5 ชิ้นต่อคน, เหลือ 0 ชิ้น
I (17858) COOKIES_MATH: 
I (17858) COOKIES_MATH:    คุกกี้ 13 ชิ้น แบ่งให้ 4 คน
I (17858) COOKIES_MATH:    = 13 ÷ 4 = 3 ชิ้นต่อคน, เหลือ 1 ชิ้น
I (17858) COOKIES_MATH:    (หารไม่ลงตัว)
I (17858) COOKIES_MATH: 
I (17858) COOKIES_MATH: ⚠️  กรณีพิเศษ - หารด้วยศูนย์:
I (17858) COOKIES_MATH:    ถ้าไม่มีเพื่อนมาแบ่ง (หารด้วย 0)
I (17858) COOKIES_MATH:    ไม่สามารถคำนวณได้ในทางคณิตศาสตร์
I (17858) COOKIES_MATH:    ในชีวิตจริง: คุกกี้จะเหลือทั้งหมด
I (17858) COOKIES_MATH: 
I (17858) COOKIES_MATH: 🔄 ความสัมพันธ์กับการคูณ:
I (17868) COOKIES_MATH:    การหาร: 24 ÷ 6 = 4
I (17868) COOKIES_MATH:    การคูณ: 4 × 6 = 24
I (17868) COOKIES_MATH:    การหารและการคูณเป็นการดำเนินการตรงข้ามกัน
I (17868) COOKIES_MATH: 
I (17868) COOKIES_MATH: ✅ หารลงตัว! ทุกคนได้เท่ากัน
I (17868) COOKIES_MATH: 📊 สรุปการดำเนินการทั้งหมด:
I (17868) COOKIES_MATH:    การบวก (+): เพิ่มจำนวน
I (17868) COOKIES_MATH:    การลบ (-): ลดจำนวน
I (17868) COOKIES_MATH:    การคูณ (×): บวกซ้ำๆ หลายชุด
I (17868) COOKIES_MATH:    การหาร (÷): แบ่งออกเป็นกลุ่มเท่าๆ กัน
I (17878) COOKIES_MATH: 
I (17878) COOKIES_MATH: 🎓 แนวคิดขั้นสูง:
I (17878) COOKIES_MATH:    1. การหารจะได้ผลหาร (quotient) และเศษ (remainder)
I (17878) COOKIES_MATH:    2. ในภาษา C:
I (17878) COOKIES_MATH:       ผลหาร = a / b
I (17878) COOKIES_MATH:       เศษ = a % b
I (17878) COOKIES_MATH:    3. การตรวจสอบการหารด้วยศูนย์เป็นสิ่งสำคัญ
I (17878) COOKIES_MATH:    4. การหารด้วย 1 จะได้ตัวเลขเดิม
I (17878) COOKIES_MATH:    5. การหารตัวเลขด้วยตัวมันเองจะได้ 1
I (17878) COOKIES_MATH: 
I (17878) COOKIES_MATH: 📚 สิ่งที่เรียนรู้:
I (17878) COOKIES_MATH:    1. การหารเลข (Division): a ÷ b = c
I (17878) COOKIES_MATH:    2. การใช้ Modulo operator (%) หาเศษ
I (17878) COOKIES_MATH:    3. การตรวจสอบการหารด้วยศูนย์
I (17888) COOKIES_MATH:    4. ความแตกต่างระหว่างหารลงตัวและไม่ลงตัว
I (17888) COOKIES_MATH:    5. ความสัมพันธ์ระหว่างการหารและการคูณ
I (17888) COOKIES_MATH:    6. การจัดการกรณีพิเศษ (Error Handling)
I (17888) COOKIES_MATH: 
I (17888) COOKIES_MATH: 🎉 จบโปรแกรมแบ่งคุกกี้!
I (17888) COOKIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 05_mixed_shopping
I (17888) COOKIES_MATH: 🔍 คุกกี้ 30 ชิ้น หารลงตัวกับ:
I (17888) COOKIES_MATH:    ✅ 1 คน → คนละ 30 ชิ้น
I (17888) COOKIES_MATH:    ✅ 2 คน → คนละ 15 ชิ้น
I (17888) COOKIES_MATH:    ✅ 3 คน → คนละ 10 ชิ้น
I (17888) COOKIES_MATH:    ✅ 5 คน → คนละ 6 ชิ้น
I (17888) COOKIES_MATH:    ✅ 6 คน → คนละ 5 ชิ้น
I (17888) COOKIES_MATH:    ✅ 10 คน → คนละ 3 ชิ้น
I (19888) main_task: Returned from app_main()
```
### 🏆 เป้าหมาย:
- [ ] เปลี่ยนจำนวนคุกกี้และเพื่อนได้
- [ ] ตรวจสอบการหารลงตัวได้
- [ ] หาจำนวนที่หารลงตัวได้
- [ ] เข้าใจการหาร และเศษ (%)

## ✅ ผลลัพธ์ที่คาดหวัง

```
=== คุกกี้แบ่งกัน ===
คุกกี้ทั้งหมด: 12 ชิ้น
จำนวนเพื่อน: 4 คน
แต่ละคนได้: 12 ÷ 4 = 3 ชิ้น
เศษที่เหลือ: 0 ชิ้น
```
