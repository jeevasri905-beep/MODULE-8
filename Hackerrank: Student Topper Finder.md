# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
```
student_marks = {
    "Arjun": [78, 82, 91, 67, 88],
    "Meera": [90, 85, 92, 80, 89],
    "Rahul": [65, 70, 72, 60, 68],
    "Sara":  [88, 90, 94, 92, 89]
}

total_marks = {}

for name, marks in student_marks.items():
    total_marks[name] = sum(marks)

topper = max(total_marks, key=total_marks.get)

print("Total Marks:", total_marks)
print("Topper:", topper, "with", total_marks[topper])

```
## OUTPUT
<img width="799" height="261" alt="Screenshot 2025-11-28 102005" src="https://github.com/user-attachments/assets/9101cd76-c04b-40c6-9f99-003ed09249bc" />

## RESULT
Thus, the program is executed successfully.
