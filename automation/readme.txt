// depending on the IDE/environment you use, your project files can reside here.

//Programme 1 - Verify Creation of To Do List //

package Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
public class verifycreationoftodolist 
{
public static void main(String[] args) 
   {
	//Launching of the application in chrome browser//
	System.setProperty("webdriver.chrome.driver", "/Downloads/chromedriver");
	WebDriver driver = new ChromeDriver();
	driver.get("http://amadeus.maclab.org/_demo/nss-todo-1.1/index.php");
	
	//Enter ToDoListName
	driver.findElement(By.name("Add")).sendkeys("Assessment1");
	
	//Click on add button
	driver.findElement(By.name("Add")).click();
	
	//Verification of to List created//
	boolean ToDoListCreationStatus = driver.findElement(By.name("Assessment1")).isDisplayed();
	if (ToDoListCreationStatus == true)
	{
		System.out.println("ToDoList Created Successfully, Test Passed");
	}
	else
	{
		System.out.println("Test Failed");	
	}
	//Close browser
	driver.close();
	}

}

//Verify Creation of Category //
package Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class verifycreationofcategory {

	public static void main(String[] args) 
	
	{
		//Launching of the application in chrome browser//
		System.setProperty("webdriver.chrome.driver", "/Downloads/chromedriver");
		WebDriver driver = new ChromeDriver();
		driver.get("http://amadeus.maclab.org/_demo/nss-todo-1.1/index.php");
		
		//Enter CategoryName
		driver.findElement(By.name("Add Category")).sendkeys("TestCategory1");
		
		//Click on add category button
		driver.findElement(By.name("Add category")).click();
		
		//Verification of Category created//
		boolean CategoryCreationStatus = driver.findElement(By.name("TestCategory1")).isDisplayed();
		if (ToDoListCreationStatus == true)
		{
			System.out.println("Category Created Successfully, Test Passed");
		}
		else
		{
			System.out.println("Test Failed");	
		}
		//Close browser
		driver.close();
		}


	}

}

//Verify Remove/Complete function

package Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class verifycreationofcategory {

	public static void main(String[] args) 
	
	{
		//Launching of the application in chrome browser//
		System.setProperty("webdriver.chrome.driver", "/Downloads/chromedriver");
		WebDriver driver = new ChromeDriver();
		driver.get("http://amadeus.maclab.org/_demo/nss-todo-1.1/index.php");
		
		//Enter CategoryName
		driver.findElement(By.name("Add Category")).sendkeys("TestCategory1");
		
		//Click on add category button
		driver.findElement(By.name("Add category")).click();
		
		//Verification of Category created//
		boolean CategoryCreationStatus = driver.findElement(By.name("TestCategory1")).isDisplayed();
		if (ToDoListCreationStatus == true)
		{
			System.out.println("Category Created Successfully, Test Passed");
		}
		else
		{
			System.out.println("Test Failed");	
		}
		//Close browser
		driver.close();
		}


	}

}

