# โปรเจค 3: การคูณ - ลูกอมในถุง 🍬

## 🎯 โจทย์
มีถุงลูกอม 5 ถุง ถุงละ 6 เม็ด  
**คำถาม:** มีลูกอมทั้งหมดกี่เม็ด?

## 🧮 การคิด
- จำนวนถุง = 5 ถุง
- ลูกอมต่อถุง = 6 เม็ด
- ลูกอมทั้งหมด = 5 × 6 = 30 เม็ด

## 💻 การเขียนโปรแกรม

### สิ่งที่จะเรียนรู้:
- การคูณเลข (Multiplication)
- การใช้ loop เพื่อแสดงการคูณ
- การแสดงผลแบบตาราง
- การเปรียบเทียบการคูณกับการบวกซ้ำๆ

### โครงสร้างโปรแกรม:
```c
1. ประกาศตัวแปรจำนวนถุงและลูกอมต่อถุง
2. คำนวณด้วยการคูณ
3. แสดงการเปรียบเทียบกับการบวกซ้ำๆ
4. แสดงตารางสูตรคูณ
```

## 🚀 วิธีรัน

```bash
cd projects/03_multiplication_candies/
idf.py build
idf.py qemu monitor
```

## 🚪 วิธีออกจาก Qemu
``` c
    หากต้องการออกจาก QEMU monitor ให้กด Ctrl+]
``` 
### ผลการรัน
```
I (21013) CANDIES_MATH: 🧮 ขั้นตอนการคิด:
I (21013) CANDIES_MATH:    จำนวนถุง × ลูกอมต่อถุง
I (21013) CANDIES_MATH:    = 5 × 6
I (21023) CANDIES_MATH:    = 30 เม็ด
I (21023) CANDIES_MATH: 
I (21023) CANDIES_MATH: ✅ คำตอบ:
I (21023) CANDIES_MATH:    มีลูกอมทั้งหมด 30 เม็ด
I (21033) CANDIES_MATH: 
I (21033) CANDIES_MATH: 🎨 ภาพประกอบ:
I (21033) CANDIES_MATH:    ถุงที่ 1: 🍬🍬🍬🍬🍬🍬 (6 เม็ด)
I (21033) CANDIES_MATH:    ถุงที่ 2: 🍬🍬🍬🍬🍬🍬 (6 เม็ด)
I (21043) CANDIES_MATH:    ถุงที่ 3: 🍬🍬🍬🍬🍬🍬 (6 เม็ด)
I (21043) CANDIES_MATH:    ถุงที่ 4: 🍬🍬🍬🍬🍬🍬 (6 เม็ด)
I (21043) CANDIES_MATH:    ถุงที่ 5: 🍬🍬🍬🍬🍬🍬 (6 เม็ด)
I (21043) CANDIES_MATH:    รวม:     30 เม็ด
I (21043) CANDIES_MATH: 
I (21043) CANDIES_MATH: 🔄 เปรียบเทียบกับการบวกซ้ำๆ:
I (21043) CANDIES_MATH:    การคูณ: 5 × 6 = 30
I (21043) CANDIES_MATH:    การบวกซ้ำๆ: 
I (21043) CANDIES_MATH:                   6
I (21053) CANDIES_MATH:                 + 6
I (21053) CANDIES_MATH:                 + 6
I (21053) CANDIES_MATH:                 + 6
I (21053) CANDIES_MATH:                 + 6 = 30
I (21053) CANDIES_MATH:    ผลลัพธ์เหมือนกัน! การคูณคือการบวกซ้ำๆ
I (21053) CANDIES_MATH: 
I (21053) CANDIES_MATH: 📊 ตารางสูตรคูณ 6:
I (21053) CANDIES_MATH:    1 × 6 = 6
I (21353) CANDIES_MATH:    2 × 6 = 12
I (21653) CANDIES_MATH:    3 × 6 = 18
I (21953) CANDIES_MATH:    4 × 6 = 24
I (22253) CANDIES_MATH:    5 × 6 = 30
I (22553) CANDIES_MATH:    6 × 6 = 36
I (22853) CANDIES_MATH:    7 × 6 = 42
I (23153) CANDIES_MATH:    8 × 6 = 48
I (23453) CANDIES_MATH:    9 × 6 = 54
I (23753) CANDIES_MATH:    10 × 6 = 60
I (24053) CANDIES_MATH: 
I (24053) CANDIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (24053) CANDIES_MATH:    ถ้ามีถุงลูกอม 3 ถุง ถุงละ 8 เม็ด
I (24053) CANDIES_MATH:    จะได้ลูกอม 3 × 8 = 24 เม็ด
I (24053) CANDIES_MATH: 
I (24053) CANDIES_MATH:    ถ้ามีถุงลูกอม 7 ถุง ถุงละ 4 เม็ด
I (24053) CANDIES_MATH:    จะได้ลูกอม 7 × 4 = 28 เม็ด
I (24053) CANDIES_MATH: 
I (24053) CANDIES_MATH: 🔄 เปรียบเทียบการดำเนินการ:
I (24053) CANDIES_MATH:    การบวก (+): เพิ่มจำนวน (เช่น ไข่ 4 + 2 = 6)
I (24053) CANDIES_MATH:    การลบ (-): ลดจำนวน (เช่น ของเล่น 8 - 3 = 5)
I (24063) CANDIES_MATH:    การคูณ (×): บวกซ้ำๆ (เช่น ลูกอม 5 × 6 = 30)
I (24063) CANDIES_MATH: 
I (24063) CANDIES_MATH: 🎓 แนวคิดขั้นสูง:
I (24063) CANDIES_MATH:    1. การคูณมีคุณสมบัติการสับเปลี่ยน:
I (24063) CANDIES_MATH:       5 × 6 = 6 × 5 = 30
I (24063) CANDIES_MATH:    2. การคูณด้วย 0 จะได้ 0 เสมอ:
I (24063) CANDIES_MATH:       5 × 0 = 0 (ไม่มีถุงลูกอม)
I (24063) CANDIES_MATH:    3. การคูณด้วย 1 จะได้ตัวเลขเดิม:
I (24063) CANDIES_MATH:       6 × 1 = 6 (มีถุงเดียว)
I (24063) CANDIES_MATH: 
I (24063) CANDIES_MATH: 📚 สิ่งที่เรียนรู้:
I (24063) CANDIES_MATH:    1. การคูณเลข (Multiplication): a × b = c
I (24073) CANDIES_MATH:    2. การใช้ for loop สำหรับการทำซ้ำ
I (24073) CANDIES_MATH:    3. ความสัมพันธ์ระหว่างการคูณและการบวกซ้ำๆ
I (24073) CANDIES_MATH:    4. คุณสมบัติพิเศษของการคูณ
I (24073) CANDIES_MATH:    5. การแสดงผลแบบตาราง
I (24073) CANDIES_MATH: 
I (24073) CANDIES_MATH: 🎉 จบโปรแกรมนับลูกอมในถุง!
I (24073) CANDIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 04_division_cookies
I (26073) main_task: Returned from app_main()
```

