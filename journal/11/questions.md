# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > Allows us to use the properties and methods of one class on another class

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > a class will inherit all the methods and properties on the parent

3. How does ***accessibility*** affect inheritance?

  > some classes are unable to be used and only able to be inherited

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > primary key is the unique property that distinguishes data in a database

5. What is an ***alias***?

  > allows an instance of a class to set the datatypes on propeties to fit its use case

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > SELECT
    *
    FROM PATIENTS
    JOIN patient_doctors ON patient_doctors.patientId = id
    JOIN doctors ON doctors.id = doctor.id
    
