# area-of-shapes
#include<stdio.h>
int main(void)
{ 
    char shape;
    float len,bre,base,height,rad,area;
    printf("Enter the shape of the figure (c=circle,t = triangle,r = rectangle): ");
    scanf("%c",&shape);

switch(shape){
   case 'c':
   case 'C':
       printf("Enter the radius: ");
       scanf("%f",&rad);
       area = ((3.14f)*rad*rad);
       printf("the area of cicle is:%.2f\n",area);
       break;
    case 't':
    case 'T':
        printf("enter the base of the triangle: ");
        scanf("%f",&base);

       printf("Enter the height of the triangle:");
       scanf("%f",&height);

      area = (0.5*base*height);
      printf("the area of triangle is: %.2f\n",area);
      break;

    case  'r':
    case 'R':
       printf("Enter the lenght of the rectangle: ");
       scanf("%f",&len);

       printf("enter the breadth of the rectangle: ");
       scanf("%f",&bre);

       area = (len*bre);
       printf("The area of rectangle is:%.2f\n",area);
       break;

    default:
        printf("invalid input choose correct shape");   
}
return 0;
}
