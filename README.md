# Hash_Tables_Project
## CLI application that keeps records about students, exams and their results.

The application user can add a student, add an exam, add a subject, add an exam result, retrieve all exams for a specific date, retrieve exams by date and subject name, retrieve all exams by one student. The emphasis is on the asymptotic complexity of operations (O(n)) and the efficient use of memory. The structure in which the data is placed is implemented using two hash tables, one that contains data about students (each student has its own key and a list of pointers to passed Exams), the other that contains data about exams (the key is the date and the list of objects of type Exam). This type of data organization enables all operations that the user can perform to be of O(1) complexity.

### Objects used in application

* Student( int index, std::vector<<Ispit>::iterator> listaPointeraDoIspita),
* Ispit( Student* student, int kljucPredmeta, int datum)

* MapaStudenata( std::unordered_map<int, Student>)
* MapaIspita(std::unordered_map<int, std::unordered_map<int kljucDatum, std::vector<Ispit>>>)

* Program(MapaStudenata, MapaIspita)
  
### Functions/Methods

The application is organized with a menu function that does different things depending on what the user decides, every option calls a different method on the object program. 

* option1: Create object Student and add it to MapaStudenata
* option2: Create object Ispit
* option3: Create object Predmet
* option4: Add exam result to MapaIspita, if there is no subject with that key, create it
* option5: fetch all exams with specific date
* option6: fetch all students for specific date and subject name(key)
* option7: fetch by index(one student) all exams and average grade
* option8: exit
  
 
[application view](https://www.canva.com/design/DAFc1gP5reI/D_UcsAYOnSQ_ROgcQDq4bQ/view?utm_content=DAFc1gP5reI&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)
