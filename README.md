Student Grade Calculator (C Project)

- Description

The Student Grade Calculator is a simple C program that automatically calculates the total marks, average, and grade of a student.
It demonstrates the use of arrays, loops, and conditional statements in computing.

-Objectives

Automate student grade calculation

Minimize human error

Strengthen understanding of core programming logic

Demonstrate real-world application of computing aptitude


- Tools Used

Language: C

Compiler: GCC / Turbo C / Code::Blocks

Operating System: Windows / Linux


- Working / Algorithm

1. Input marks for 5 subjects.


2. Calculate total and average.


3. Determine grade using if-else logic:

90–100 → Grade A

80–89 → Grade B

70–79 → Grade C

60–69 → Grade D

Below 60 → Grade F



4. Display total, average, and grade neatly.



- Source Code (C)

#include <stdio.h>

int main() {
    float marks[5], total = 0, average;
    int i;

    printf("Enter marks of 5 subjects:\n");
    for(i = 0; i < 5; i++) {
        printf("Subject %d: ", i + 1);
        scanf("%f", &marks[i]);
        total += marks[i];
    }

    average = total / 5;

    printf("\n===== Student Grade Report =====\n");
    printf("Total Marks: %.2f\n", total);
    printf("Average Marks: %.2f\n", average);

    if(average >= 90)
        printf("Grade: A\n");
    else if(average >= 80)
        printf("Grade: B\n");
    else if(average >= 70)
        printf("Grade: C\n");
    else if(average >= 60)
        printf("Grade: D\n");
    else
        printf("Grade: F\n");

    printf("================================\n");
    return 0;
}

📄 Sample Output

Enter marks of 5 subjects:
85 90 78 88 92

===== Student Grade Report =====
Total Marks: 433.00
Average Marks: 86.60
Grade: B
================================

🚀 Future Enhancements

Add student name and roll number

Support variable subject counts

Save results in a file or database

Create GUI version


👨‍💻 Developed by

Kartik Choudhary (UID: 23BCA10198)
Sahil Arora (UID: 23BCA10193)
Section: 23BCA-7B
Subject Code: 23CAP-308
