// LOAD AND ESTABLISH THE CONNECTION 
		Class.forName("com.mysql.cj.jdbc.Driver");

		// ESTABLISH THE CONNECTION WITH WITH DATA BASE
		Connection connection=DriverManager.getConnection("jdbc:mysql://localhost:3306/persondb", "root", "root");
		
		// CREATE THE STATEMENT
		Statement statement=connection.createStatement();
		
		// EXECUTE STATEMENT
		statement.execute(" insert into person values(2,'vardhan','pithapuram',21,9390246996)  ");
		
		// CLOSE THE CONNECTION
		connection.close();
