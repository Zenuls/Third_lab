# Third_lab
Предметная область: Больница

Описание предметной области: Данная проектная область представляет собой больницу, включающую в себя персонал, пациентов, кабинеты, ресурсы больницы, отчёт

Анализ сущностей:

Больница (location, list_doctors, list_patients, rooms)
Она включает в себя местоположение (location:string), список докторов (list_doctors: vector<int>), список пациентов (list_patients: vector<string>), кабинеты (rooms: vector<string>).
Методы для "Больница":
addDoctor(doctor: Doctor): Метод для добавления нового доктора в список докторов больницы.
removeDoctor(doctor: Doctor): Метод для удаления доктора из списка докторов больницы.
addPatient(patient: Patient): Метод для добавления нового пациента в список пациентов больницы.

Мед.персонал (Full_Name, Specialization, Room)
Включает в себя ФИО (Full_Name: string), специализацию (Specialization: string), и номер кабинета (Room: int)
Методы для "Мед.персонал": 
changeSpecialization(Specialization: string): Метод для изменения специализации медицинского персонала.
changeRoom(Room: int): Метод для изменения номера кабинета медицинского персонала.

Пациент  (Full_Name, Date_of_Birth, Gender, Phone_Number)
Включает в себя ФИО (Full_Name: string), Дату рождения (Date_of_Birth: string), Пол (Gender: bool), Номер телефона (Phone_Number: string)
Методы для "Пациент":
createMedicalRecord(doctor: Doctor, date: string, information: string): Метод для создания медицинской записи о визите пациента к доктору.


Кабинеты (Number, Doctor)
Включает в себя номер кабинета (Room: int) и ФИО доктора (Full_Name: string)
Методы для "Кабинеты":
assignDoctor(doctor: Doctor): Метод для назначения доктора на определенный кабинет


Ресурсы больницы (Equipment, Medications)
Включает в себя оборудование (Equipment: string) и медикаменты (Medications: string)
Методы для "Ресурсы больницы":
addEquipment(equipment: string): Метод для добавления оборудования в ресурсы больницы.
addMedication(medication: string): Метод для добавления медикаментов в ресурсы больницы.


Отчёт (Type, Date, Information)
Включает в себя тип отчёта (Type: string), дату создания (Date: string), информация (Information: string)
Методы для "Отчёт":
generateReport(Full_Name: string, type: string, date: string, information: string): Метод для создания мед.персоналом отчёта с указанием типа, даты и информации.
