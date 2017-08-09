#include <time.h>
#include <stdio.h>

void main()
{
  struct tm* tt;
  time_t t;

  t = time(NULL);

  tt = gmtime(&t);
  printf("time %d %d %d - %d %d %s\n",
    tt->tm_hour, tt->tm_min, tt->tm_sec, tt->tm_isdst, tt->tm_gmtoff, tt->tm_zone);

  tt = localtime(&t);
  printf("time %d %d %d - %d %d %s\n",
    tt->tm_hour, tt->tm_min, tt->tm_sec, tt->tm_isdst, tt->tm_gmtoff/60/60, tt->tm_zone);

}
