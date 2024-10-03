# Program1a
#include<stdio.h>

int main() {
    int bookID, dueDate, returnDate, daysOverdue, fine;
    
    printf("Enter book ID: ");
    scanf("%d", &bookID);
    
    printf("Enter Due Date: ");
    scanf("%d", &dueDate);
    
    printf("Enter Return Date: ");
    scanf("%d", &returnDate);
    
    daysOverdue = returnDate - dueDate;
    
    if (daysOverdue <=7) {
      fine = daysOverdue * 20;
    } else if (daysOverdue <=14) {
      fine = (daysOverdue - 7) * 50 + 140;
    } else {
      fine = (daysOverdue - 14) * 100 + 700;
    }
        
    printf("Total fine: Ksh. %d\n", fine);
    
    return 0;
}
