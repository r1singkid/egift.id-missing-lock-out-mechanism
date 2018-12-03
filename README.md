# giftn.id-missing lock out mechanism - AFTER FIXED BYPASS [PART 2]


http://www.giftn.id is one of the more popular egift webshops in Indonesia, even big companies like Tokopedi*, Mandir*, BC*, Gra*, and OV* use this site as their e-gift provider. 
I was looking around on their website and comparing prices when I found out that there is a Lock-out Mechanism but its very weak and can be bypassed just by using simple random User Agent and Proxy while using the cURL function.
Its actually only 31 lines of code in the core process, but ofcourse I need to declare cURL function at first.

![alt text](https://github.com/r1singkid/egift.id-missing-lock-out-mechanism/blob/master/core%20code.png)

This is the second bypass I made for http://www.giftn.id. Basically the curl function above is for crawling giftn.id voucher provider(egif.id) , I found out that there is pattern in the gift voucher url.

![alt text](https://github.com/r1singkid/egift.id-missing-lock-out-mechanism/blob/master/proccess.png)

Because I used while(true) function, this php script have to be run in php folder in xampp

Here is my finding

![alt text](https://github.com/r1singkid/egift.id-missing-lock-out-mechanism/blob/master/running%20and%20found.png)


In this case, after doing random curl, I realized that the pattern is
DU8E16X0000000
for a voucher worth 100k (Given for Mandir* Fiesta Point). So i just random in that range and found really much voucher.

http://egift.id/DU8E16P1350001 

http://egift.id/DU8E16P2650001

http://egift.id/DU8E16P2800001 

http://egift.id/DU8E16P3200001 

http://egift.id/DU8E16P3500001 

http://egift.id/DU8E16P3610001 

http://egift.id/DU8E16P3750001 

http://egift.id/DU8E16P3920001 

here is the example for trying accessing the found url.
![alt text](https://github.com/r1singkid/egift.id-missing-lock-out-mechanism/blob/master/boom.png)



