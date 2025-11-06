# Coffee Cart Automation Testing Project

## Framework Used
- **Language:** Java
- **Testing Framework:** JUnit 5
- **Automation Tool:** Selenium WebDriver
- **IDE:** Eclipse IDE
- **Browser Tested:** Google Chrome

---

## Setup Instructions

#### Prerequisites
**Ensure I have:**
- Java JDK 17 
- Eclipse IDE
- Google Chrome (142.0.7444.60)(Stable) 
- ChromeDriver (142.0.7444.59) (Stable)
- Selenium Java Client
- Selenium Server
- JUnit JAR files


#### Add Dependencies
1. Download Selenium Java Client and Selenium Server
2. Extract the zip file and include:
- selenium-java-4.9.0.jar
- selenium-server-4.38.0.jar
- All JARs inside the /libs folder
3. Download JUnit 5 (junit-5.9.2.jar)
4. Download JDK 17.0.7
5. **Add JRE**
- Right-click CoffeeCart_Project → Properties
- Go to Java Build Path → Libraries tab
- Click Add Library → JRE System Library → Next
- Select Execution Environment: JavaSE-17
- Click Finish → Apply and Close
6. **Add Selenium Libraries**
- Right-click CoffeeCart_Project → Build Path → Configure Build Path
- Click Libraries → Add External JARs...
- Select all .jar files
- Apply and Close
7. **Add JUnit Library**
- Right-click CoffeeCart_Project → Build Path → Add Libraries...
- Choose JUnit → Click Next
- Select JUnit 5 → Finish
- Click Apply and Close


### Configure ChromeDriver Path
In each test file, I set driver path correctly:
- System.setProperty("webdriver.chrome.driver", "C:\\Users\\USER\\Downloads\\chromedriver-win64\\chromedriver.exe");
  

### Execution Test
- Right-click src folder in CoffeeCart_Project → New → Package → name it TS01
- Right-click TS01 → New → Class : name.java
- Write the test script
- Right-click inside the code → Run As → JUnit Test

---

## Notes and Limitations

### Notes
- The tests are written for [https://coffee-cart.app](https://coffee-cart.app) using Selenium WebDriver and JUnit 5.
- Each test case represents a separate scenario
- The project was developed using Eclipse IDE on Windows 10.
- WebDriverManager is used to handle ChromeDriver setup automatically.

### Limitations
- Tests depend on the Coffee Cart website being online and unchanged.
- Use explicit waits for dynamic elements instead of fixed Thread.sleep()
- Currently, no advanced test reports or screenshots are generated.
- Only tested on Google Chrome (latest version).
- Uses static data 
- May require manual updates if website structure changes.
