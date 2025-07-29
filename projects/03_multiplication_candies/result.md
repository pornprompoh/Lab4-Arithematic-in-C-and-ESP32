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
