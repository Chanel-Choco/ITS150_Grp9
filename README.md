# Get a Copy of This Project

Open your terminal or command prompt and type:
- git clone https://github.com/Chanel-Choco/ITS150_Grp9.git

# Update or Edit and Sync to GitHub

Open Command Prompt and go to your project folder:
- C:\Users\Julianna Boado\Documents\NetBeansProjects\SecuritySystem>

Type the following commands:
- git add .
- git commit -m "Updated feature or fixed something"   # Replace this message
- git push


# To add sql

Watch this vid: https://www.youtube.com/watch?v=d-VMTilnLJs

Please create a database in your sql workbench 



CREATE DATABASE securitySystem;


USE securitySystem;


CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  
  username VARCHAR(50) NOT NULL UNIQUE,
  
  password VARCHAR(255) NOT NULL,
  
  createdAt TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  
  lastLogin TIMESTAMP NULL
);


INSERT INTO users (username, password)

VALUES 

('admin', SHA2('1234', 256)),

VALUES ('grp9', SHA2('group9', 256)),

('its150', SHA2('lecture', 256)),

('testUser', SHA2('user123', 256)), 

('testuser2', SHA2('user123', 256));


