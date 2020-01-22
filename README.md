# spring-openapi-3-spec-gen

# For Generating OpenAPi Spec 3.* for Spring Controllers
 - At Runtime 
  ```
  <dependency>
			<groupId>org.springdoc</groupId>
			<artifactId>springdoc-openapi-core</artifactId>
			<version>1.1.44</version>
	</dependency>
  
  ```
  > visit -  [/v3/api-docs](http:localhost:8080/v3/api-docs) { to customize springdoc.api-docs.path=/api-docs}
  - At Build Time
  ```
  ```
# For Generating OpenAPi Spec 3.* for JAX-RS

```
<plugin>
				<groupId>io.openapitools.swagger</groupId>
				<artifactId>swagger-maven-plugin</artifactId>
				<version>2.1.1</version>
				<configuration>
					<resourcePackages>
						<resourcePackage>uk.co.rbs.mortgage.customer</resourcePackage>
						<resourcePackage>uk.co.rbs.mortgage.customer.request.api</resourcePackage>
					</resourcePackages>
					<outputDirectory>${basedir}/target/</outputDirectory>
					<outputFilename>swagger</outputFilename>
					<outputFormats>JSON,YAML</outputFormats>
					<prettyPrint>true</prettyPrint>
				</configuration>
				<executions>
					<execution>
						<goals>
							<goal>generate</goal>
						</goals>
					</execution>
				</executions>
	</plugin>
  ```
