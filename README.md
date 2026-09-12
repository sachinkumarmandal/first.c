#include <stdio.h>

void displayHeader() {
    printf("\n");
    printf("============================================================\n");
    printf("                 SACHIN KUMAR\n");
    printf("              SOFTWARE DEVELOPER\n");
    printf("============================================================\n");
}

void displayProfile() {
    printf("\n-------------------- PROFESSIONAL PROFILE ------------------\n");
    printf("Name        : Sachin Kumar\n");
    printf("Role        : Aspiring Software Developer\n");
    printf("Languages   : C | C++ | Python\n");
    printf("Focus       : DSA | Problem Solving | Software Development\n");
    printf("Mindset     : Continuous Learning & Improvement\n");
    printf("Principles  : Discipline | Consistency | Punctuality\n");
}

void displaySkills() {
    printf("\n------------------------- SKILLS -----------------------------\n");
    printf("[+] C Programming\n");
    printf("[+] C++ Programming\n");
    printf("[+] Python Programming\n");
    printf("[+] Data Structures & Algorithms\n");
    printf("[+] Logical & Analytical Problem Solving\n");
    printf("[+] Programming Fundamentals\n");
}

void displayCareer() {
    printf("\n-------------------- CAREER OBJECTIVE -----------------------\n");
    printf("I am focused on developing strong programming and\n");
    printf("problem-solving skills while building practical projects.\n");
    printf("My goal is to grow into a professional software developer\n");
    printf("through continuous learning, discipline, and consistency.\n");
}

void displayContact() {
    printf("\n------------------- CONTACT INFORMATION ---------------------\n");
    printf("LinkedIn : www.linkedin.com/in/sachin-kumar-3a1a85432\n");
    printf("Email    : sachinmandle591@gmail.com\n");
    printf("GitHub   : github.com/sachinkumarmandal\n");
}

int main() {
    int choice;

    displayHeader();

    while (1) {
        printf("\n======================= MAIN MENU ============================\n");
        printf("1. View Professional Profile\n");
        printf("2. View Skills\n");
        printf("3. View Career Objective\n");
        printf("4. View Contact Information\n");
        printf("5. View Complete Profile\n");
        printf("0. Exit\n");
        printf("============================================================\n");

        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice) {

            case 1:
                displayProfile();
                break;

            case 2:
                displaySkills();
                break;

            case 3:
                displayCareer();
                break;

            case 4:
                displayContact();
                break;

            case 5:
                displayProfile();
                displaySkills();
                displayCareer();
                displayContact();
                break;

            case 0:
                printf("\nThank you for visiting my profile.\n");
                printf("Keep Learning. Keep Building. Keep Growing.\n\n");
                return 0;

            default:
                printf("\nInvalid choice! Please select a valid option.\n");
        }
    }

    return 0;
}
