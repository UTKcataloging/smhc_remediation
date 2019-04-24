# Open Refine Template for Smoky Mountain Hiking Club


## Template

#### Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```
####Body

```
<mods>
<identifier type="pid">{{cells['PID'].value}}</identifier>
<identifier type="filename">{{cells['identifier'].value}}</identifier>
<titleInfo><title>{{cells["title"].value}}</title></titleInfo> 
{{if(isBlank(cells['title_alternative'].value), '', '<titleInfo type="alternative"><title>' + cells["title_alternative"].value + '</title></titleInfo>')}}
<abstract>Annual handbook which outlines the Smoky Mountains Hiking Club's schedule of hikes and social events for the year. Includes membership roster and lists committee members.</abstract>
{{if(isBlank(cells['dateIssued'].value), '', '<originInfo><dateIssued>' + cells['dateIssued'].value + '</dateIssued><dateIssued encoding="edtf" keyDate="yes">' + cells['dateIssued_edtf'].value + '</dateIssued></originInfo>')}}
<physicalDescription><extent>6 x 4 inches</extent><form authority="aat" valueURI="http://vocab.getty.edu/aat/300028051">books</form><digitalOrigin>reformatted digital</digitalOrigin></physicalDescription>
{{if(isBlank(cells['DPN_Note'].value), '', '<note displayLabel="dpn">' + cells['DPN_Note'].value + '</note>')}}
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh2009126331"><topic>Hiking--Handbooks, manuals, etc</topic></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh2008121594"><topic>Hiking--Appalachian Trail</topic></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh2006008852"><topic>Trails--Tennessee</topic></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh85136819"><topic>Trails--North Carolina</topic></subject>
<subject authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh89001997"><topic>Associations, institutions, etc.--Membership</topic></subject>
<subject authority="naf" valueURI="http://id.loc.gov/authorities/names/n86844817"><name><namePart>Smoky Mountains Hiking Club of Knoxville</namePart></name></subject>
<subject><geographic authority="lcsh" valueURI="http://id.loc.gov/authorities/subjects/sh85057008">Great Smoky Mountains (N.C. and Tenn.)</geographic><cartographics><coordinates>35.58343, -83.50822</coordinates></cartographics></subject>
<language><languageTerm authority="iso639-2b" type="text">English</languageTerm></language>
<typeOfResource>text</typeOfResource>
<classification authority="lcc">F442.1 .S5</classification>
<relatedItem displayLabel="Project" type="host"><titleInfo><title>Smoky Mountains Hiking Club Handbooks</title></titleInfo></relatedItem>
<location><physicalLocation authority="naf" valueURI="http://id.loc.gov/authorities/names/no2014027633">University of Tennessee, Knoxville. Special Collections</physicalLocation></location>
<recordInfo><languageOfCataloging><languageTerm authority="iso639-2b" type="text">English</languageTerm></languageOfCataloging><recordOrigin>Created and edited in general conformance to MODS Guidelines (Version 3.5).</recordOrigin><recordContentSource valueURI="http://id.loc.gov/authorities/names/n87808088">University of Tennessee, Knoxville. Libraries</recordContentSource></recordInfo>
<accessCondition type="use and reproduction" xlink:href="http://rightsstatements.org/vocab/InC/1.0/">In Copyright</accessCondition>
</mods>
```

#### Suffix

```
</modsCollection>
```