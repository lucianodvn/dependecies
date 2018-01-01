# dependecies
<repositories>
 		<repository>
 	        <id>spring-milestones</id>
 	        <name>Spring Milestones</name>
 	        <url>http://repo.spring.io/milestone</url>
 	        <snapshots>
 	            <enabled>false</enabled>
 	        </snapshots>
 	    </repository>
 	</repositories>
 	
 	<dependencies>
 		<dependency>
 			<groupId>org.springframework</groupId>
 			<artifactId>spring-webmvc</artifactId>
 			<version>4.1.2.RELEASE</version>
 		</dependency>
 		
 		<dependency>
 			<groupId>org.springframework</groupId>
 			<artifactId>spring-jdbc</artifactId>
 			<version>4.1.2.RELEASE</version>
 		</dependency>
 		<dependency>
 			<groupId>org.springframework</groupId>
 			<artifactId>spring-orm</artifactId>
 			<version>4.1.2.RELEASE</version>
 			<scope>compile</scope>
 		</dependency>
 		<dependency>
 			<groupId>org.springframework</groupId>
 			<artifactId>spring-aop</artifactId>
 			<version>4.1.2.RELEASE</version>
 		</dependency>
 		<dependency>
 			<groupId>org.springframework.data</groupId>
 			<artifactId>spring-data-jpa</artifactId>
 			<version>1.7.1.RELEASE</version>
 		</dependency>
 		
 		
 		<dependency>
 			<groupId>org.hibernate</groupId>
 			<artifactId>hibernate-core</artifactId>
 			<version>4.3.7.Final</version>
 		</dependency>
 		<dependency>
 			<groupId>org.hibernate</groupId>
 			<artifactId>hibernate-entitymanager</artifactId>
 			<version>4.3.7.Final</version>
 		</dependency>
 		<dependency>
 			<groupId>org.hibernate</groupId>
 			<artifactId>hibernate-validator</artifactId>
 			<version>5.1.3.Final</version>
 		</dependency>
 		<dependency>
 			<groupId>org.hibernate</groupId>
 			<artifactId>hibernate-envers</artifactId>
 			<version>4.3.7.Final</version>
 		</dependency>
 		<dependency>
 			<groupId>cglib</groupId>
 			<artifactId>cglib</artifactId>
 			<version>2.2.2</version>
 		</dependency>
 		
 		<dependency>
 			<groupId>mysql</groupId>
 			<artifactId>mysql-connector-java</artifactId>
 			<version>5.1.34</version>
 		</dependency>
 		<dependency>
 			<groupId>com.mchange</groupId>
 			<artifactId>c3p0</artifactId>
 			<version>0.9.2.1</version>
 		</dependency>
 		
 		
 		<dependency>
 			<groupId>javax.servlet</groupId>
 			<artifactId>javax.servlet-api</artifactId>
 			<version>3.0.1</version>
 			<scope>provided</scope>
 		</dependency>
 		<dependency>
 			<groupId>javax.servlet.jsp</groupId>
 			<artifactId>jsp-api</artifactId>
 			<version>2.2.1-b03</version>
 			<scope>provided</scope>
 		</dependency>
 		<dependency>
 			<groupId>javax.servlet</groupId>
 			<artifactId>jstl</artifactId>
 			<version>1.2</version>
 		</dependency>
 		
 		<dependency>
 			<groupId>com.fasterxml.jackson.core</groupId>
 			<artifactId>jackson-databind</artifactId>
 			<version>2.3.1</version>
 		</dependency>
 		
 		<dependency>
 	        <groupId>org.springframework.security</groupId>
 	        <artifactId>spring-security-web</artifactId>
 	        <version>4.0.0.RC2</version>
 	    </dependency>
 		<dependency>
 	        <groupId>org.springframework.security</groupId>
 	        <artifactId>spring-security-config</artifactId>
 	        <version>4.0.0.RC2</version>
 	    </dependency>
 	</dependencies>
 	
 	
 	<build>
 		<plugins>
 			<plugin>
 				<groupId>org.apache.maven.plugins</groupId>
 				<artifactId>maven-war-plugin</artifactId>
 				<version>2.4</version>
 				<configuration>
 					<failOnMissingWebXml>false</failOnMissingWebXml>
 				</configuration>
 			</plugin>
 		
 			<plugin>
 				<groupId>org.apache.maven.plugins</groupId>
 				<artifactId>maven-compiler-plugin</artifactId>
 				<version>2.3.2</version>
 				<configuration>
 					<source>1.8</source>
 					<target>1.8</target>
 				</configuration>
 			</plugin>
 			
 			<plugin>
 				<groupId>org.apache.maven.plugins</groupId>
 				<artifactId>maven-eclipse-plugin</artifactId>
 				<version>2.9</version>
 				<configuration>
 					<downloadSources>true</downloadSources>
 					<downloadJavadocs>true</downloadJavadocs>
 				</configuration>
 			</plugin>
 			
 			<plugin>
 				<groupId>org.mortbay.jetty</groupId>
 				<artifactId>jetty-maven-plugin</artifactId>
 				<version>8.1.16.v20140903</version>
 				<configuration>
 					<scanIntervalSeconds>3</scanIntervalSeconds>
 					<webApp>
 						<contextPath>/pizzaria</contextPath>
 					</webApp>
 				</configuration>
 			</plugin>
 		</plugins>
 	</build>