## 🎓 ท้าทาย

ลองแก้ไขโค้ดในไฟล์ `main/main.c`:

### 📝 แบบฝึกหัดที่ 1: เปลี่ยนจำนวนถุงลูกอม
```c
// หาบรรทัดนี้ในโค้ด:
int candy_bags = 5;         // จำนวนถุง
int candies_per_bag = 6;    // ลูกอมต่อถุง

// ลองเปลี่ยนเป็น:
int candy_bags = 7;         // เพิ่มเป็น 7 ถุง
int candies_per_bag = 8;    // ลูกอมถุงละ 8 เม็ด
```
### ผลการรัน
```
I (17689) CANDIES_MATH: 🧮 ขั้นตอนการคิด:
I (17689) CANDIES_MATH:    จำนวนถุง × ลูกอมต่อถุง
I (17699) CANDIES_MATH:    = 7 × 8
I (17699) CANDIES_MATH:    = 56 เม็ด
I (17699) CANDIES_MATH: 
I (17699) CANDIES_MATH: ✅ คำตอบ:
I (17709) CANDIES_MATH:    มีลูกอมทั้งหมด 56 เม็ด
I (17709) CANDIES_MATH: 
I (17709) CANDIES_MATH: 🎨 ภาพประกอบ:
I (17709) CANDIES_MATH:    ถุงที่ 1: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17709) CANDIES_MATH:    ถุงที่ 2: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17709) CANDIES_MATH:    ถุงที่ 3: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17709) CANDIES_MATH:    ถุงที่ 4: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17719) CANDIES_MATH:    ถุงที่ 5: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17719) CANDIES_MATH:    รวม:     56 เม็ด
I (17719) CANDIES_MATH: 
I (17719) CANDIES_MATH: 🔄 เปรียบเทียบกับการบวกซ้ำๆ:
I (17719) CANDIES_MATH:    การคูณ: 7 × 8 = 56
I (17719) CANDIES_MATH:    การบวกซ้ำๆ: 
I (17719) CANDIES_MATH:                   8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8 = 56
I (17719) CANDIES_MATH:    ผลลัพธ์เหมือนกัน! การคูณคือการบวกซ้ำๆ
I (17729) CANDIES_MATH: 
I (17729) CANDIES_MATH: 📊 ตารางสูตรคูณ 8:
I (17729) CANDIES_MATH:    1 × 8 = 8
I (18029) CANDIES_MATH:    2 × 8 = 16
I (18329) CANDIES_MATH:    3 × 8 = 24
I (18629) CANDIES_MATH:    4 × 8 = 32
I (18929) CANDIES_MATH:    5 × 8 = 40
I (19229) CANDIES_MATH:    6 × 8 = 48
I (19529) CANDIES_MATH:    7 × 8 = 56
I (19829) CANDIES_MATH:    8 × 8 = 64
I (20129) CANDIES_MATH:    9 × 8 = 72
I (20429) CANDIES_MATH:    10 × 8 = 80
I (20729) CANDIES_MATH: 
I (20729) CANDIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (20729) CANDIES_MATH:    ถ้ามีถุงลูกอม 3 ถุง ถุงละ 8 เม็ด
I (20739) CANDIES_MATH:    จะได้ลูกอม 3 × 8 = 24 เม็ด
I (20739) CANDIES_MATH: 
I (20739) CANDIES_MATH:    ถ้ามีถุงลูกอม 7 ถุง ถุงละ 4 เม็ด
I (20749) CANDIES_MATH:    จะได้ลูกอม 7 × 4 = 28 เม็ด
I (20749) CANDIES_MATH: 
I (20749) CANDIES_MATH: 🔄 เปรียบเทียบการดำเนินการ:
I (20759) CANDIES_MATH:    การบวก (+): เพิ่มจำนวน (เช่น ไข่ 4 + 2 = 6)
I (20759) CANDIES_MATH:    การลบ (-): ลดจำนวน (เช่น ของเล่น 8 - 3 = 5)
I (20759) CANDIES_MATH:    การคูณ (×): บวกซ้ำๆ (เช่น ลูกอม 5 × 6 = 30)
I (20769) CANDIES_MATH: 
I (20769) CANDIES_MATH: 🎓 แนวคิดขั้นสูง:
I (20769) CANDIES_MATH:    1. การคูณมีคุณสมบัติการสับเปลี่ยน:
I (20769) CANDIES_MATH:       7 × 8 = 8 × 7 = 56
I (20779) CANDIES_MATH:    2. การคูณด้วย 0 จะได้ 0 เสมอ:
I (20779) CANDIES_MATH:       7 × 0 = 0 (ไม่มีถุงลูกอม)
I (20779) CANDIES_MATH:    3. การคูณด้วย 1 จะได้ตัวเลขเดิม:
I (20779) CANDIES_MATH:       8 × 1 = 8 (มีถุงเดียว)
I (20779) CANDIES_MATH: 
I (20779) CANDIES_MATH: 📚 สิ่งที่เรียนรู้:
I (20779) CANDIES_MATH:    1. การคูณเลข (Multiplication): a × b = c
I (20779) CANDIES_MATH:    2. การใช้ for loop สำหรับการทำซ้ำ
I (20789) CANDIES_MATH:    3. ความสัมพันธ์ระหว่างการคูณและการบวกซ้ำๆ
I (20789) CANDIES_MATH:    4. คุณสมบัติพิเศษของการคูณ
I (20789) CANDIES_MATH:    5. การแสดงผลแบบตาราง
I (20789) CANDIES_MATH: 
I (20789) CANDIES_MATH: 🎉 จบโปรแกรมนับลูกอมในถุง!
I (20789) CANDIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 04_division_cookies
I (22799) main_task: Returned from app_main()
```

