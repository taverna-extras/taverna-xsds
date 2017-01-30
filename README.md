# Taverna XSDs
Contains XML `.xsd` files with non Apache like licences required by other repos with licence restrictions.  
Uses [Maven Remote Resources plugin](http://maven.apache.org/components/plugins/maven-remote-resources-plugin/index.html "Maven Remote Resources plugin").

To build use `maven install`. To include in your project add the following to the plugin section of your pom file.
```xml
			      <plugin>
					<groupId>org.apache.maven.plugins</groupId>
					<artifactId>maven-remote-resources-plugin</artifactId>
					<version>1.5</version>
					<configuration>
						<resourceBundles>
							<resourceBundle>uk.org.taverna:shared-resources:1</resourceBundle>
						</resourceBundles>
					</configuration>
					<executions>
						<execution>
							<goals>
								<goal>process</goal>
							</goals>
						</execution>
					</executions>
				</plugin>
```
