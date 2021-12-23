# Facebook
package testClass_Fb;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;


import pomp_fb.SignUp_fb;


public class TC01 {
public static void main(String[] args) throws InterruptedException {
	System.setProperty("webdriver.chrome.driver", "C:\\Users\\Shubham\\Downloads\\chromedriver.exe");
	WebDriver driver = new ChromeDriver();
	driver.get("https://www.facebook.com/signup");
	driver.manage().window().maximize();

	SignUp_fb sign = new SignUp_fb(driver);
	sign.enterFirstname();
	Thread.sleep(2000);
	sign.enterLastname();
	Thread.sleep(2000);
	sign.enterEmailId();
	
	
}
}
