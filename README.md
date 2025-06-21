<?php
$host = "localhost";
$user = "root";
$pass = "";
try{
	$conn = new PDO("mysql:host=$host",$user, $pass,);
	$sql = "Create database test12";
	$conn->exec($sql);
	echo" Database is created";
}catch(Exception $e){
	echo "Databse not created , something went wrong!";
}

?>



mmmm

<?php
    
    $host = "localhost";
    $db = "test12";
    $user = "root";
    $pass = " ";

    try { 
        $pdo = new PDO("mysql:host=$host;dbname=$db", $user, $pass);
        $sql = "CREATE TABLE users (id INT(6) NOT NULL AUTO_INCREMENT PRIMARY KEY 
        	username VARCHAR(30) NOT NULL ,
        	password VARCHAR(50) NOT NULL )";

        $pdo->exec($sql);

    echo "Table created succesfully ";

    } catch(Exceptio $e){
    	echo "Error creating table: " . $e->getMessage();

    }

?>

mmm

<?php
try {

	$pdo = new PDO("mysql:host=localhost;dbname=test12", "root", " ");

	$username ="Jack";
	$password = password_hash("mypassword", PASSWORD_DEFAULT;

    $sql = "INSERT INTO users (username, password) VALUES ('$username', '$password')";
    $pdo->exec($sql);


    echo "New record created succesfully.";


} catch()
    

mm
<?php

try {
	//connect to the database
	$pdo = new PDO("mysql:host=localhost;dbname=test12", "root", " ");

	//Table alteration SQL 
	$sql = "ALTER TABLE users ADD emain VARCHAR (255)";

	//Excecute the statement using the esec() method of PDO object 
    $pdo->exec($sql);

    echo "Column created succesfully!";
} catch (PDOException $e) {
	echo "Error creating column: " .. $e->getMessage();
}

?>


















