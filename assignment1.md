 **Student name**: Mohammed Abdul kareem 
 
 **Student id**: MOH22609097
 
 **lab**:Security testing 
 
 **Date**:21-02-2024

**  1. Setup security testing environment **

   1. Use case : OWASP juice shop server
   2. Operating system :Ubuntu 22.04
   3. Network adaptor :192.168.123.111/24
   4. User: student
   5. Password :Student1
      
      ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/40d900b7-fc2c-40d4-9405-bea46bf982a0)

   6. Use case : security testing workstation
   7. Operating system :kali Linux
   8. Network adaptor :192.168.123.112/24
   9. User:kali
   10. Password :kali

      ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/2dfb5937-e0c8-4527-9e7a-51beb17389f0)

 **Requirement 3: Exploit a cross-site scripting vulnerability**

   **Reflected XSS:**

 1. The reflected XSS attack is done by entering the payload into the URL.
 2. Firstly i have purchased some product and then in the track order page i got the tracking id.
 3. In the tracking id url just remove the order id and enter the payload <iframe src="javascript:alert(`xss`)">
 4. After reloading the attack successfully runs.

![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/56c377ea-b192-46cf-a204-a3788a54c323)


 **Requirement 4: Exploit a SQL injection vulnerability**
**Login Bender:**:
1. In the reviews i got the bender account username
2. bender@juice-sh.op
3. I want to log in with bender account so just after the mail id enter '-- which means ' close bracket in SQL and -- comment out
4. username: bender@juice-sh.op'--
5. password: something


 ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/5834251e-d772-4b29-a4cd-2a0000c67fa8)


 **Requirement 5. Exploit a Broken Access Control vulnerability.**
 **Easter Egg:**
 1. Firstly log in to the ftp page as 192.168.123.111:3000/ftp
 2. It comes a page with the hidden files
 3. There is a file named eastere.gg
 4. When i open the file it is giving me error as only .pdf and .md files allowed
    
    ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/c9ba6e09-efee-4bbd-a201-5cda555bb47f)

 5. So to solve this error use %2500.md as http://192.168.123.111:3000/ftp/eastere.gg%2500.md
    
   ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/bd97b9f0-2e9e-4157-8c9a-86454bff8ad3)

 6. then file is downloaded on the browser.

 ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/36aa3d73-2657-4f16-aa38-9dad728657e0)


**Requirement 6. Exploit an Authentication Bypass vulnerability:**

**Reset Bjoern's password via Forget password:**

1. Firstly check the email from reviews of Bjoern as Bjoern@juice-sh.op
2. now when i click on forgot password it asks me the security question as hometown postal code
3. i googled it and got to know the postalcode of this hometown Uteresen,Germany as West-2082
4. after entering it i successfully changed the password of Bjoern..

   ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/57be0eec-c6f1-4c0b-a880-e6ca1df47e46)



**Requirement 7. Expliot an Improper Input validation vulnerability.**

**Poison Null Byte:**

1.Firstly log in to the ftp page as 192.168.111:3000/ftp
2.It comes a page with hidden files
3.There is a file named package.json.bak
4.when i open the fike it is giving me error only .pdf and .md files allowed
5. so to solve this error use %2500.md
6.Then file is downloaded on the browser
  
  ![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/60eddb0f-449e-4e55-8575-e852e01fc883)


**Requirement 8. Expliot a Sensitive data Exposure vulnerability.**

**Forgotten Developer Backup:**

1.Firstly log in to ftp page as 192.168.123.111:3000/ftp
2.It comes a page with hidden files
3.There is a file named package.json.bak

![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/32545e86-8415-4ba4-8cde-cfd41892e72a)

4.When open the file it is giving me error only .md and .pdf files allowed
5.So to solve this error use %2500.mdas http://192.168.123.111:3000/ftp/package.json.bak%2500.md
6.Then file is downloaded on the browser
 
![image](https://github.com/mak7075/PORTFOLIO-1/assets/153539105/4595509a-670d-4921-97a7-993924af7672)

 
   
 
