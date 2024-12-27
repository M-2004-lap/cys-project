# cys-project
final-cys-project(haking owasp juice shop)
1-Enumeration attack 
by using ffuf to get all possible username to the admin user
code(ffuf -u http://localhost:3000/Fuzz -w common.txt)
![صورة واتساب بتاريخ 2024-12-27 في 09 17 42_b3c80f73](https://github.com/user-attachments/assets/769cfad7-0597-4fe5-a5b7-56afed5a6107)
![صورة واتساب بتاريخ 2024-12-27 في 09 19 35_85cf8d0b](https://github.com/user-attachments/assets/73bf941f-3e82-45b2-95c1-241c6d2e0b62)
after this try all possible outcomes until get(username=administration)
![صورة واتساب بتاريخ 2024-12-27 في 09 19 27_db515a7e](https://github.com/user-attachments/assets/8024f37b-91af-4aa6-9ef1-705d0e12d5e3)
that mean that you are not ahve the access to this page (403 == forbidden)
and make an sql injection to get into the admin account 

2-Now we get the username of admin user 
to get the password to the admin user by brup suite  
![image](https://github.com/user-attachments/assets/bca858b3-fabc-4784-8810-21a24ac21c78)
![صورة واتساب بتاريخ 2024-12-27 في 09 49 50_f518a26d](https://github.com/user-attachments/assets/eecec138-a7e1-4bda-b898-044c97863633)




3-xss
![صورة واتساب بتاريخ 2024-12-25 في 00 07 32_b4534ea1](https://github.com/user-attachments/assets/ff430cb2-8e5d-4d01-ac4d-3e22f8b82b57)
to get the alert that apper to the user code(<iframe src="javascript:alert('xss')">)

![صورة واتساب بتاريخ 2024-12-26 في 13 31 59_13e05476](https://github.com/user-attachments/assets/18cc37a4-40e3-4401-b524-7027f6db3935)
to apper our website in the web that get the user to our website
code(<iframe src="https://alexu.mans.edu.eg/static/index.html"></iframe>)

![صورة واتساب بتاريخ 2024-12-26 في 13 35 02_a885e198](https://github.com/user-attachments/assets/821520a4-5831-401b-a4e5-5312838f6202)
that make the user inpute thir data by alert to the user as offer page in the main website
code(<form method="GET">Username: <input type="text" name="username" value="" /> <br 
/>Password: <input type="password" name="passwd" value="" /> <br /><input 
type="submit" name="submit" value="login" /></form>)

![صورة واتساب بتاريخ 2024-12-26 في 13 34 10_2eb708ca](https://github.com/user-attachments/assets/b6b3a720-b4ba-4507-9baa-35cc3259485c)
code(<button type="button">Click Me!</button>) to click by the user to get into our website

4-sql injection 
![صورة واتساب بتاريخ 2024-12-26 في 11 48 43_5e3ec530](https://github.com/user-attachments/assets/d172beed-6407-4144-b688-7d8d324199b4)
![صورة واتساب بتاريخ 2024-12-26 في 11 50 00_b4d68b3a](https://github.com/user-attachments/assets/6e781a8e-213a-4967-8238-26b995eafe04)
to enter to the website with out kouwn the username or password

![صورة واتساب بتاريخ 2024-12-26 في 11 52 06_c843a937](https://github.com/user-attachments/assets/ca0c415f-60b0-48d9-8ce0-29ab1da213a1)
to enter the website with kouwn only the user name without kouwn the apssword










