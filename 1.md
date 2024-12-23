#include <stdio.h>
#include <stdlib.h>
#include <string.h>
struct day
{
    char *name;   
    int date;
    char *activity;
};struct day week[7];
void create()
{
for(int i=0;i<7;i++)
{
week[i].name= (char*)malloc(20*sizeof(char));
week[i]. activity= (char*)malloc(20*sizeof(char));
}
}
void read()
{
for(int i=0;i<7;i++)
{
printf("enter the name of day %d",i+1);
scanf("%s",week[i].name);
printf("enter the date of day%d",i+1);
scanf("%d",&week[i].date);
printf("enter the activity day%d",i+1);
getchar();
fgets(week[i].activity,100,stdin);
}
}

void display(){
printf("\n day\t date\t activity\n");
for(int i=0;i<7;i++)
{
printf("%s\t%d\t%s",week[i].name,week[i].date,week[i].activity);
}
}
int main()
{
printf("creating calender\n");
create();
read();	
printf("displaying the calender\n");
display();
return 0;
}

creating calender
enter the name of day1 Sunday
enter the date of day1 1
enter the activity day1 sleeping
enter the name of day 2 Monday
enter the date of day2 2
enter the activity day2 reading
enter the name of day 3tuesday
enter the date of day3 3
enter the activity day3writing article
enter the name of day 4wednesday
enter the date of day4 4
enter the activity day4 meeting friends
enter the name of day 5  thursday
enter the date of day5  5
enter the activity day5  conference call
enter the name of day 6   friday
enter the date of day6  6
enter the activity day6outing with friends
enter the name of day 7saturday
enter the date of day7 7
enter the activity day 7movie

displaying the calender
 day     date    activity
sunday  1      sleeping
monday  2     reading
tuesday 3      writing article
wednesday       4   meeting friends
thursday        5     conference call
friday  6      outing with friends
saturday        7     movie