### 📝 แบบฝึกหัดที่ 2: เพิ่มลูกอมหลายรส
เพิ่มลูกอมหลายรส:
```c
int strawberry_bags = 3;    // ถุงรสสตรอเบอร์รี่
int orange_bags = 2;        // ถุงรสส้ม
int grape_bags = 4;         // ถุงรสองุ่น

int total_bags = strawberry_bags + orange_bags + grape_bags;
int total_candies = total_bags * candies_per_bag;

ESP_LOGI(TAG, "🍓 สตรอเบอร์รี่: %d ถุง = %d เม็ด", 
         strawberry_bags, strawberry_bags * candies_per_bag);
ESP_LOGI(TAG, "🍊 รสส้ม: %d ถุง = %d เม็ด", 
         orange_bags, orange_bags * candies_per_bag);
ESP_LOGI(TAG, "🍇 รสองุ่น: %d ถุง = %d เม็ด", 
         grape_bags, grape_bags * candies_per_bag);
```
### ผลการรัน
```
I (17689) CANDIES_MATH: 🧮 ขั้นตอนการคิด:
I (17689) CANDIES_MATH:    จำนวนถุง × ลูกอมต่อถุง
I (17699) CANDIES_MATH:    = 7 × 8
I (17699) CANDIES_MATH:    = 56 เม็ด
I (17699) CANDIES_MATH: 
I (17699) CANDIES_MATH: ✅ คำตอบ:
I (17709) CANDIES_MATH:    มีลูกอมทั้งหมด 56 เม็ด
I (17709) CANDIES_MATH: 
I (17709) CANDIES_MATH: 🎨 ภาพประกอบ:
I (17709) CANDIES_MATH:    ถุงที่ 1: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17709) CANDIES_MATH:    ถุงที่ 2: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17709) CANDIES_MATH:    ถุงที่ 3: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17709) CANDIES_MATH:    ถุงที่ 4: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17719) CANDIES_MATH:    ถุงที่ 5: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (17719) CANDIES_MATH:    รวม:     56 เม็ด
I (17719) CANDIES_MATH: 
I (17719) CANDIES_MATH: 🔄 เปรียบเทียบกับการบวกซ้ำๆ:
I (17719) CANDIES_MATH:    การคูณ: 7 × 8 = 56
I (17719) CANDIES_MATH:    การบวกซ้ำๆ: 
I (17719) CANDIES_MATH:                   8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8
I (17719) CANDIES_MATH:                 + 8 = 56
I (17719) CANDIES_MATH:    ผลลัพธ์เหมือนกัน! การคูณคือการบวกซ้ำๆ
I (17729) CANDIES_MATH: 
I (17729) CANDIES_MATH: 📊 ตารางสูตรคูณ 8:
I (17729) CANDIES_MATH:    1 × 8 = 8
I (18029) CANDIES_MATH:    2 × 8 = 16
I (18329) CANDIES_MATH:    3 × 8 = 24
I (18629) CANDIES_MATH:    4 × 8 = 32
I (18929) CANDIES_MATH:    5 × 8 = 40
I (19229) CANDIES_MATH:    6 × 8 = 48
I (19529) CANDIES_MATH:    7 × 8 = 56
I (19829) CANDIES_MATH:    8 × 8 = 64
I (20129) CANDIES_MATH:    9 × 8 = 72
I (20429) CANDIES_MATH:    10 × 8 = 80
I (20729) CANDIES_MATH: 
I (20729) CANDIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (20729) CANDIES_MATH:    ถ้ามีถุงลูกอม 3 ถุง ถุงละ 8 เม็ด
I (20739) CANDIES_MATH:    จะได้ลูกอม 3 × 8 = 24 เม็ด
I (20739) CANDIES_MATH: 
I (20739) CANDIES_MATH:    ถ้ามีถุงลูกอม 7 ถุง ถุงละ 4 เม็ด
I (20749) CANDIES_MATH:    จะได้ลูกอม 7 × 4 = 28 เม็ด
I (20749) CANDIES_MATH: 
I (20749) CANDIES_MATH: 🔄 เปรียบเทียบการดำเนินการ:
I (20759) CANDIES_MATH:    การบวก (+): เพิ่มจำนวน (เช่น ไข่ 4 + 2 = 6)
I (20759) CANDIES_MATH:    การลบ (-): ลดจำนวน (เช่น ของเล่น 8 - 3 = 5)
I (20759) CANDIES_MATH:    การคูณ (×): บวกซ้ำๆ (เช่น ลูกอม 5 × 6 = 30)
I (20769) CANDIES_MATH: 
I (20769) CANDIES_MATH: 🎓 แนวคิดขั้นสูง:
I (20769) CANDIES_MATH:    1. การคูณมีคุณสมบัติการสับเปลี่ยน:
I (20769) CANDIES_MATH:       7 × 8 = 8 × 7 = 56
I (20779) CANDIES_MATH:    2. การคูณด้วย 0 จะได้ 0 เสมอ:
I (20779) CANDIES_MATH:       7 × 0 = 0 (ไม่มีถุงลูกอม)
I (20779) CANDIES_MATH:    3. การคูณด้วย 1 จะได้ตัวเลขเดิม:
I (20779) CANDIES_MATH:       8 × 1 = 8 (มีถุงเดียว)
I (20779) CANDIES_MATH: 
I (20779) CANDIES_MATH: 📚 สิ่งที่เรียนรู้:
I (20779) CANDIES_MATH:    1. การคูณเลข (Multiplication): a × b = c
I (20779) CANDIES_MATH:    2. การใช้ for loop สำหรับการทำซ้ำ
I (20789) CANDIES_MATH:    3. ความสัมพันธ์ระหว่างการคูณและการบวกซ้ำๆ
I (20789) CANDIES_MATH:    4. คุณสมบัติพิเศษของการคูณ
I (20789) CANDIES_MATH:    5. การแสดงผลแบบตาราง
I (20789) CANDIES_MATH: 
I (20789) CANDIES_MATH: 🎉 จบโปรแกรมนับลูกอมในถุง!
I (20789) CANDIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 04_division_cookies
I (22799) main_task: Returned from app_main()
```
### 📝 แบบฝึกหัดที่ 3: สร้างตารางสูตรคูณ
เพิ่มการแสดงตารางสูตรคูณ:
```c
ESP_LOGI(TAG, "📊 ตารางสูตรคูณของ %d:", candies_per_bag);
for (int i = 1; i <= 10; i++) {
    ESP_LOGI(TAG, "   %d x %d = %d", i, candies_per_bag, i * candies_per_bag);
}
```
### ผลการรัน
```
I (16538) CANDIES_MATH: 🧮 ขั้นตอนการคิด:
I (16538) CANDIES_MATH:    จำนวนถุง × ลูกอมต่อถุง
I (16538) CANDIES_MATH:    = 7 × 8
I (16538) CANDIES_MATH:    = 56 เม็ด
I (16538) CANDIES_MATH: 
I (16538) CANDIES_MATH: ✅ คำตอบ:
I (16538) CANDIES_MATH:    มีลูกอมทั้งหมด 56 เม็ด
I (16538) CANDIES_MATH: 
I (16538) CANDIES_MATH: 🎨 ภาพประกอบ:
I (16538) CANDIES_MATH:    ถุงที่ 1: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (16538) CANDIES_MATH:    ถุงที่ 2: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (16538) CANDIES_MATH:    ถุงที่ 3: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (16538) CANDIES_MATH:    ถุงที่ 4: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (16548) CANDIES_MATH:    ถุงที่ 5: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (16548) CANDIES_MATH:    รวม:     56 เม็ด
I (16548) CANDIES_MATH: 
I (16548) CANDIES_MATH: 🔄 เปรียบเทียบกับการบวกซ้ำๆ:
I (16548) CANDIES_MATH:    การคูณ: 7 × 8 = 56
I (16548) CANDIES_MATH:    การบวกซ้ำๆ: 
I (16548) CANDIES_MATH:                   8
I (16548) CANDIES_MATH:                 + 8
I (16548) CANDIES_MATH:                 + 8
I (16548) CANDIES_MATH:                 + 8
I (16548) CANDIES_MATH:                 + 8
I (16548) CANDIES_MATH:                 + 8
I (16548) CANDIES_MATH:                 + 8 = 56
I (16548) CANDIES_MATH:    ผลลัพธ์เหมือนกัน! การคูณคือการบวกซ้ำๆ
I (16558) CANDIES_MATH: 
I (16558) CANDIES_MATH: 📊 ตารางสูตรคูณ 8:
I (16558) CANDIES_MATH:    1 × 8 = 8
I (16858) CANDIES_MATH:    2 × 8 = 16
I (17158) CANDIES_MATH:    3 × 8 = 24
I (17458) CANDIES_MATH:    4 × 8 = 32
I (17758) CANDIES_MATH:    5 × 8 = 40
I (18058) CANDIES_MATH:    6 × 8 = 48
I (18358) CANDIES_MATH:    7 × 8 = 56
I (18658) CANDIES_MATH:    8 × 8 = 64
I (18958) CANDIES_MATH:    9 × 8 = 72
I (19258) CANDIES_MATH:    10 × 8 = 80
I (19558) CANDIES_MATH: 
I (19558) CANDIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (19558) CANDIES_MATH:    ถ้ามีถุงลูกอม 3 ถุง ถุงละ 8 เม็ด
I (19558) CANDIES_MATH:    จะได้ลูกอม 3 × 8 = 24 เม็ด
I (19558) CANDIES_MATH: 
I (19558) CANDIES_MATH:    ถ้ามีถุงลูกอม 7 ถุง ถุงละ 4 เม็ด
I (19558) CANDIES_MATH:    จะได้ลูกอม 7 × 4 = 28 เม็ด
I (19558) CANDIES_MATH: 
I (19558) CANDIES_MATH: 🔄 เปรียบเทียบการดำเนินการ:
I (19558) CANDIES_MATH:    การบวก (+): เพิ่มจำนวน (เช่น ไข่ 4 + 2 = 6)
I (19558) CANDIES_MATH:    การลบ (-): ลดจำนวน (เช่น ของเล่น 8 - 3 = 5)
I (19568) CANDIES_MATH:    การคูณ (×): บวกซ้ำๆ (เช่น ลูกอม 5 × 6 = 30)
I (19568) CANDIES_MATH: 
I (19568) CANDIES_MATH: 🎓 แนวคิดขั้นสูง:
I (19568) CANDIES_MATH:    1. การคูณมีคุณสมบัติการสับเปลี่ยน:
I (19568) CANDIES_MATH:       7 × 8 = 8 × 7 = 56
I (19578) CANDIES_MATH:    2. การคูณด้วย 0 จะได้ 0 เสมอ:
I (19578) CANDIES_MATH:       7 × 0 = 0 (ไม่มีถุงลูกอม)
I (19578) CANDIES_MATH:    3. การคูณด้วย 1 จะได้ตัวเลขเดิม:
I (19578) CANDIES_MATH:       8 × 1 = 8 (มีถุงเดียว)
I (19588) CANDIES_MATH: 
I (19588) CANDIES_MATH: 📚 สิ่งที่เรียนรู้:
I (19588) CANDIES_MATH:    1. การคูณเลข (Multiplication): a × b = c
I (19588) CANDIES_MATH:    2. การใช้ for loop สำหรับการทำซ้ำ
I (19588) CANDIES_MATH:    3. ความสัมพันธ์ระหว่างการคูณและการบวกซ้ำๆ
I (19608) CANDIES_MATH:    4. คุณสมบัติพิเศษของการคูณ
I (19608) CANDIES_MATH:    5. การแสดงผลแบบตาราง
I (19608) CANDIES_MATH: 
I (19608) CANDIES_MATH: 🎉 จบโปรแกรมนับลูกอมในถุง!
I (19608) CANDIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 04_division_cookies
I (19608) CANDIES_MATH: 🍓 สตรอเบอร์รี่: 3 ถุง = 24 เม็ด
I (19608) CANDIES_MATH: 🍊 รสส้ม: 2 ถุง = 16 เม็ด
I (19608) CANDIES_MATH: 🍇 รสองุ่น: 4 ถุง = 32 เม็ด
I (21608) main_task: Returned from app_main()
```
### 📝 แบบฝึกหัดที่ 4: แจกลูกอมให้เพื่อน
คำนวณการแจกลูกอม:
```c
int friends = 12;           // จำนวนเพื่อน
int candies_per_friend = total_candies / friends;  // ลูกอมต่อคน
int remaining_candies = total_candies % friends;   // ลูกอมที่เหลือ

ESP_LOGI(TAG, "👥 แจกให้เพื่อน %d คน:", friends);
ESP_LOGI(TAG, "   คนละ %d เม็ด", candies_per_friend);
ESP_LOGI(TAG, "   เหลือ %d เม็ด", remaining_candies);
```
### ผลการรัน
```
I (18084) CANDIES_MATH: 🧮 ขั้นตอนการคิด:
I (18084) CANDIES_MATH:    จำนวนถุง × ลูกอมต่อถุง
I (18084) CANDIES_MATH:    = 7 × 8
I (18084) CANDIES_MATH:    = 56 เม็ด
I (18084) CANDIES_MATH: 
I (18084) CANDIES_MATH: ✅ คำตอบ:
I (18084) CANDIES_MATH:    มีลูกอมทั้งหมด 56 เม็ด
I (18084) CANDIES_MATH: 
I (18084) CANDIES_MATH: 🎨 ภาพประกอบ:
I (18084) CANDIES_MATH:    ถุงที่ 1: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (18084) CANDIES_MATH:    ถุงที่ 2: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (18084) CANDIES_MATH:    ถุงที่ 3: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (18094) CANDIES_MATH:    ถุงที่ 4: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (18094) CANDIES_MATH:    ถุงที่ 5: 🍬🍬🍬🍬🍬🍬 (8 เม็ด)
I (18094) CANDIES_MATH:    รวม:     56 เม็ด
I (18094) CANDIES_MATH: 
I (18094) CANDIES_MATH: 🔄 เปรียบเทียบกับการบวกซ้ำๆ:
I (18094) CANDIES_MATH:    การคูณ: 7 × 8 = 56
I (18094) CANDIES_MATH:    การบวกซ้ำๆ: 
I (18104) CANDIES_MATH:                   8
I (18104) CANDIES_MATH:                 + 8
I (18104) CANDIES_MATH:                 + 8
I (18104) CANDIES_MATH:                 + 8
I (18104) CANDIES_MATH:                 + 8
I (18104) CANDIES_MATH:                 + 8
I (18104) CANDIES_MATH:                 + 8 = 56
I (18104) CANDIES_MATH:    ผลลัพธ์เหมือนกัน! การคูณคือการบวกซ้ำๆ
I (18104) CANDIES_MATH: 
I (18104) CANDIES_MATH: 📊 ตารางสูตรคูณ 8:
I (18104) CANDIES_MATH:    1 × 8 = 8
I (18404) CANDIES_MATH:    2 × 8 = 16
I (18704) CANDIES_MATH:    3 × 8 = 24
I (19004) CANDIES_MATH:    4 × 8 = 32
I (19304) CANDIES_MATH:    5 × 8 = 40
I (19604) CANDIES_MATH:    6 × 8 = 48
I (19904) CANDIES_MATH:    7 × 8 = 56
I (20204) CANDIES_MATH:    8 × 8 = 64
I (20504) CANDIES_MATH:    9 × 8 = 72
I (20804) CANDIES_MATH:    10 × 8 = 80
I (21104) CANDIES_MATH: 
I (21104) CANDIES_MATH: 💡 ตัวอย่างเพิ่มเติม:
I (21104) CANDIES_MATH:    ถ้ามีถุงลูกอม 3 ถุง ถุงละ 8 เม็ด
I (21104) CANDIES_MATH:    จะได้ลูกอม 3 × 8 = 24 เม็ด
I (21104) CANDIES_MATH: 
I (21104) CANDIES_MATH:    ถ้ามีถุงลูกอม 7 ถุง ถุงละ 4 เม็ด
I (21104) CANDIES_MATH:    จะได้ลูกอม 7 × 4 = 28 เม็ด
I (21104) CANDIES_MATH: 
I (21104) CANDIES_MATH: 🔄 เปรียบเทียบการดำเนินการ:
I (21104) CANDIES_MATH:    การบวก (+): เพิ่มจำนวน (เช่น ไข่ 4 + 2 = 6)
I (21104) CANDIES_MATH:    การลบ (-): ลดจำนวน (เช่น ของเล่น 8 - 3 = 5)
I (21104) CANDIES_MATH:    การคูณ (×): บวกซ้ำๆ (เช่น ลูกอม 5 × 6 = 30)
I (21114) CANDIES_MATH: 
I (21114) CANDIES_MATH: 🎓 แนวคิดขั้นสูง:
I (21114) CANDIES_MATH:    1. การคูณมีคุณสมบัติการสับเปลี่ยน:
I (21114) CANDIES_MATH:       7 × 8 = 8 × 7 = 56
I (21114) CANDIES_MATH:    2. การคูณด้วย 0 จะได้ 0 เสมอ:
I (21114) CANDIES_MATH:       7 × 0 = 0 (ไม่มีถุงลูกอม)
I (21114) CANDIES_MATH:    3. การคูณด้วย 1 จะได้ตัวเลขเดิม:
I (21114) CANDIES_MATH:       8 × 1 = 8 (มีถุงเดียว)
I (21114) CANDIES_MATH: 
I (21114) CANDIES_MATH: 📚 สิ่งที่เรียนรู้:
I (21114) CANDIES_MATH:    1. การคูณเลข (Multiplication): a × b = c
I (21114) CANDIES_MATH:    2. การใช้ for loop สำหรับการทำซ้ำ
I (21124) CANDIES_MATH:    3. ความสัมพันธ์ระหว่างการคูณและการบวกซ้ำๆ
I (21124) CANDIES_MATH:    4. คุณสมบัติพิเศษของการคูณ
I (21124) CANDIES_MATH:    5. การแสดงผลแบบตาราง
I (21124) CANDIES_MATH: 
I (21124) CANDIES_MATH: 🎉 จบโปรแกรมนับลูกอมในถุง!
I (21124) CANDIES_MATH: 📖 อ่านต่อในโปรเจคถัดไป: 04_division_cookies
I (21124) CANDIES_MATH: 🍓 สตรอเบอร์รี่: 3 ถุง = 24 เม็ด
I (21124) CANDIES_MATH: 🍊 รสส้ม: 2 ถุง = 16 เม็ด
I (21134) CANDIES_MATH: 🍇 รสองุ่น: 4 ถุง = 32 เม็ด
I (21134) CANDIES_MATH: 👥 แจกให้เพื่อน 12 คน:
I (21134) CANDIES_MATH:    คนละ 6 เม็ด
I (21134) CANDIES_MATH:    เหลือ 0 เม็ด
I (23134) main_task: Returned from app_main()
```
### 🏆 เป้าหมาย:
- [ ] เปลี่ยนจำนวนถุงลูกอมได้
- [ ] เพิ่มลูกอมหลายรสได้
- [ ] สร้างตารางสูตรคูณได้
- [ ] คำนวณการแจกลูกอมได้
- [ ] เข้าใจการคูณ, หาร, และเศษ (%)

## ✅ ผลลัพธ์ที่คาดหวัง

```
=== ลูกอมในถุง ===
จำนวนถุง: 5 ถุง
ลูกอมต่อถุง: 6 เม็ด
ลูกอมทั้งหมด: 5 × 6 = 30 เม็ด

การบวกซ้ำๆ: 6 + 6 + 6 + 6 + 6 = 30
```
