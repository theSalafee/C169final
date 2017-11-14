# C169final
For this assessment, you will write a program containing two classes named student and roster, respectively. The program will maintain a current roster of students within a given course. Student data for the program includes student ID, first name, last name, e­mail address, age, and array of grades. The program you create will read a list of five students, with one of the students being yourself, and use the series of method calls below (see part B3 below). A well ­designed program would use the principles of encapsulation and information hiding


package com.WGUroster;
//package Roster;
//import java.util.ArrayList;


/** This program maintains a current roster of students within a course. */
/* Author: Jayson E. Bush */
/* Western Governors' University C169 Performance Assessment */
/* Date: 2017.11.13 */
/* Version 1.0 */
/* IDE: IntelliJ IDEA Community Ed. */


public class Student
{
    /*
        SECTION B.1 REQUIREMENTS: FOR THE STUDENT OBJECT CLASS, DO THE FOLLOWING. INCLUDE THE FOLLOWING INSTANCE
        VARIABLES THAT DESCRIBE EACH STUDENT
    */

    private int student_ID;
    private String firstName;
    private String lastName ;
    private String email_address;
    private int age ;
    private int[] student_grades; // Array of Student grades.

    public static void main(String[] args)
    {
        /*
            SECTION B.2-A & B REQUIREMENTS: INCLUDE THE FOLLOWING METHODS IN THE STUDENT CLASS:
            A. AN ACCESSOR (I.E., GETTER) FOR EACH INSTANCE VARIABLE FROM PART B.1.
            B. A MUTATOR (I.E., SETTER) FOR EACH INSTANCE VARIABLE FROM PART B.1.
        */


        //Accessor
        public int getStudent_ID()
        {
            return student_ID;
        }
        public String getFirstName()
        {
            return firstName;
        }
        public String getLastName()
        {
            return lastName;
        }
        public String getEmail_address()
        {
            return email_address;
        }
        public int getAge()
        {
            return age;
        }
        public int[] getStudent_grades()
        {
            return student_grades;
        }

        //Mutator
        public void setStudent_ID (int student_ID)
        {
            this.student_ID = student_ID ;
        }
        public void setFirstName (String firstName)
        {
            this.firstName = firstName ;
        }
        public void setLastName (String lastName)
        {
            this.lastName = lastName ;
        }
        public void setEmail_address (String email_address)
        {
            this.email_address = email_address ;
        }
        public void setAge (int age)
        {
            this.age = age ;
        }
        public void setStudent_grades (int[] student_grades)
        {
            this.student_grades = student_grades ;
        }

        /*
            SECTION B.2-C REQUIREMENTS: INCLUDE A CONSTRUCTOR USING ALL OF THE INPUT PARAMETERS
        */

    public Student(int student_ID, String firstName, String lastName, String email_address, int age, int[] grades)
    {
        setStudent_ID(student_ID);
        setFirstName(firstName);
        setLastName(lastName);
        setEmail_address(email_address);
        setAge(age);
        setStudent_grades(student_grades);
    }

    /*
        SECTION B.2-D REQUIREMENTS: INCLUDE A PRINT() TO PRINT SPECIFIC STUDENT DATA (E.G., STUDENT ID, FIRST NAME,
        LAST NAME) USING ACCESSORS (I.E. GETTERS)
    */

    public void print()
    {
        System.out.println(getStudent_ID() + "\tFirst Name: " + getFirstName() + "\tLast Name: " + getLastName()
                                          + "\tAge: " + getAge() + "\t\tEmail Address: " + getEmail_address() );

    }

    }
}
