# ant-rd
Ant Retrieve and Deploy to copy Salesforce metadata from a package to a development environment. 

The build file uses the [Force.com Migration Tool](https://developer.salesforce.com/page/Force.com_Migration_Tool) and expects Apache Ant to be installed on your system path.

Copy the "build.properties.sample" file to "build.properties" and complete the right side of the property settings with your own details. 

If you are using Windows, you can run the retrieve target, edit the package.xml to remove the namespacePrefix line, and run the deploy target. 

        > ant retrieve
        > (edit package.xml)
        > ant deploy

If you are using OSX or Linux, you can use the fix-manifest script, and the default target. 

        $ ant
