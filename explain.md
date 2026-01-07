//node 01-variables.js //

=== Variables & Data Types Practice ===

Constants:
MAX_USERS: 100
PI: 3.14159

Variable (let):
count after increment: 2

=== Primitive Data Types ===
Numbers: 25 5.9 -10
Strings: John Doe
Booleans: isStudent: true isTeacher: false
null: null
undefined: undefined

=== Object Data Types ===
Array: [ 'apple', 'banana', 'orange' ]
First fruit: apple
Array length: 3
Object: { name: 'John', age: 25, city: 'Bangkok', isStudent: true }
Person name: John
Person age: 25

=== typeof Operator ===
typeof 25: number
typeof 'hello': string
typeof true: boolean
typeof undefined: undefined
typeof []: object
typeof {}: object
typeof (() => {}): function

=== Type Coercion ===
'5' + 2: 52
'5' - 2: 3
'5' \* 2: 10
true + 1: 2

Explicit coercion:
String(25): 25
Number('25'): 25
Boolean(1): true
Boolean(0): false
Boolean(''): false
Boolean('hello'): true

=== Challenge: Person Object ===
Student object:
{
firstName: 'Alice',
lastName: 'Smith',
age: 20,
gpa: 3.8,
courses: [ 'HTML', 'CSS', 'JavaScript' ],
isActive: true,
getFullName: [Function: getFullName],
getInfo: [Function: getInfo]
}
Full name: Alice Smith
Info: Alice Smith, Age: 20, GPA: 3.8
Courses: HTML, CSS, JavaScript

=== Truthy vs Falsy ===
Falsy values:
0: false
"": false
null: false
undefined: false
false: false
NaN: false

Truthy values:
1: true
hello: true
true: true
[]: true
{}: true
() => {}: true

✅ Activity 1 completed!

::อธิบาย::
การทำงานของโค้ดนี้คือการรับคำสั่งทีละบรรทัด จากบนลงล่าง โดยใช้ฟังก์ชั่น console.log เป็นตัวสั่งให้พิมพ์ผลลัพธ์ ขณะนั้นออกมาแสดงบนจอ
variable ประกาศค่าคงที่และตัวแปรนับเลข
Primitive เก็บข้อมูลพื้นฐาน
Arrays เก็บรายการ
Objects เก็บประวัติ
typeof สั่งตรวจสอบข้อมูลว่าเป็นชนิดอะไร
truthy/falsy วนลูปเช็คค่าต่างๆว่าถ้าแปลงเป็น boolean แล้วจะเป็นจริงหรือเท็จ

// node 02-functions.js //

=== Functions & Arrow Functions Practice ===

Function Declaration:
Hello, John!
Hello, Alice!

Function Expression:
add(5, 3): 8
add(10, 20): 30

Arrow Function (full syntax):
multiply(4, 5): 20
Arrow Function (shorthand):
square(5): 25
double(10): 20
getRandom(): 35

Default Parameters:
Anonymous is 0 years old from Unknown
John is 0 years old from Unknown
John is 25 years old from Unknown
John is 25 years old from Bangkok

Rest Parameters:
sum(1, 2, 3): 6
sum(5, 10, 15, 20): 50
sum(): 0
sumWithReduce(2, 4, 6, 8): 20

Destructuring Parameters:
Alice, 22 years old, from Chiang Mai

Validation Function:
{ valid: false, message: 'Email is required' }
{ valid: false, message: 'Invalid email format' }
{ valid: false, message: 'Missing domain extension' }
{ valid: true, message: 'Email is valid' }

Returning Objects:
{
firstName: 'John',
lastName: 'Doe',
age: 30,
email: 'john.doe@example.com',
getFullName: [Function: getFullName],
getAge: [Function: getAge]
}
Email: john.doe@example.com
Full name: John Doe

Callback Function:
Original: [ 1, 2, 3, 4, 5 ]
Doubled: [ 2, 4, 6, 8, 10 ]
Squared: [ 1, 4, 9, 16, 25 ]

Challenge: Calculator
5 + 3 = 8
10 - 4 = 6
6 \* 7 = 42
20 / 4 = 5
2 ^ 10 = 1024
Using operate('add', 5, 3) = 8

✅ Activity 2 completed!

::อธิบาย::
Default Parameters กำหนดค่าให้ตัวแปรไว้เลย ถ้าคนเรียกใช้ไม่ส่งมาก็ไม่ error
Rest parameters รับค่าได้ไม่จำกัด
Destructuring Parameters ระบุ {name, age} เพื่อดึงเฉพาะค่านั้นออกมาใช้ได้เลย
Early return เช็ค error ก่อน ถ้าผิดให้จบงานทันที
call back ฝากฟังก์ชั่นไปรันในอีกฟังก์ชั่น
calculator รวมฟังก์ชั่นบวก ลบ คูณ หาร ไว้ในทีเดียว

// node 03-control-flow.js //

=== Control Flow & Logic Practice ===

Age Classification:
Age 5: Child
Age 15: Teenager
Age 25: Adult
Age 65: Senior

Day Names:
Day 1: Monday
Day 2: Tuesday
Day 3: Wednesday
Day 4: Thursday
Day 5: Friday
Day 6: Saturday
Day 7: Sunday
Day 8: Unknown day

Weekday/Weekend:
Monday (1): Weekday
Saturday (6): Weekend

Logical Operators:
Can drive: true
Is special age: true
Is not adult: false

Short-Circuit Evaluation:
User name: John
User profile: undefined

