Dependencies
	
	<dependencies>
		<!-- Spring Dependency -->
		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-context</artifactId>
			<version>5.2.7.RELEASE</version>
		</dependency>

	</dependencies>
	<properties>
		<maven.compiler.target>11</maven.compiler.target>
		<maven.compiler.source>11</maven.compiler.source>
	</properties>
------------------------------------------------------------------------------------------
com.infy.demo
->class Customer
-->geters, setters , functions

->class UserInterface
-->import org.springframework.context.ApplicationContext;
-->import org.springframework.context.annotation.AnnotationConfigApplicationContext;
-->import com.infy.config.SpringConfig;
--->ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
--->Customer customer = applicationContext.getBean(Customer.class);

------------------------------------------------------------------------------------------
com.infy.config
->import org.springframework.context.annotation.Bean;
->import org.springframework.context.annotation.Configuration;
->import com.infy.demo.Customer;
-->@Configuration
->class SpringConfig
-->@Bean

-------------------------------------------------------------------------------------------