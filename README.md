truct student {
    char first_name[50];
    char last_name[50];
    int roll_number;
    char grade [10];
} s[50];
int main() {
    int x, i;
    printf("Enter the number of students: ");
    scanf("%d", &x);
    printf("\nEnter the students's informations:\n");
    for (i = 0; i < x; i++) {
        s[i].roll_number = i + 1;
        printf("\nInformation for Roll Number:\t%d\n", s[i].roll_number);
//student ke naam 
        printf("Enter the first name: ");
        scanf("%s", s[i].first_name);

        printf("Enter the last name: ");
        scanf("%s", s[i].last_name);

        printf("Enter the Grade: ");
        scanf("%s", s[i].grade);
    }

//student ke roll no 
    printf("\n\nDisplay the student's information:\n");
    for (i = 0; i < x; i++) {
        printf("\nThe Roll Number:\t%d\n", i + 1);

        printf("The First Name: ");
        puts(s[i].first_name);

        printf("The Last Name: ");
        puts(s[i].last_name);

        printf("The Grade: ");
        puts(s[i].grade);
        printf("\n");
    }
    return 0;
}
   
