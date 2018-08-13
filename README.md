# sample-maven-junit-war

**************pom.xml******************************
<project>
  
# 4.11 to generate Test result in xml amd txt format

 <dependencies>
   <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.11</version>
      <scope>test</scope>
    </dependency>
  </dependencies>
 
# Generate HTML view to render test result in xml and txt
# HTML report should be generated in  ${basedir}/target/site/surefire-report.html

  <reporting>
    <plugins>
      <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-surefire-report-plugin</artifactId>
        <version>2.5</version>
      </plugin>
    </plugins>
  </reporting>
  
</project>
**********************************************************
#
# mvn clean test surefire-report:report
#

  


  
