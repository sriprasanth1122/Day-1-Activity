# Day-1-Activity
Blog on Difference between HTTP1.1 vs HTTP2 and Blog about objects and its internal representation in Javascript.


# DAY_01-Task

DAY_01

1]. Difference between HTTP1.1 and HTTP2

HTTP 1.1 
	keeps all requests and responses in plain text formet
	It loads a single request for every TCP connection
	Loading speed is slow when compared with HTTP2
	The protocol serving for over 15 years 

HTTP 2

	It uses the binary framing layer to ENCAPSULATE all the messages in binary formet
	It avoids network delay by using Multiplexing.
	It loads faster than HTTP1.1
	grealy increasing in the flexibility of data tranfer
	
2]. Object and its internal representation in Javascript
	
	Javascript Object is a collection of Key-Value pairs,example
	
	objects contains many values, and separated by coma(,)
	
	Syntax: object = { key1:value1, key2:value2 };

	A Person has many propeties like name, age, education, job...
	A car has properties like  color, model, weight 
	
	const car = {type:"Aspire", model:"500", color:"white"};
	const person = {firstName:"John", lastName:"Doe", age:20 };
 	
 	Accessing Object Properties using camal notation that is objectName second in capital letter
 	
 	object properties can be accessed in 2 ways: 
 	
 			using ( . ) objectName.propertyName
 			 Example :  person.firstName;
 									(or)
 			using[" "] objectName["propertyName"]
 			Example :  person["firstName"];
 	
	Internal representation which is nesting objects inside the object.
	nested objects that have other objects inside them as their property.
	Nesting is widely used in programming as it provides the code with more enhanced details.
	
		const layer0 = {
				Item1: "Layer 1 Item 1 Text",
 				Item2: {
    			Item1: "Layer 2 Item 2 Text",
    			Item2: false,    
   				Item3: {
      			Item1: "Layer 3 Item 2 Text"
   									 }
 								 }
							};
					
		to access the properties of objects using ( . ) 					
				layer0.layer1Item2.layer2Item1.layer3Item1
	    to add property we will simply attach the object name with the object property with a dot and assign it a value.
		
