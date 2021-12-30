# Browser-Automation
Sample Code

public static void main(String[] args) {
		
		
		//WebDriverManager.chromedriver().setup(); // setting up chrome driver manager
		WebDriverManager.edgedriver().setup(); //
		
		//WebDriver driver = new ChromeDriver();
		WebDriver driver = new EdgeDriver();
		driver.get("https://google.com"); // Get means fetching the browser 
		//driver.manage().window().maximize();
		//driver.close();// Close the entire browser
		//String title = driver.getTitle(); 
		System.out.println(driver.getTitle()); 
		driver.navigate().to("https://facebook.com");
		System.out.println(driver.getTitle());
		driver.navigate().forward();
		driver.navigate().to("https://amazon.com");
		driver.navigate().back();
		driver.navigate().refresh();
		driver.quit();
		
		
	}
