# PersianCalendar
Persian (Jalali) Calendar in Java

## Sample Usage
Here is an example of how you would use PersianCalendar:
```java
PersianCalendar.DateStruct persianDate = PersianCalendar.gregorianToPersian(2016, 11, 6);   // 1395/8/16
PersianCalendar.DateStruct gregorianDate = PersianCalendar.persianToGregorian(1395, 8, 16); // 2016/11/6

PersianCalendar pCalendar = new PersianCalendar(Calendar.getInstance()); // Gets a calendar using the default time zone and locale. 
                                                                         // The Calendar returned is based on the current time in 
                                                                         // the default time zone with the default locale.
pCalendar.getDate();      // 1395/8/16
pCalendar.addDay(5);      // 1395/8/21
pCalendar.addMonth(4);    // 1395/0/21 --> 0 = Farvardin
pCalendar.getDayOfWeek(); // 2         --> 2 = Monday
```

## Note
- **FirstDayOfWeek** in PersianCalendar is **Saturday**
- **DayOfWeek** and **Month** is zero based. 
   - **Month** : 0: Farvardin, 1: Ordibehesht and ...
   - **DayOfWeek** 0: Saturday, 1: Sunday and ...
