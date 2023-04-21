
#include <stdio.h>
#include<time.h>

int main()

{
    int d1, m1, y1, d, m, y, a, b, c, e;
    time_t t= time(NULL);
    struct tm date =*localtime(&t);
    printf("Current Date is %d %d %d \n",date.tm_mday,date.tm_mon+1,date.tm_year+1900);
    printf("Enter Your DOB ( dd mm yyyy )  ");
    scanf("%d%d%d", &d1, &m1, &y1);
    
    if (y1 % 4 == 0 && d1<=29 && (y1 % 100 != 0 || y1 % 400 == 0))
    {
        y = date.tm_year+1900 - (y1 + 1);
        m = (12 - m1) + (date.tm_mon+1 - 1);
        d = (29 - d1) + date.tm_mday;
        a = y * 365 + m * 30 + d + (y + 1) / 4;
        b = a / 365;

        if (m1 = date.tm_mon && date.tm_mday >= d1)
        {
            c = (m + 1) % 12;
        }
        else if (m1 = date.tm_mon && date.tm_mday < d1)
        {
            c = m % 12;
        }

        e = d % 29;
        printf("\nYour Age is  %d Years %d Months %d Days", b, c, e);
        goto end;

    }

    if (m1 == 2  && d1 > 28 )
    {
        printf("Input Invalid !");
        goto end;
    }

    else if (d1 <= 31 && m1 <= 12 && date.tm_mday <= 31 && date.tm_mon+1 <= 12)
    {
        y = date.tm_year+1900 - (y1 + 1);
        m = (12 - m1) + (date.tm_mon+1 - 1);

        if (m1 == 1, 3, 5, 7, 8, 10, 12)
        {
            d = (31 - d1) + date.tm_mday;
        }
        else if (m1 == 4, 6, 9, 11)
        {
            d = (30 - d1) + date.tm_mday;
        }
        else
        {
            d = (28 - d1) + date.tm_mday;
        }

        a = y * 365 + m * 30 + d + (y + 1) / 4;
        b = a / 365;

        if (m1 = date.tm_mon && date.tm_mday >= d1)
        {
            c = (m + 1) % 12;
        }
        else if (m1 = date.tm_mon && date.tm_mday < d1)
        {
            c = m % 12;
        }

        if (m1 == 1, 3, 5, 7, 8, 10, 12)
        {
            e = d % 31;
        }
        else if (m1 == 4, 6, 9, 11)
        {
            e = d % 30;
        }
        else
        {
            e = d % 28;
        }

        printf("\nYour Age is  %d Years %d Months %d Days", b, c, e);
    }

    else
    {
        printf("Input Invalid !");
    }

end:

return 0;

}

