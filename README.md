

### Spring Boot Demo 5 Database Example (H2 Database)

**Steps:**
<ol>
<li>To setup IDE for Spring project, follow steps in https://github.com/worldpeacez0991/SpringBoot_demo1</li>

<br/>

<li>Add External Jar to Classpath for H2 driver
<ul>
<li>Via Spring IDE, right click on 'Referenced Libraries' > Bulid Path > Configure Build Path...</li>
<kbd><img src="Pic0A.PNG" width="500" /></kbd><br/><br/>
<li>Via Properties window, select 'classpath' and add external jar 'lib\h2-2.2.220.jar'</li>
<kbd><img src="Pic0B.PNG" width="500" /></kbd><br/>
</ul>
</li>

<br/>

<li>Edit file 'application.properties' 
<br/>(My %USERNAME% is USER1, you may edit this folder path to any folder where you have enough permissions )
<br/>***Note that this folder path will have to match with the steps for 'http://localhost:8080/h2-console' later.
<p>spring.datasource.url=jdbc:h2:file:C:\\Users\\USER1\\H2_DB</p>
</li>

<br/>

<li>Start Spring Boot App
<ul>
<li>Via Spring IDE, open 'DemoApplication.java', press 'Alt+Shift+X, B', to start 'Spring Boot App'</li>
<li>Via browser, type 'http://localhost:8080/h2-console', to test</li>
<kbd><img src="Pic1.PNG" width="500" /></kbd><br/>
<kbd><img src="Pic2.PNG" width="500" /></kbd><br/>

<br/>

<li>When Spring Boot Application starts, SQL Data is loaded with this file 'src\main\resources\data.sql'
<br/>In H2 console, you will see that 'COUNTRIES' is loaded with SQL Data.
</li><br/>
<kbd><img src="Pic3.PNG" width="500" /></kbd><br/>
</ul>
</li>
</ol>

Credits: https://spring.io/team<br/>
Source: https://www.baeldung.com/spring-boot-h2-database<br/>



