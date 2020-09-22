<div align="center">

## Winkey


</div>

### Description

Its an aunthication Program which you can use it to load at the windows startup by using Autoexec.bat file.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Abu\-Mavia](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/abu-mavia.md)
**Level**          |Beginner
**User Rating**    |5.0 (30 globes from 6 users)
**Compatibility**  |C
**Category**       |[Security](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/security__3-14.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/abu-mavia-winkey__3-5150/archive/master.zip)

### API Declarations

graphics.h , conio.h , stdio.h.


### Source Code

```
/* Abu-Mavia Presents.
 Password is : mavia
     winkey.c */
#include<string.h>
#include<stdio.h>
#include<conio.h>
#include<graphics.h>
main()
{
char ah,bh,ch,dh,eh,fh,gh,hh,ih,jh;
int gd=DETECT ,gm,x,y;
int n=1;
str:
initgraph(&gd,&gm,"c:\\tc\\bgi"); // Here is path of your tc dir..
x=getmaxx();
y=getmaxy();
setfillstyle(3, 1);
setcolor(WHITE);
bar(-1,-1,640,480);
rectangle(x/30,y/20,x/1.03,y/1.03);
rectangle(x/30,y/2,x/1.03,y/1.03);
outtextxy(x/1.8+25,y/1.15+5,"Abu-Mavia Presents");
outtextxy(x/1.8+25,y/1.1+5,"E-Mail:mrmasood@hotmil.com");
rectangle(247,175,328,192);
outtextxy(173,180,"Password:");
gotoxy(32,12);
while(!kbhit())
  {
  n++;
  setcolor(n);
  outtextxy(250,179," ? ? ? ?");
  outtextxy(x/2.3+25,y/18+8,"WINKEY");
  delay(100);
  }
ah=getch();
printf("*");
if(ah=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
bh=getch();
printf("*");
if(bh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
ch=getch();
printf("*");
if(ch=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
dh=getch();
printf("*");
if(dh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
eh=getch();
printf("*");
if(eh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
fh=getch();
printf("*");
if(fh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
gh=getch();
printf("*");
if(gh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
hh=getch();
printf("*");
if(hh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
ih=getch();
printf("*");
if(ih=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
jh=getch();
printf("*");
if(jh=='\r')
{
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 { goto yes; } goto wro;
}
if(ah=='m' && bh=='a' && ch=='v' && dh=='i' && eh=='a')
 {
yes:
gotoxy(30,18);
//printf("\a\a");
setcolor(WHITE);
outtextxy(200,300,"Success Full");
sound(2000); delay(200); nosound();
sound(1000); delay(200); nosound();
//printf("Press Any Key");
//getch();
 }
else
   {
   wro:
   sound(2000); delay(300); nosound();
   setcolor(WHITE);
   outtextxy(x/9+10,y/18+8,"Wrong Entry");
   delay(500);
   goto str;
   }
closegraph();
restorecrtmode();
}
```

