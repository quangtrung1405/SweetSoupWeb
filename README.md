Member: Nguyen Quang Trung – 1801040230
	    Nguyen Van Son – 1801040182
               Do Viet Anh - 1801040004


I.	Install tools
-	Vs code:  https://code.visualstudio.com/download
-	Nodejs: https://nodejs.org/en/download/
-	Mongodb Community server: https://www.mongodb.com/try/download/community
-	Navigate to the C Drive on your computer using Explorer and create a new folder called data here.	
-	 ![image](https://user-images.githubusercontent.com/40718164/141686945-5b503d6c-0467-49d5-a58a-bd5423a549a5.png)
-	B. Inside the data folder you just created, create another folder called db.
-	![image](https://user-images.githubusercontent.com/40718164/141686952-32744771-592c-48ad-b747-04fc1e825452.png)

Configure the VM and MongoDB
1.	Right-click the Start menu, and select System.
2.	Click Advanced system settings, and then click Environment Variables.
3.	Under System variables, select Path, and then click Edit. Click new and add the path C:\Program Files\MongoDB\Server\4.2\bin

Reboot computer to make sure everything work fine

II.	Configuration project
1.	Download the IWS_Final zip file at https://drive.google.com/file/d/160POh7pSC8UDRcRObymkDrN6KXagNr5p/view?usp=sharing and extract it to your computer
2.	Open visual studio code and choose open folder, then Select the folder you just extracted.
 
![image](https://user-images.githubusercontent.com/40718164/141686978-05aab895-5b8a-4c51-9bcd-a2688d456cd5.png)

3.	Enter cd backend in Terminal window to direct to backend folder
 
![image](https://user-images.githubusercontent.com/40718164/141686977-784628db-c201-4f2d-909c-cd4225678513.png)

4.	Enter npm install npm-install-all -g to install all the dependences of the backend
 ![image](https://user-images.githubusercontent.com/40718164/141686985-8db9f340-2fae-4314-9560-a6b3f080727d.png)

5.	Before run the backend services, download the dbs zip file at https://drive.google.com/file/d/160POh7pSC8UDRcRObymkDrN6KXagNr5p/view?usp=sharing
and extract it to your C drive
6.	Open cmd by press start key and type cmd
7.	Enter the command cd C:\Program Files\MongoDB\Server\4.2\bin
8.	Enter the following 3 lines of code to import database to mongodb local collection:
mongoimport -d test -c soups C:\dbs\soups.json
mongoimport -d test -c comments C:\dbs\comments.json
mongoimport -d test -c orders C:\dbs\orders.json
 ![image](https://user-images.githubusercontent.com/40718164/141686991-cf7077bc-d99d-47cb-8732-a7f2c4b12b0a.png)

9.	Back to Visual Studio Code, in terminal, type npm run serve to run backend service
10.	Press crtl+shift+` or click Terminal -> New Terminal to get a new terminal window
11.	Enter cd sweetsoup-website to direct to frontend folder
12.	Enter npm install npm-install-all -g to install all the dependences
13.	After Instaling finish, type npm start to run the frontend
