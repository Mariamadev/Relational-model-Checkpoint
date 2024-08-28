1. Table : Hotel
Hotel_Id (PK)
Hotel_name
2. Table : Type
Type_Id (PK)
Type_Name
3. Table : Room
Room_Id (PK)
Floor
Hotel_Id (FK) -> Hotel.Hotel_Id
Type_Id (FK) -> Type.Type_Id
Category_Id (FK) -> Category.Category_Id
4. Table : Category
Category_Id (PK)
Category_Name
Price
Beds_numbers
5. Table : Employee
Employee_Id (PK)
Employee_Name
Employee_Speciality
Hotel_Id (FK) -> Hotel.Hotel_Id
Supervisor_Id (FK) -> Employee.Employee_Id (auto-référence pour le relation "leads")
Relations :
Hotel peut avoir plusieurs Room (1
)
Chaque Room appartient à un seul Hotel (N:1)
Chaque Room appartient à un seul Type (N:1)
Chaque Room appartient à une seule Category (N:1)
Employee travaille dans un seul Hotel (N:1)
Hotel peut avoir plusieurs Employee (1
)
Un Employee peut superviser plusieurs Employee (1
)
Chaque Employee est supervisé par un seul Employee (N:1)