Grading System:
Score 95: Grade A
Score 85: Grade B
Score 75: Grade C
Score 65: Grade D
Score 55: Grade F

Form Validation:
Valid user: { isValid: true, errors: [] }
Invalid user: {
isValid: false,
errors: [
'Name must be at least 3 characters',
'Valid email is required',
'Must be 18 or older',
'Password must be at least 6 characters',
'Must agree to terms'
]
}

Challenge: Traffic Light
red: 🛑🛑 STOP
yellow: 🟨🟨 SLOW DOWN
green: 🟢🟢 GO
blue: ❓ INVALID COLOR

✅ Activity 3 completed!

::อธิบาย::

if/else เช็คเงื่อนไข
Switch กระโดดไปทำคำสั่งที่ตรงกับค่าตัวแปร
Logic ops รวมเงื่อนไข
Short-circuit กัน error เมื่อข้อมูลเป็น null
Grading เช็คช่วงคะแนนเพื่อระบุเกรด
Validation ไล่เช้คข้อมูล ถ้า error จะเก็บไว้ในรายการ
Traffic Light จับคู่สีไฟจราจรกับข้อความเตือนด้วย switch csae

// node 04-loops.js //

=== Loops & Array Methods Practice ===

For loop (0-4):
i = 0
i = 1
i = 2
i = 3
i = 4

While loop (count down):
5...
4...
3...
2...
1...
Blastoff! 🚀🚀

For...of loop (fruits):

- apple
- banana
- orange

For...in loop (person properties):
name: John
age: 25
city: Bangkok

forEach (with index):
0: apple
1: banana
2: orange

map - transform elements:
Original: [ 1, 2, 3, 4, 5 ]
Doubled: [ 2, 4, 6, 8, 10 ]
Squared: [ 1, 4, 9, 16, 25 ]
As strings: [ 'Number: 1', 'Number: 2', 'Number: 3', 'Number: 4', 'Number: 5' ]

filter - select elements:
Even numbers: [ 2, 4 ]
Odd numbers: [ 1, 3, 5 ]
Numbers > 2: [ 3, 4, 5 ]

reduce - accumulate:
Sum: 15
Product: 120
Concatenated: 12345
Word count: { apple: 3, banana: 1, orange: 1 }

Method chaining:
Even numbers squared: 2²=4, 4²=16, 6²=36, 8²=64, 10²=100
Average: 30

Challenge: Student Analysis
Students: [
{ name: 'Alice', score: 95 },
{ name: 'Bob', score: 75 },
{ name: 'Charlie', score: 85 },
{ name: 'Diana', score: 92 },
{ name: 'Eve', score: 88 }
]
Names: Alice, Bob, Charlie, Diana, Eve
High scorers: Alice (95), Charlie (85), Diana (92), Eve (88)
Class average: 87.00
Top scorer: Alice (95)
Summary (sorted):
Alice: 95 (A)
Diana: 92 (A)
Eve: 88 (B)
Charlie: 85 (B)
Bob: 75 (C)

✅ Activity 4 completed!

::อธิบาย::
For loop วนลูปโดยคุมตัวนับเอง(i=0 ถึง i=5)
while loop วนลูปตราบใดที่เงื่อนไขเป็นจริง
for..of วนลูปดึงค่า array ออกมาใช้
for..in วนลูปดึงชื่อ key ใน object
map สร้าง array ใหม่ โดยเปลี่ยนค่าข้อมูลเดิมทุกตัว
filter สร้าง array ใหม่โดยเลือกแค่ตัวที่ผ่านเงื่อนไข
reduce ยุบรวบข้อมูลใน array ให้เหลือผลลลัพธ์เดียว
student challenge ใช้ map/filter/reduce/sort เพื่อวิเคราะห์และสรุปผลสอบนักเรียน

// node 05-integration.js //

🎯🎯 === QUIZ APPLICATION === 🎯🎯

QUIZ RESULTS:
────────────────────────────────────────────────────────────
Q1: What is 5 + 3?
Your answer: 9
Correct answer: 8
❌ WRONG

Q2: What is the capital of Thailand?
Your answer: Chiang Mai
Correct answer: Bangkok
❌ WRONG

Q3: What is the largest planet?
Your answer: Mars
Correct answer: Jupiter
❌ WRONG

Q4: What is 2^8?
Your answer: 64
Correct answer: 256
❌ WRONG

Q5: Which is NOT a JavaScript data type?
Your answer: boolean
Correct answer: class
❌ WRONG

────────────────────────────────────────────────────────────
FINAL SCORE: 0/5 (0.0%)
GRADE: F

FEEDBACK:
💪💪 Keep practicing. You'll improve!

📊📊 STATISTICS:
Total questions: 5
Correct: 0
Incorrect: 5
Success rate: 0.0%

Answer breakdown:
✅ Correct: 0
❌ Incorrect: 5

✅ All activities completed!
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

::อธิบาย::
quiz data เก็บโจทยืและเฉลยในรูปแบบ array object
simulation วนลูปสร้างคำตอบจำลองด้วยการสุ่ม
Storage เก็บผลการตรวจคำตอบลง array Results
Display loop วนลูปโชซ์ผลสอบทีละข้อถ้าผิดจะโชว์เฉลย
Scoring ใช้ filter นับจำนวนข้อที่ตอบถูก
Grading ใช้ if/else แปลงคะแนนเป็นเกรด A-Falsy
Feedback ให้คำชมตามช่วงคะแนนที่ได้
Statistics ใช้ reduce สรุปยอดรวม ถูก/ผิด
