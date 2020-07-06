# IATI Graph Database

Microproject focusing on storing an up-to-date version of IATI's entire dataset in a Neo4j graph database.

## Milestones

The project will undertake to do three things:

* Research and test ways of [formatting and storing]() IATI XML data in a graph database
* [Setup and load]() an entire IATI corpus into a test graph database
* [Setup and maintain](https://github.com/Humanitarian-AI/IATI-Graph/milestone/3) an up-to-date version of IATI's entire dataset in a research ready graph database

## IATI Data Formatting and Storage

IATI is an open data sharing framework and XML Standard which over 1000 humanitarian organizations are using to share detailed information on aid activities, transactions and results. IATI is made up of two standards, an Organizations Standard and an Activity Standard.

The project will identify an ideal way to graphically harmonize and format IATI's two different types of data, facilitating extraction, storage and retrieval.

* Lists of IATI elements and activities can be found here: [Organization]() and [Activity]().
* Example XML files containing all of IATI's elements and attributes can be found here: [Organization]() and [Activity]()
* Preview of an actual activity file containing multiple activities: [Oxfam-Jordan](http://preview.iatistandard.org/index.php?url=http%3A//iati.oxfam.org.uk/xml/oxfamgb-jo.xml)
* Source XML file: [Oxfam-Jordan](http://iati.oxfam.org.uk/xml/oxfamgb-jo.xml)

#### Graphical Field Hierarchy

IATI breaks information down in XML elements from "Organizations" to "Organization" and "Activities" to "Activity". Harmonizing Organization and Activity XML files would yield a graphical structure starting with Organizations and breaking down into individual organizations and then each organization's activities and singular activities. Then each activity could be broken down into field elements and attributes.

![IATI Graph Format](https://github.com/Humanitarian-AI/IATI-Graph/blob/master/IATI_Graph_Format.png)

#### Example XML (Three activities and Reporting Organization, Title and Description fields)

```xml
<iati-activities generated-datetime="2020-06-22T00:46:34" version="2.02">
<iati-activity default-currency="GBP" last-updated-datetime="2015-02-19T12:23:58" xml:lang="en">
<iati-identifier>GB-CHC-202918-JORA43</iati-identifier>
<reporting-org ref="GB-CHC-202918" type="21">
<narrative>Oxfam GB</narrative>
</reporting-org>
<title>
<narrative>WASH response in Zataari camp, Jordan</narrative>
</title>
<description type="1">
<narrative>Camp Za'atari population is currently estimated at 32,340 people and is expected to increase to 60,000 people. At least 75% of the refugees are vulnerable women and children and as winter approaches and number continue to increase; the humanitarian situation is likely to worsen. The recommendation proposed Oxfam's to support the implementation of WASH activities in Za'atari camp due to possible high influx of newcomers and the need to enable timely and good standard WASH services for the camp population</narrative>
</description>
</iati-activity>
<iati-activity default-currency="GBP" last-updated-datetime="2020-01-02T18:22:51" xml:lang="en">
<iati-identifier>GB-CHC-202918-JORA51</iati-identifier>
<reporting-org ref="GB-CHC-202918" type="21">
<narrative>Oxfam GB</narrative>
</reporting-org>
<title>
<narrative>Emergency Water, Sanitation and Hygiene activities in host communities in Jordan</narrative>
</title>
<description type="1">
<narrative>This project aims to alleviate the suffering and distinct vulnerabilities of men, women, boys and girls through activities which will be directed towards people affected by the Syrian Crisis including between 30 -40% Jordanians. These activities will seek to improve access to quality WASH services and safe water including storage, conservation, and hygiene/environmental promotion. The interventions will take place in Balqa and Zarqa governorates in 2015.</narrative>
</description>
</iati-activity>
</iati-activities>
```

#### Graphical Format (proposed)

Under Construction

## Data Loading and Testing

Under Construction

## Establish a Research Ready IATI Graph Database

Under Construction
