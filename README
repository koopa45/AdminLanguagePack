Language pack for the Broadleaf Commerce Admin

Instructions to add this language pack to the Admin Demo:

1) download the Admin Demo from https://github.com/BroadleafCommerce/BroadleafCommerceDemoSite

2) modify the dependency-management section of pom.xml to add the Swedish language dependency.
        <dependency>
            <groupId>org.broadleafcommerce</groupId>
            <artifactId>broadleaf-admin-language-pack-sv</artifactId>
            <version>1.7.0-SNAPSHOT</version>
            <type>jar</type>
            <scope>compile</scope>
        </dependency>

3) modify the dependency section of pom.xml to add the Swedish language dependency.
        <dependency>
            <groupId>org.broadleafcommerce</groupId>
            <artifactId>broadleaf-admin-language-pack-sv</artifactId>
        </dependency>

4) repeat steps 2 - 3 for any other languages you wish to install (e.g. broadleaf-admin-language-pack-es for Spanish, etc...)

5) modify demoAdmin.gwt.xml to include the languages you would like to compile. Here's a sample:

<?xml version="1.0" encoding="UTF-8"?>
<module>
	<inherits name="com.google.gwt.user.User" />
    <inherits name="com.google.gwt.precompress.Precompress"/>
	<inherits name="org.broadleafcommerce.admin.merchandisingModule" />
	<inherits name="org.broadleafcommerce.admin.customerCareModule" />
    <inherits name="org.broadleafcommerce.openadmin.userModule" />
    <inherits name="org.broadleafcommerce.cms.admin.contentManagementModule" />
    <inherits name="com.google.gwt.core.CompilerParameters"/>
    <inherits name="com.google.gwt.i18n.I18N"/>

    <extend-property name="locale" values="en_US"/>
    <extend-property name="locale" values="sv"/>
    <extend-property name="locale" values="es"/>
    <extend-property name="locale" values="fr"/>
    <set-property-fallback name="locale" value="en_US"/>

	<entry-point class="org.broadleafcommerce.openadmin.client.BLCLaunch" />
	<set-property name="user.agent" value="gecko1_8" />
</module>

6) mvn install and launch the admin as normal
     
7) modify the url to add the locale for the changes to occur.

   http://localhost:8080/broadleafdemo/admin.html?locale=sv