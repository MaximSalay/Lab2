import datetime

def create_student():
    student = {}
    student["last_name"] = input("Введите фамилию студента: ")
    student["first_name"] = input("Введите имя студента: ")
    year = int(input("Введите год рождения студента: "))
    month = int(input("Введите месяц рождения студента: "))
    day = int(input("Введите число рождения студента: "))
    student["birthdate"] = datetime.date(year, month, day)
    
    student["record_book"] = []
    num_subjects = int(input("Введите количество предметов в зачетке студента (от 3 до 5): "))
    for i in range(num_subjects):
        record = {}
        record["subject"] = input("Введите предмет: ")
        year = int(input("Введите год экзамена по предмету: "))
        month = int(input("Введите месяц экзамена по предмету: "))
        day = int(input("Введите число экзамена по предмету: "))
        record["exam_date"] = datetime.date(year, month, day)
        record["teacher"] = input("Введите ФИО преподавателя: ")
        student["record_book"].append(record)
    
    return student

def main():
    students = []
    num_students = int(input("Введите количество студентов в учебной группе: "))
    
    for i in range(num_students):
        print(f"Введите информацию о студенте {i+1}:")
        student = create_student()
        students.append(student)
    
    min_student = min(students, key=lambda x: x["birthdate"])
    max_student = max(students, key=lambda x: x["birthdate"])
    
    print(f"Самый младший студент: {min_student['last_name']} {min_student['first_name']}, Дата рождения: {min_student['birthdate']}")
    print(f"Самый старший студент: {max_student['last_name']} {max_student['first_name']}, Дата рождения: {max_student['birthdate']}")

if name == "main":
    main()
