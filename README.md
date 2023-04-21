<p align="center">
    <img  src="https://user-images.githubusercontent.com/100967786/232732898-7362dc01-01a3-4088-9432-fadbef53c397.png">
</p>

## Name: Aditya Jadeja

## Student ID: 202001432

## Lab-8 : Unit Testing with JUnit
## Date : 21-04-2023



---
### 1. Create a new Eclipse project, and within the project create a package.

**A java project created with package "lab8_202001432".**

![image](https://user-images.githubusercontent.com/100967786/233599822-8d6f4bd4-529f-4716-b0ea-362a2412200a.png)

### 2. Create a class for a Boa. Here’s the code you can use (you may copy/paste):

![image](https://user-images.githubusercontent.com/100967786/233600602-1b291a3b-6efa-4801-83c6-3e04aca341e5.png)

### 3.Create a JUnit test file for Boa class Mentioned above:

![image](https://user-images.githubusercontent.com/100967786/233601780-1f160357-b65b-4abf-87ee-a1a144381193.png)

### 4. Created Before annotation in test file.

![image](https://user-images.githubusercontent.com/100967786/233603029-9bb57f58-eb04-4aa5-9455-b1ac05e1ad3c.png)


### 5. Implemented test cases for both isHealthy() and Fitsincage() method.
![image](https://user-images.githubusercontent.com/100967786/233604156-85995c24-ad67-4a84-9daf-0baeb314eaf9.png)

**Code for BoaTest**
```
package lab8_202001432;

import static org.junit.jupiter.api.Assertions.*;

import org.junit.Before;
import org.junit.jupiter.api.Test;

class TestBoa {
	
	Boa jen,ken;
	
	@Before
	public void setUp() throws Exception {
	jen = new Boa("Jennifer", 2, "grapes");
	ken = new Boa ("Kenneth", 3, "granola bars");
	}

	@Test
	void testIsHealthy() {
		assertFalse(jen.isHealthy());
		assertTrue(ken.isHealthy());
	}

	@Test
	void testFitsInCage() {
		  //For jen Object
		  assertTrue(jen.fitsInCage(5));  //cage length is greater
		  assertFalse(jen.fitsInCage(2)); // Cage length is same
		  assertFalse(jen.fitsInCage(1));  //cage length is less

		  //For ken Object
		  assertTrue(ken.fitsInCage(5));  //cage length is greater
		  assertFalse(ken.fitsInCage(3)); // Cage length is same
		  assertFalse(ken.fitsInCage(1));  //cage length is less
	}

}

```

### 6. Then,I ran the test-case on Eclipse IDE and get green bar on JUnit Pane.
![image1](https://user-images.githubusercontent.com/100967786/233612018-cf4d4820-a600-4edc-8d36-5575fcd2e7b7.png)

### 7. Create a New method LengthInInches() which will convert length from feet to inches.

![image](https://user-images.githubusercontent.com/100967786/233612981-6adddcb2-3002-42ac-807e-356efafe522b.png)

### 8. Wrote the new test-case for new LengthInInches() method and tested it.
![image](https://user-images.githubusercontent.com/100967786/233613131-c77ec9a8-b4ad-4ad0-8710-04c3b1893655.png)



