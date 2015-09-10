

#Federal Digital System (FDsys) User Guide

##Electronic Code of Federal Regulations (e-CFR) XML User Guide

Prepared by: Office of Programs, Strategy, and Technology

Office of the Chief Technology Officer  
U.S. Government Publishing Office
 

##Revision History

- 1.0 August 2015
  Initial publication

##Table of Contents

[1. Introduction](#1.-Introduction)
[2. XML Version Description](#2.-XML-Version-Description)
[3. Alphabetical List of XML Elements](#3.-Alphabetical-List-of-XML-Elements)
[4. Resources Directory](#4.-Resources-Directory)

# 1. Introduction

The U.S. Government Publishing Office (GPO) and the National Archives and Records Administration's Office of the Federal Register (OFR) are making Electronic Code of Federal Regulation (e-CFR) XML files available via the [FDsys Bulk Data Repository](http://www.gpo.gov/fdsys/bulkdata). The e-CFR is a currently updated version of the Code of Federal Regulations (CFR). It is not an official legal edition of the CFR. The e-CFR is an editorial compilation of CFR material and _Federal Register_ amendments produced by the OFR and the GPO. The OFR will update the material in the e-CFR on an irregular basis that can be as frequent as every day. Please see [www.ecfr.gov](http://www.ecfr.gov/) for additional information.

The effort to provide Federal Government information in more open formats began when the President challenged Federal agencies to create a more open and transparent government, promote accountability, and provide information to citizens about what their Government is doing (see 74 FR 4685, January 26, 2009 at [http://www.gpo.gov/fdsys/pkg/FR-2009-01-26/pdf/E9-1777.pdf](http://www.gpo.gov/fdsys/pkg/FR-2009-01-26/pdf/E9-1777.pdf)). The Director's letter of March 9, 2009 pledged to provide trusted information in whatever form is required to meet the President's objectives [http://www.gpo.gov/pdfs/news-media/letter\_030909.pdf](http://www.gpo.gov/pdfs/news-media/letter_030909.pdf).

## 1.1. Purpose

The purpose of this document is to provide an overview of e-CFR XML files and associated schema. The FDsys Bulk Data repository at [http://www.gpo.gov/fdsys/bulkdata/](http://www.gpo.gov/fdsys/bulkdata/) contains the e-CFR in XML from 2015 forward. Please see FDsys at [www.fdsys.gov](http://www.fdsys.gov/) for access to the CFR Annual Edition and the _Federal Register_ in PDF format.

## 1.2. Legal Status and Authenticity of CFR Files via the FDsys Bulk Data Repository

**Q. What is the data set available for the e-CFR in XML?**

**A.        ** E–CFR files in XML have been converted and simplified from data in SGML that originates at the OFR.  The E–CFR is available in XML starting with the year 2015. Only the most recent e-CFR data will be available at endpoints on the FDsys Bulk Data Repository. Please see [www.ecfr.gov](http://www.ecfr.gov/) to search and browse a point in time edition of the e-CFR.

**Q.  Are e-CFR XML files offered on the FDsys Bulk Data Repository part of the official version of the CFR?**

**A.**  No, the XML-structured files offered for bulk download are not part of the official on-line format of the CFRor the _Federal Register_. While GPO's e-CFR XML files are based on the original source data submitted by Federal agencies and OFR/GPO markup in SGML, only the PDF and Text versions of CFRcontent on FDsys have legal status as parts of the official online format of the CFR.

**Q. Do OFR/GPO plan to include e-CFR XML files as part of the official format of the CFR?**

**A.**  No. The e-CFR XML files are provided as a snapshot of the most current CFR information in XML (with associated graphics).  For official versions of CFR information, refer to the CFR collection on FDsys at:

[http://www.gpo.gov/fdsys/browse/collectionCfr.action?collectionCode=CFR](http://www.gpo.gov/fdsys/browse/collectionCfr.action?collectionCode=CFR)

In particular, refer to the PDF versions found there.

**Q.  Are e-CFR XML bulk download files digitally signed?**

**A.  ** No, XML files available for download are not digitally signed.  They can be manipulated and enriched to operate in the various applications that users may devise.

**Q. How reliable are the metadata and the underlying tagging in bulk data files?**

**A.  ** The document markup and metadata found within bulk data files are generally reliable and complete.  However, there are variations in this underlying data due to inconsistencies in the composition and typesetting process.  As a result, some data-mining applications and user aids may not produce 100 per cent accurate results.

**Q.  What is the legal status of e-CFR user aids?**

**A.** Federal Register user aids, including, finding aids, indexes, search tools, metadata associations, and tagging schemes are not part of the legal text of the CFR.  These ancillary features help users explore and extract data, but the official legal text stands on its own.  No person should form absolute legal conclusions based on search results, finding aids, metadata associations, extractions of data, and the like.  Ultimately, only the official text of the CFR may be relied upon as evidence in a court of law.

**Q.  What is the authenticity of the e-CFR bulk data files after they have been downloaded to another site?  **

**A.**   We cannot vouch for the authenticity of data that is not under OFR/GPO control. OFR and GPO are providing free access to the e-CFR data via XML for display in various applications and mash-ups outside the FDsys domain. OFR and GPO do not endorse third party applications, and do not evaluate how our original legal content is displayed on other sites. Consumers should form their own conclusions as to whether the downloaded data can be relied upon within an application or mash-up. An application may link to the official CFR on FDsys to provide users with additional assurance.

**Q. Do OFR and GPO assert any control over downstream uses of bulk data?**

**A.**  In general, there are no restrictions on re-use of information in the e-CFR documents because U.S. Government works are not subject to copyright. OFR and GPO do not restrict downstream uses of the e-CFR data, except that independent providers should be aware that only the OFR and GPO are entitled to represent that they are the providers of the official versions of the e-CFR and related Federal Register publications.

**Q. How can re-publishers indicate the source of the e-CFR data?**

**A**. Re-publishers of the e-CFR data may cite FDsys and OFR/GPO as the source of their data, and they are free to characterize the quality of data as it appears on their site. But private sector re-publishers are prohibited from using the seal of the National Archives and Records Administration (NARA) or stylized CFR logos identified in NARA regulations (36 CFR part 1200) on their products because that would unlawfully misrepresent the legal status of the material, and could falsely identify private organizations as entities of the Federal Government.

# 2. XML Version Description

The content of the XML e-CFR data provided on the FDsys Bulk Data Repository is derived from that the SGML content on which the print version is based.  In creating the XML content, the SGML content is converted to well-formed XML with minimal intervention.  The resulting XML was built this way for the following reasons:

1. It is a faithful representation of the CFR, which corresponds to the original SGML mark-up.
2. It describes the structure of the CFR, including the large structure (parts, articles, corrections, table of contents, etc.), the document structure (titles, paragraphs, sections, etc.), and semantic structure (CFR references, agency names, contact information, amendment text, etc.)
3. The SGML version on which it is based is almost fully XML-compliant since all element tags have corresponding closing tags as required in XML.

The schema of the incoming SGML content remains essentially unchanged as it is converted to XML without changing any element names. Such an approach maintains fidelity to the original data, and reduces errors that might occur in schema interpretation or further data manipulation.

The changes required to convert the SGML into well-formed XML are as follows:

1. All embedded XML prolog lines of the form `<?xml version="1.0" ?>` are removed.
2. All character entities of the form `"&<name>;"` are replaced with Unicode equivalents or replaced with something else functional.
3. An XML prolog line is prepended to the file and looks like this:
	`<?xml version="1.0" encoding="ISO-8859-1"?>`
4. Links to e-CFR graphics images are adjusted so that their root is as follows:?
  - [www.ecfr.gov](http://www.ecfr.gov/)
5. Standard front matter, such as, the title page and "U.S. Government Official Edition Notice" are normally already removed in the SGML version. In the rare circumstance where it is not removed in the SGML version, it is not copied to the XML version.
6. `<STYLE>` elements are removed from the XML version.

Other than the changes listed above, no SGML tags that are removed or collapsed in the resulting XML.

## 2.1. Outer XML Structure

The XML file has the following overall structure:

```
<?xml version="1.0" encoding="ISO-8859-1"?>
<DLPSTEXTCLASS>
<HEADER>
       <!-- Header information -->
</HEADER>
<TEXT>
      <BODY>
            <ECFRBRWS>
    <!-- e-CFR content -->
            </ECFRBRWS>
      </BODY>
</TEXT>
</DLPSTEXTCLASS>
```
## 2.2. Header Content

There is normally, very little information in the header section. Usually it only contains the number and the title as can be seen in the following example:


```
<FILEDESC>
  <TITLESTMT>
    <TITLE>Title 1: General Provisions</TITLE>
    <AUTHOR TYPE="nameinv"></AUTHOR>
  </TITLESTMT>
  <PUBLICATIONSTMT>
    <PUBLISHER></PUBLISHER>
    <PUBPLACE></PUBPLACE>
    <IDNO TYPE="title">1</IDNO>
    <DATE></DATE>
  </PUBLICATIONSTMT>
  <SERIESSTMT>
    <TITLE></TITLE>
  </SERIESSTMT>
</FILEDESC>
<PROFILEDESC>
  <TEXTCLASS>
    <KEYWORDS></KEYWORDS>
  </TEXTCLASS>
</PROFILEDESC>
```

## 2.3. Sectioning of Body Content

The sectioning of content is managed through the use of` <DIV#>` elements, where # represents a digit such as 1, 2, 3, etc.  For example, the first` <DIV#>` element in the file should be for the Title itself and looks like this:

```
<DIV1 N="1" NODE="5:1" TYPE="TITLE">
```

This indicates that the top level section is a Title and all other `<DIV#>` elements will fall in nested layers within this one.  For the `<DIV1>` element, the value of attribute, N, is the volume number.  For titles that have no volumes, this is "1".  The value of the attribute NODE is a structured value for internal use and may be changed at any time, so it should not be relied on.

In other `<DIV#>` elements, the attribute, N, will be the "number" of the section and the attribute, "TYPE", will be the type of section.  For example, for sub-chapter B, the `<DIV#>` element might read:

` <DIV4 N="B" NODE="1:1.0.1.2" TYPE="SUBCHAP">`

Now since the `<DIV#>` elements are nested within the parent sections that they belong the overall structure may look something like this:

```
<DIV1 N="1" NODE="1:1" TYPE="TITLE">
  …
  <DIV3 N="I" NODE="1:1.0.1" TYPE="CHAPTER">
    …
    <DIV4 N="A" NODE="1:1.0.1.1" TYPE="SUBCHAP">
      …
      <DIV5 N="1" NODE="1:1.0.1.1.1" TYPE="PART">
        …
        <DIV8 N="§ 1.1" NODE="1:1.0.1.1.1.0.1.1" TYPE="SECTION">
          …
        </DIV8>
        …
      </DIV5>
      <DIV5 N="2" NODE="1:1.0.1.1.2" TYPE="PART">
        …
        <DIV8 N="§ 2.1" NODE="1:1.0.1.1.2.0.1.1" TYPE="SECTION">
          …
        </DIV8>
        <DIV8 N="§ 2.2" NODE="1:1.0.1.1.2.0.1.2" TYPE="SECTION">
          …
        </DIV8>
        <DIV8 N="§ 2.3" NODE="1:1.0.1.1.2.0.1.3" TYPE="SECTION">
          …
        </DIV8>
        …
      </DIV5>
      <DIV5 N="3" NODE="1:1.0.1.1.3" TYPE="PART">
        …
        <DIV8 N="§ 3.1" NODE="1:1.0.1.1.3.0.1.1" TYPE="SECTION">
          …
        </DIV8>
        <DIV8 N="§ 3.2" NODE="1:1.0.1.1.3.0.1.2" TYPE="SECTION">
          …
        </DIV8>
        <DIV8 N="§ 3.3" NODE="1:1.0.1.1.3.0.1.3" TYPE="SECTION">
          …
        </DIV8>
        …
      </DIV5>
      …
    </DIV4>
    <DIV4 N="B" NODE="1:1.0.1.2" TYPE="SUBCHAP">
      …
```

Note that though there are `<DIV8>` elements, there are no `<DIV6>` or `<DIV7>` elements in the example above.  While the higher number DIV elements are always nested within lower number DIV elements, they are not required to be sequential.

The title of a section is almost always given by the `<HEAD>` element immediately following the `<DIV#>` element, for example:


```
<DIV4 N="B" NODE="5:1.0.1.2" TYPE="SUBCHAP">
<HEAD>SUBCHAPTER B—CIVIL SERVICE REGULATIONS</HEAD>
```

Note that the `<DIV#>` elements are consistent in their meaning as shown below:

1. DIV1 => TYPE="TITLE"
2. DIV2 => TYPE="SUBTITLE"
3. DIV3 => TYPE="CHAPTER"
4. DIV4 => TYPE="SUBCHAP"
5. DIV5 => TYPE="PART"
6. DIV6 => TYPE="SUBPART"
7. DIV7 => TYPE=" SUBJGRP"
8. DIV8 => TYPE="SECTION"
9. DIV9 => TYPE="APPENDIX"

## 2.4. Paragraphs

The `<P>` element and other elements that are closely related to it (examples: `<PSPACE>`, `<FP>`, `<P-1>`, etc.) are used extensively in the content sections to separate paragraphs.  While paragraphs are often itemized points in an enumerated list with nested sub-lists, the numbering scheme is hardcoded in the content and there is no nesting of elements to preserve indentation levels.  For example:

```
<DIV8 N="§ 151.101" NODE="5:1.0.1.2.12.0.1.1" TYPE="SECTION">
<HEAD>§ 151.101   Definitions.</HEAD>
<P>In this part: </P>
<P>(a) <I>State</I> means a State or territory or possession of the United States. </P>
<P>(b) <I>State or local agency</I> means:</P>
<P>(1) The executive branch of a State, municipality, or other political subdivision of a State, or an agency or department thereof; or</P>
<P>(2) The executive branch of the District of Columbia, or an agency or department thereof.</P>
<P>(c) <I>Federal agency</I> means an executive agency or other agency of the United States, but does not include a member bank of the Federal Reserve System; </P>
<P>(d) <I>State or local officer or employee</I> means an individual employed by a State or local agency whose principal employment is in connection with an activity which is financed in whole or in part by loans or grants made by the United States or a Federal agency but does not include—</P>
<P>(1) An individual who exercises no functions in connection with that activity.</P>
<P>(2) An individual employed by an educational or research institution, establishment, agency, or system which is supported in whole or in part by—</P>
<P>(i) A State or political subdivision thereof;</P>
<P>(ii) The District of Columbia; or</P>
<P>(iii) A recognized religious, philanthropic, or cultural organization.
</P>
<P>(e) <I>Political party</I> means a National political party, a State political party, and an affiliated organization. </P>
<P>(f) <I>Election</I> includes a primary, special, and general election. </P>
<P>(g) <I>Nonpartisan election</I> means an election at which none of the candidates is to be nominated or elected as representing a political party any of whose candidates for Presidential elector receives votes in the last preceding election at which Presidential electors were selected. </P>
<P>(h) <I>Partisan</I> when used as an adjective refers to a political party. </P>
<P>(i) <I>Elective office</I> means any office which is voted upon at an election as defined at § 151.101(f), above, but does not include political party office. </P>
<CITA TYPE="N">[40 FR 42733, Sept. 16, 1975, as amended at 79 FR 25484, May 5, 2014]
</CITA>
</DIV8>
```

The proper indentation of the items in the aforementioned example should probably be as follows:

```
(a)_State_ means a State or territory ...
(b)_State or local agency_ means:
   (1)The executive branch of a State, municipality, ...
   (2)The executive of the District of Columbia, ...
(c)_Federal agency_ means and executive agency or...
(d)_State or local officer or employee_ means an...
   (1)An individual who exercises no functions in ...
   (2)An individual employed by and educational or .
      (i)A State or political subdivision thereof...
      (ii)The District of Columbia; or
      (iii)A recognized religious, philanthropic, or 
          ...
(e)_Political party_ means a National political party, 
(f)_Election_ includes a primary, special, and ...
(g)_Nonpartisan election_ means an election at which ...
(h)_Partisan_ when used as an adjective refers to ...
(i)_Elective office_ means any office which is voted...
```
However, this is not deducible from the XML syntax alone.


## 2.5. Images

If an e-CFR Title has images, they will be in either GIF and/or PDF format.  They will usually be referenced as in the following example:

```
<DIV9 N="Appendix A" NODE="2:1.2.25.3.2.11.51.1.16" TYPE="APPENDIX">
  <HEAD>Appendix A to Part 3485—Covered Transactions</HEAD>
  <img src="http://www.ecfr.gov/graphics/er28mr12.000.gif"/>
  <P/>
  <a href="http://www.ecfr.gov/graphics/pdfs/er28mr12.000.pdf">View or download PDF</a>
  <P/><P/>
</DIV9>
```

As per the example above there are usually both a low-resolution image in GIF format and a high-resolution version by the same base name in PDF format. These links will access the correct images online. However, they are also available in a graphics ZIP archive on the FDsys Bulk Data Repository in the same location as the XML rendition. All the GIF files are in the "graphics" folder within the ZIP file and all the PDF files are within the "pdfs" subfolder.

- ZIP archive
  - o.graphics (folder)
    - er28mr12.000.gif
    - ...
    - pdfs (folder)
      - er28mr12.000.pdf
      - ...

# 3.Alphabetical List of XML Elements

The XML elements that appear in the Titles of the e-CFR are listed below with a brief description of their meaning.  In some cases, the description may include one of the following in square brackets, i.e. [], to show where they are typically used. Note that additional elements may appear in addition to the elements listed below.

- B -- Back Matter
- C -- Table of Contents
- F -- Front Matter
- T -- General textual content

## 3.1. a

This element defines a hyperlink, which is used to link a URL. The most important attribute of the `<a>` element is the "href" attribute, which indicates the link's destination. This is most frequently used to link to an image in the e-CFR Titles.

```
  <a href="http://www.ecfr.gov/graphics/pdfs/er28mr12.000.pdf">View or download PDF</a>
```
## 3.2. ABBR

This element presents a list of abbreviations or acronyms. It is only ever observed inside the `<CFRTOC>` element. [C]

```
<ABBR>
<HED>Abbreviations Used in This Chapter:</HED>
<P>ATF = <I>Alcohol, Tobacco and Firearms.</I> </P>
<P>TD = <I>Treasury Decision.</I></P>
<P>TTB = <I>Alcohol and Tobacco Tax and Trade Bureau.</I></P>
</ABBR>
```

## 3.3. AC

The accent function places certain diacritical marks at letters. The `<AC>` tag follows the letter modified. Usage is `<AC T='d'>` where d is a single digit 0-9:


|Digit|Character|
|-----|--|
|0|&#124;|
|1|é|
|2|	è|
|3|	ê|
|4|ë|
|5|&#9633;|		
|6|	ñ
|7|	å|
|8|	~|
|9|	ç|


These can be used for any letters. Entities (e.g., &eacute;) can accomplish the same effects and are preferable, because they are more intelligible.

```
<FP>and, <I>x<AC T="8"/></I> is the sample mean; n is the number of samples;
and x<E T="52">i</E> is the i<E T="51">th</E> sample; Or,</FP>
```

## 3.4. ALPHHD

This is an alphabet separator heading in agency indexes, i.e. the `<SUBCHIND>` element. [T, B]

```
<HED>INDEX I—RULES RELATING TO PATENTS</HED>
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
<SECHD>Section</SECHD>
<ALPHHD>A</ALPHHD>
<SUBJECT>Abandoned applications:</SUBJECT>
<SUBJ1L>Abandonment by failure to prosecute</SUBJ1L>
<PT>1.135</PT>
<SUBJ1L>Abandonment during interference</SUBJ1L>
```

## 3.5. AMDDATE

This is the amendment date of the title.  This is always found just inside the `<ECFRBRWS>` element.

```
<BODY>
<ECFRBRWS>
<AMDDATE>May 1, 2014</AMDDATE>
<DIV1 N="1" NODE="37:1" TYPE="TITLE">
```

## 3.6. APP
This indicates an appendix, exhibit or supplement heading as contents entry. [C, T]

```
<CFRTOC>
  <EDNOTE>
    <HED>Editorial Note:</HED>
    <PSPACE>Title 5 of the United States Code was revised and enacted into positive law by Pub. L. 89–554, Sept. 6, 1966. New citations for obsolete references to sections of 5 U.S.C. appearing in this volume may be found in a redesignation table under Title 5, Government Organization and Employees, United States Code.</PSPACE>
  </EDNOTE>
  <PTHD>Part</PTHD>
  <CHAPTI>
    <SUBJECT><E T="04">chapter ii</E>—Merit Systems Protection Board</SUBJECT>
    <PG>1200</PG>
    <SUBJECT><E T="04">chapter iii</E>—Office of Management and Budget</SUBJECT>
    <PG>1300</PG>
    …
  </CHAPTI>
  <APP>Appendix A to 5 CFR Chapter XIV—Current Addresses and Geographic Jurisdictions. </APP>
  <APP>Appendix B to 5 CFR Chapter XIV—Memorandum Describing the Authority and Assigned Responsibilities of the General Counsel of the Federal Labor Relations Authority.</APP>
  <CHAPTI>
    <SUBJECT><E T="04">chapter xv</E>—Office of Administration, Executive Office of the President</SUBJECT>
    <PG>2500</PG>
    <SUBJECT><E T="04">chapter xvi</E>—Office of Government Ethics</SUBJECT>
    <PG>2600</PG>
    …
  </CHAPTI>
</CFRTOC>
```

## 3.7. APPRO

This is an OMB number approval note in parentheses. [T]

```
<DIV8 N="§ 1305.3" NODE="5:3.0.2.2.5.0.48.3" TYPE="SECTION">
  <HEAD>§ 1305.3   Procedures in the event of a demand for disclosure.</HEAD>
  <P>(a) Whenever a demand is made upon an employee or former employee of OMB ... </P>
  <P>(b) If information or material is sought by a demand in any case or ... </P>
  <P>(c) If response to a demand is required before instructions from the ... </P>
  <APPRO TYPE="N">(Approved by the Office of Management and Budget under control number 0348–0056)</APPRO>
</DIV8>
```

## 3.8. AUTH

This is an authority statement that usually contains a mini-header.  Almost every `<DIV#>` element has one.

```
<DIV5 N="1" NODE="37:1.0.1.1.1" TYPE="PART">
<HEAD>PART 1—RULES OF PRACTICE IN PATENT CASES</HEAD>
<AUTH>
  <HED>Authority:</HED>
  <PSPACE>35 U.S.C. 2(b)(2), unless otherwise noted.</PSPACE>
</AUTH>
<SOURCE>
  <HED>Source:</HED>
  <PSPACE>24 FR 10332, Dec. 22, 1959, unless otherwise noted.</PSPACE>
</SOURCE>
```

## 3.9. AUTHOR

This element designates an author although there are currently no examples of where an author is actually named.  The TYPE attribute has been observed to have the value "nameinv" or "author".

```
<TITLESTMT>
  <TITLE>Title 37: Patents, Trademarks, and Copyrights</TITLE>
  <AUTHOR TYPE="nameinv"></AUTHOR>
</TITLESTMT>
```

## 3.10. B

This element represents a span of text stylistically different from normal text, without conveying any special importance or relevance. It is typically used for keywords in a summary, product names in a review, or other spans of text whose typical presentation would be boldfaced. Another example of its use is to mark the lead sentence of each paragraph of an article.

Note:  The `<B>` element should not be confused with the `<strong>` or `<em>` elements. The `<strong>` element represents text of certain importance, while `<em>` puts some emphasis on the text.  The `<b>` element does not convey such special semantic information; it is used when the others do not fit.

```
<P>(ii) $10,000; whichever is higher, unless the employee has elected a Living Benefit under subpart K of this part. Effective for pay periods beginning on or after October 30, 1998, there is no maximum BIA. <B>Note:</B> If an employee's pay is "capped" by law, the amount of the Basic insurance is based on the capped amount, which is the amount the employee is actually being paid. It is not based on the amount the employee's pay would have been without the pay cap.</P>
```

## 3.11. BCAP

This is a bottom caption for a graphic or mathpac insert. [T]

```
<img src="http://www.ecfr.gov/graphics/ec27oc91.004.gif"/>
<BCAP><E T="15">Figure D-4—Ladder Far from Wall</E></BCAP>
```

## 3.12. BODY

This element encapsulates the body content of an e-CFR Title and occurs exactly once per e-CFR XML document.  It occurs separately (outside of) the `<header>` element but is found within a `<TEXT>` element.  See [Section 2.1](#2.1.-Outer-XML-Structure)

## 3.13. BOXTXT

This marks text surrounded with a box. [T]

```
<BOXTXT>
  <P>Drugs with thyroid hormone activity, alone or together with other therapeutic agents, have been used for the treatment of obesity. In euthyroid patients, doses within the range of daily hormonal requirements are ineffective for weight reduction. Larger doses may produce serious or even life-threatening manifestations of toxicity, particularly when given in association with sympathomimetic amines such as those used for their anorectic effects.</P>
</BOXTXT>
```

## 3.14. br

The `<br>` tag inserts a single line break.


```
<br/>—Department of the Environment.
<br/>—Department of General Services.
<br/>—Department of Housing and Community Development.
<br/>—Department of Human Resources.
<br/>—Department of Licensing and Regulation.
<br/>—Department of Natural Resources.
<br/>—Department of Public Safety and Correctional Services.
<br/>—Department of Personnel.
<br/>—Department of Transportation.
```

## 3.15. CFRTOC

A table of contents is given within this element.  It is only ever seen inside a `<DIV1>` element.

```
<CFRTOC>
  <PTHD>Part</PTHD>
  <CHAPTI>
    <SUBJECT><E T="04">chapter i</E>—United States Patent and Trademark Office, Department of Commerce</SUBJECT>
    <PG>1</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter ii</E>—U.S. Copyright Office, Library of Congress</SUBJECT>
    <PG>201</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter iii</E>—Copyright Royalty Board, Library of Congress</SUBJECT>
    <PG>301</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter iv</E>—Assistant Secretary for Technology Policy, Department of Commerce</SUBJECT>
    <PG>401</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter v</E>—Under Secretary for Technology, Department of Commerce</SUBJECT>
    <PG>501</PG>
  </CHAPTI>
</CFRTOC>
```

## 3.16. CHAPNO

This is a chapter number and has special use in table of contents and a few others cases. [C, B]

```
<DIV2 N="Subtitle E" NODE="41:4.1" TYPE="SUBTITLE">
  <HEAD>Subtitle E—Federal Information Resources Management Regulations System</HEAD>
  <CHAPNO>CHAPTER 201 [RESERVED]</CHAPNO>
</DIV2>
```

## 3.17. CHAPTI

This element has special use in table of contents, i.e. `<CFRTOC>`.  It is a single element within a parts list. [F, C]

```
<CFRTOC>
  <PTHD>Part</PTHD>
  <CHAPTI>
    <SUBJECT><E T="04">chapter i</E>—United States Patent and Trademark Office, Department of Commerce</SUBJECT>
    <PG>1</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter ii</E>—U.S. Copyright Office, Library of Congress</SUBJECT>
    <PG>201</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter iii</E>—Copyright Royalty Board, Library of Congress</SUBJECT>
    <PG>301</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter iv</E>—Assistant Secretary for Technology Policy, Department of Commerce</SUBJECT>
    <PG>401</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter v</E>—Under Secretary for Technology, Department of Commerce</SUBJECT>
    <PG>501</PG>
  </CHAPTI>
</CFRTOC>
```

## 3.18. CITA

This is a source note at the section level. Alone, it marks a one-column citation.

```
<DIV8 N="§ 1.3" NODE="37:1.0.1.1.1.1.66.3" TYPE="SECTION">
  <HEAD>§ 1.3   Business to be conducted with decorum and courtesy.</HEAD>
  <P>Applicants and their attorneys or agents are required to conduct their business with the United States Patent and Trademark Office with decorum and courtesy. Papers presented in violation of this requirement will be submitted to the Director and will not be entered. A notice of the non-entry of the paper will be provided. Complaints against examiners and other employees must be made in correspondence separate from other papers.</P>
  <CITA TYPE="N">[68 FR 38624, June 30, 2003]</CITA>
</DIV8>
```

## 3.19. CROSSREF

This is a cross reference note.

```
<DIV5 N="93" NODE="29:1.1.1.1.38" TYPE="PART">
  <HEAD>PART 93—NEW RESTRICTIONS ON LOBBYING</HEAD>
  <AUTH>
    <HED>Authority:</HED>
    <PSPACE>Section 319, Public Law 101-121 (31 U.S.C. 1352); 5 U.S.C. 301, Reorganization Plan Number 6 of 1950.</PSPACE>
  </AUTH>
  <SOURCE>
    <HED>Source:</HED>
    <PSPACE>55 FR 6737 and 6751, Feb. 26, 1990, unless otherwise noted.</PSPACE>
  </SOURCE>
  <CROSSREF>
    <HED>Cross Reference:</HED>
    <P>See also Office of Management and Budget notice published at 54 FR 52306, December 20, 1989.</P>
  </CROSSREF>
```

## 3.20. DATE

This is a date specification.  This tag is frequently empty/has no value.

```
<PUBLICATIONSTMT>
  <PUBLISHER></PUBLISHER>
  <PUBPLACE></PUBPLACE>
  <IDNO TYPE="title">37</IDNO>
  <DATE></DATE>
</PUBLICATIONSTMT>
```

## 3.21. DIV

This is a division or section of a document that is grouped into a block, often for formatting purposes.

```
<DIV9 N="Appendix to" NODE="37:1.0.1.4.15.2.214.15.2" TYPE="APPENDIX">
  <HEAD>Appendix to Part 102—Systems of Records Noticed by Other Federal Agencies
<SU>1</SU> and Applicable to USPTO Records and Applicability of This Part Thereto</HEAD>
  <DIV width="100%">
    <DIV class="gpotbl\_div">
      <TABLE border="1" cellpadding="1" cellspacing="1" class="gpotbl\_table" frame="void" width="100%">
        <TR>
          <TH class="gpotbl\_colhed" scope="col">Category of records</TH>
          <TH class="gpotbl\_colhed" scope="col">Other federal agency</TH>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Federal Personnel Records</TD>
          <TD align="left" class="gpotbl\_cell">Office of Personnel Management.
<sup>2</sup></TD>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Federal Employee Compensation Act Program</TD>
          <TD align="left" class="gpotbl\_cell">Department of Labor.
<sup>3</sup></TD>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Equal Employment Opportunity Appeal Complaints</TD>
          <TD align="left" class="gpotbl\_cell">Equal Employment Opportunity Commission.
<sup>4</sup></TD>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Formal Complaints/Appeals of Adverse Personnel Actions</TD>
          <TD align="left" class="gpotbl\_cell">Merit Systems Protection Board.
<sup>5</sup></TD>
        </TR>
      </TABLE>
    </DIV>
    <DIV class="table\_foot">
      <P class="gpotbl\_note">
        <sup>1</sup> Other than systems of records noticed by the Department of Commerce. Where the system of records applies only to USPTO, these regulations apply. Where the system of records applies generally to components of the Department of Commerce, the regulations of that department attach at the point of any denial for access or for correction or amendment.
      </P>
      <P class="gpotbl\_note">
        <sup>2</sup> The provisions of this part do not apply to these records covered by notices of systems of records published by the Office of Personnel Management for all agencies. The regulations of OPM alone apply.
      </P>
      <P class="gpotbl\_note">
        <sup>3</sup> The provisions of this part apply only initially to these records covered by notices of systems of records published by the U.S. Department of Labor for all agencies. The regulations of that department attach at the point of any denial for access or for correction or amendment.
      </P>
      <P class="gpotbl\_note">
        <sup>4</sup> The provisions of this part do not apply to these records covered by notices of systems of records published by the Equal Employment Opportunity Commission for all agencies. The regulations of the Commission alone apply.
      </P>
      <P class="gpotbl\_note">
        <sup>5</sup> The provisions of this part do not apply to these records covered by notices of systems of records published by the Merit Systems Protection Board for all agencies. The regulations of the Board alone apply.
      </P>
    </DIV>
  </DIV>
</DIV9>
```
## 3.22. DIV1

This element denotes the first-level subdivision of the content body of the XML document. For e-CFR documents this element encapsulates the body of an entire CFR Title or CFR Title volume. The values of the "N" and "TYPE" attributes are always set to "1" and "TITLE" respectively in the e-CFR XML data when there are no volumes. Otherwise, "N" will have the number of the volume. Other subdivision elements such as `<DIV2>`, `<DIV3>`, and so on, will be nested within this element.

```
<?xml version="1.0" ?>
<DLPSTEXTCLASS>
  <HEADER>
    …
  </HEADER>
  <TEXT>
    <BODY>
      <ECFRBRWS>
        <AMDDATE>Mar. 31, 2014</AMDDATE>
          <DIV1 N="1" NODE="1:1" TYPE="TITLE">
            …
          </DIV1>
      </ECFRBRWS>
    </BODY>
  </TEXT>
</DLPSTEXTCLASS>
```

## 3.23. DIV2

This element denotes the second-level subdivision of the content body of the XML document.  For e-CFR documents this element encapsulates the body of a CFR Sub-Title. The value of the "N" attribute will be the number of the CFR Sub-Title and the value of the "TYPE" attribute will be "SUBTITLE". This element may only reside inside of a `<DIV#>` element where # is a number lower than "2".

```
<DIV2 N="Subtitle B" NODE="2:1.3" TYPE="SUBTITLE">
<HEAD>Subtitle B-Federal Agency Regulations for Grants and Agreements</HEAD>
```

## 3.24. DIV3

This element denotes the third-level subdivision of the content body of the XML document. For e-CFR documents this element encapsulates the body of a Chapter. The value of the "N" attribute will be the number of the Chapter and the value of the "TYPE" attribute will be "CHAPTER".  This element may only reside inside of a `<DIV#>` element where # is a number lower than "3".

```
<DIV3 N="I" NODE="5:1.0.1" TYPE="CHAPTER">
<HEAD> CHAPTER I—OFFICE OF PERSONNEL MANAGEMENT</HEAD>
```

## 3.25. DIV4

This element denotes the fourth-level subdivision of the content body of the XML document.  For e-CFR documents this element encapsulates the body of a Sub-Chapter. The value of the "N" attribute will be the number of the Sub-Chapter and the value of the "TYPE" attribute will be "SUBCHAP". This element may only reside inside of a `<DIV#>` element where # is a number lower than "4".

```
<DIV4 N="B" NODE="5:1.0.1.2" TYPE="SUBCHAP">
<HEAD>SUBCHAPTER B—CIVIL SERVICE REGULATIONS </HEAD>
```

## 3.26. DIV5

This element denotes the fifth-level subdivision of the content body of the XML document. For e-CFR documents this element encapsulates the body of a Part. The value of the "N" attribute will be the number of the Part and the value of the "TYPE" attribute will be "PART". This element may only reside inside of a `<DIV#>` element where # is a number lower than "5".

```
<DIV5 N="9" NODE="5:1.0.1.1.9" TYPE="PART">
<HEAD>PART 9—WORKFORCE INFORMATION (RULE IX)</HEAD>
```

## 3.27. DIV6

This element denotes the sixth-level subdivision of the content body of the XML document. For e-CFR documents this element encapsulates the body of a Sub-Part. The value of the "N" attribute will be the number of the Sub-Part and the value of the "TYPE" attribute will be "SUBPART".  This element may only reside inside of a `<DIV#>` element where # is a number lower than "6".

```
<DIV6 N="C" NODE="5:1.0.1.2.16.3" TYPE="SUBPART">
<HEAD>Subpart C—Administrative Offset</HEAD>
```

## 3.28. DIV7

This element denotes the seventh-level subdivision of the content body of the XML document.  For e-CFR documents this element encapsulates the body of a Subject Group. The value of the "N" attribute will be the number of the Subject Group and the value of the "TYPE" attribute will be "SUBJGRP". This element may only reside inside of a `<DIV#>` element where # is a number lower than "7".

```
<DIV7 N="2" NODE="5:1.0.1.2.12.0.2" TYPE="SUBJGRP">
<HEAD>Permissible Activities</HEAD>
```

## 3.29. DIV8

This element denotes the eighth-level subdivision of the content body of the XML document.  For e-CFR documents this element encapsulates the body of a Section. The value of the "N" attribute will be the number of the Section and the value of the "TYPE" attribute will be "SECTION". This element may only reside inside of a `<DIV#>` element where # is a number lower than "8".

```
<DIV8 N="§ 177.110" NODE="5:1.0.1.2.14.0.4.10" TYPE="SECTION">
<HEAD>§ 177.110   Action on approved claim.</HEAD>
```

## 3.30. DIV9

This element denotes the ninth-level subdivision of the content body of the XML document. For e-CFR documents this element encapsulates the body of an Appendix. The value of the "N" attribute will be the number of the Appendix and the value of the "TYPE" attribute will be "APPENDIX".

```
<DIV9 N="Appendix B" NODE="5:1.0.1.2.80.3.96.11.15" TYPE="APPENDIX">
<HEAD>Appendix B to Subpart C of Part 591—Daily Inconvenience or Hardship Allowance Schedule, Commuting Over Land by Motor Vehicle to Remote Duty Posts</HEAD>
```

## 3.31. DLPSTEXTCLASS

This is the root element of any one of the e-CFR Titles. This element only occurs once in each XML document and encapsulates all the rest of the XML data. See [Section 2.1](#2.1.-Outer-XML-Structure)

## 3.32. DOCKETHD

This indicates a docket heading in an appendix, exhibit, or extract. [T]

```
<EXTRACT>
  <FP>(Date)</FP>
  <P>Division of Dockets Management, Food and Drug Administration, Department of Health and Human Services, 5630 Fishers Lane, rm. 1061, Rockville, MD 20852.</P>
  <HD1>Notice of Participation</HD1>
  <DOCKETHD>Docket No. \_\_</DOCKETHD>
  <P>Under 21 CFR part 12, please enter the participation of:</P>
  <FP-DASH>(Name)</FP-DASH>
  <FP-DASH>(Street address)</FP-DASH>
  <FP-DASH>(City and State)</FP-DASH>
  <FP-DASH>(Telephone number)</FP-DASH>
```

## 3.33. E

This element is used to denote emphasis (change face) where type attribute, "T", suggests the following emphasis style:

- `<E T='01'>`  standard c & lc light-face Roman (this is NOT used to end any of the other font changes below; </E> is used for that purpose)
- `<E T='02'>` boldface
- `<E T='03'>`  italic
- `<E T='04'>`  cap & small cap (figures are small)
- `<E T='05'>`  cap & small cap (figures are full) (this is the default for tags that supply c & sc emphasis, e.g., `<EDNOTE>`)

When used with other Grid and Table numbers, certain characters will print superior or inferior (`<E T='51'>` or `<E T='52'>`) or a character or entity will appear as some other character (e.g., `<E T='61'>&plusmn;</E>` becomes a ±, though in this example the emphasis tag is no longer necessary).

```
<SUBJECT><E T="04">chapter i</E>—Office of Personnel Management</SUBJECT>
```

## 3.34. ECFRBRWS

This element encapsulates all the body content for an e-CFR Title. It is always found immediately after the `<BODY>` element.

```
<BODY>
  <ECFRBRWS>
    <AMDDATE>May 1, 2014</AMDDATE>
    <DIV1 N="1" NODE="37:1" TYPE="TITLE">
```

## 3.35. EDNOTE

This is meant for inserting an editorial note. Alone, it marks a one-column citation. The tag is immediately followed by `<HED>`. [F, C, T, B]

```
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
```

## 3.36. EFFDNOT

This is an effective date note. Alone it marks a one-column citation. The tag is normally followed by a `<HED>` element, which is styled differently than the subsequent note. [F, C, T, B]

```
<DIV5 N="502" NODE="29:3.1.1.1.3" TYPE="PART">
  <HEAD>PART 502—ENFORCEMENT OF CONTRACTUAL OBLIGATIONS FOR TEMPORARY ALIEN AGRICULTURAL WORKERS ADMITTED UNDER SECTION 218 OF THE IMMIGRATION AND NATIONALITY ACT (SUSPENDED 6-29-2009)</HEAD>
  <AUTH>
    <HED>Authority:</HED>
    <PSPACE>8 U.S.C. 1101(a)(15)(H)(ii)(a), 1184(c), and 1188. </PSPACE>
  </AUTH>
  <SOURCE>
    <HED>Source:</HED>
    <PSPACE>73 FR 77229, Dec. 18, 2008, unless otherwise noted.</PSPACE>
  </SOURCE>
  <EFFDNOT>
    <HED>Effective Date Note:</HED>
    <PSPACE>At 74 FR 26008, May 29, 2009, part 501 was redesignated as part 502, and newly designated part 502 was suspended, effective June 29, 2009.</PSPACE>
  </EFFDNOT>
```

## 3.37. EFTNT

This is a footnote within and appendix or extract that stays in place rather than printing at the bottom of the column.

```
<EXTRACT>
  <FP-2>Class 1. Flue-cured types.</FP-2>
  <FP-2>Class 2. Fire-cured types.</FP-2>
  <FP-2>Class 3. <SU>1</SU> Air-cured types.</FP-2>
  <FP-2>Class 4. Cigar-filler types.</FP-2>
  <FP-2>Class 5. Cigar-binder types.</FP-2>
  <FP-2>Class 6. Cigar-wrapper types.</FP-2>
  <FP-2>Class 7. Miscellaneous domestic types.</FP-2>
  <FP-2>Class 8. Foreign-grown cigar-leaf types.</FP-2>
  <FP-2>Class 9. Foreign-grown types, other than cigar types.</FP-2>
  <EFTNT>
    <P><SU>1</SU> Class 3 covers Air-cured tobacco other than cigar leaf. This class may be subdivided as follows: Class 3a, Light Air-cured tobacco, including types 31 and 32, and Class 3b, Dark Air-cured tobacco, including types 35, 36, and 37.</P>
  </EFTNT>
</EXTRACT>
```

## 3.38. em

This element denotes that the enclosed text is emphasized.

```
<P>Identify the highest applicable rate range for the employee's grade after promotion based on consideration of any pay schedule that applied to the employee's position of record <em>before</em> promotion (after any geographic conversion). (Do not consider pay schedules that apply only to the employee's new position of record after… </P>
```

## 3.39. EXAMPLE

This element denotes an example to be introduced by the text in the `<HED>` element, which is usually set in italic. Space should be supplied as needed. The opening tag is immediately followed by the `<HED>` element. The first `<P>` following the `<HED>` element should add word space and change back to the regular font, such as, Roman c & lc. [T, B]


```
<EXAMPLE>
  <HED>Example 1:</HED>
  <PSPACE>An employee of the Department of Education may serve as a delegate, alternate, or proxy to a State or national party convention.</PSPACE>
</EXAMPLE>
<EXAMPLE>
  <HED>Example 2:</HED>
  <PSPACE>A noncareer member of the Senior Executive Service, or other employee covered under this subpart, may serve as a vice-president of a political action committee, as long as the duties of the office do not involve personal solicitation, acceptance, or receipt of political contributions. Ministerial activities which precede or follow the official acceptance and receipt, such as handling, disbursing, or accounting for contributions are not covered under the definitions of <I>accept</I> and <I>receive</I> in § 734.101. Sections 734.208 and 734.303 describe in detail permitted and prohibited activities which are related to fundraising.</PSPACE>
</EXAMPLE>
```

## 3.40. EXTRACT

This element is for (quoted material, addresses, lists, etc.) where other tags are inappropriate.  This will often be rendered with note-sized type.  [T, B]


```
<EXTRACT>
  <FP-1>City of \_\_\_\_</FP-1>
  <FP-1>County of \_\_\_\_ :ss</FP-1>
  <FP-1>(Name of individual), who affixed (his) (her) signature below in my presence, came before me, a (title), in and for the aforesaid County and State, this \_\_\_ day of \_\_\_, 20\_, and established (his) (her) identity to my satisfaction.</FP-1>
  <FP-1>My commission expires \_\_\_\_.</FP-1>
  <FP>(Signature)</FP>
</EXTRACT>
```

## 3.41. FILEDESC

This is one of the top-level elements within the `<HEADER>` element. See [Section 2.2](#2.2.-Header-Content)

## 3.42. FL-2

This element contains a left column item in leaderwork text, i.e. `<LDRWK>`. [T]


```
<DIV8 N="§ 2.6" NODE="37:1.0.1.2.5.0.142.3" TYPE="SECTION">
  <HEAD>§ 2.6   Trademark fees.</HEAD>
  <P>The Patent and Trademark Office requires the following fees and charges:</P>
  <P>(a) Trademark process fees.</P>
  <LDRWK>
    <FL-2>(1) Application filing fees.</FL-2>
    <FL-2>(i) For filing an application on paper, per class </FL-2>
    <LDRFIG>$375.00</LDRFIG>
    <FL-2>(ii) For filing an application through TEAS, per class </FL-2>
    <LDRFIG>$325.00</LDRFIG>
```

## 3.43. FP

This indicates a flush paragraph with flush overs. [T, B]

```
<EXTRACT>
  <FP>The undersigned being warned that willful false statements and the like are punishable by fine or imprisonment, or both, under 18 U.S.C. 1001, and that such willful false statements and the like may jeopardize the validity of the application or document or any registration resulting therefrom, declares that all statements made of his/her own knowledge are true; and all statements made on information and belief are believed to be true.</FP>
</EXTRACT>
```

## 3.44. FP-1

This indicates a flush paragraph with one-level turnovers. [T]


```
<EXTRACT>
  <FP-1>City of \_\_\_\_</FP-1>
  <FP-1>County of \_\_\_\_ :ss</FP-1>
  <FP-1>(Name of individual), who affixed (his) (her) signature below in my presence, came before me, a (title), in and for the aforesaid County and State, this \_\_\_ day of \_\_\_, 20\_, and established (his) (her) identity to my satisfaction.</FP-1>
  <FP-1>My commission expires \_\_\_\_.</FP-1>
  <FP>(Signature)</FP>
</EXTRACT>
```


## 3.45. FP-2

This indicates a flush paragraph with two-level turnovers. [T]


```
<EXTRACT>
  <HD1>Appendix A to § 201.33—Notice of Intent To Enforce a Copyright Restored under the Uruguay Round Agreements Act (URAA)</HD1>
  <FP-DASH>1. Title:</FP-DASH>
  <P>(If this work does not have a title, state "No title.") OR</P>
  <P>Brief description of work (for untitled works only): \_\_\_\_</P>
  <FP-DASH></FP-DASH>
  <FP-DASH>2. English translation of title (if applicable):</FP-DASH>
  <FP-DASH>3. Alternative title(s) (if any):</FP-DASH>
  <FP-DASH>4. Type of work:</FP-DASH>
  <P>(e.g. painting, sculpture, music, motion picture, sound recording, book)</P>
  <FP-DASH>5. Name of author(s):</FP-DASH>
  <FP-DASH>6. Source country:</FP-DASH>
  <FP-DASH>7. Approximate year of publication:</FP-DASH>
  <FP-DASH>8. Additional identifying information:</FP-DASH>
  <FP1-2>(e.g. for movies; director, leading actors, screenwriter, animator, for photographs: subject matter; for books; editor, publisher, contributors, subject matter).</FP1-2>
  <FP-DASH>9. Name of copyright owner:</FP-DASH>
  <FP1-2>(Statements may be filed in the name of the owner of the restored copyright or the owner of an exclusive right therein.)</FP1-2>
  <FP-2>10. If you are not the owner of all rights, specify the rights you own:</FP-2>
  <FP-DASH></FP-DASH>
  <FP1-2>(e.g. the right to reproduce/distribute publicly display/publicly perform the work, or to prepare a derivative work based on the work)</FP1-2>
  <FP-2>11. Address at which copyright owner may be contacted:</FP-2>
  <FP-DASH></FP-DASH>
  <FP-DASH></FP-DASH>
  <FP1-2>(Give the complete address, including the country and an "attention" line, or "in care of" name, if necessary.)</FP1-2>
  <FP-DASH>12. Telephone number of owner:</FP-DASH>
  <FP-DASH>13. Telefax number of owner:</FP-DASH>
  <FP-2>14. Certification and Signature:</FP-2>
  <P>I hereby certify that, for each of the work(s) listed above, I am the copyright owner, or the owner of an exclusive right, or the owner's authorized agent, the agency relationship having been constituted in a writing signed by the owner before the filing of this notice, and that the information given herein is true and correct to the best of my knowledge.</P>
  <FP-DASH>Signature:</FP-DASH>
  <FP-DASH>Name (printed or typed):</FP-DASH>
  <FP-DASH>As agent for (if applicable):</FP-DASH>
  <FP-DASH>Date:</FP-DASH>
</EXTRACT>
```

## 3.46. FP-DASH

This indicates flush text with remainder of line supplied with horizontal lowline-dash rule (as used with forms). It should only be used within extract or appendix. [T]


```
<EXTRACT>
  <HD1>Appendix A to § 201.33—Notice of Intent To Enforce a Copyright Restored under the Uruguay Round Agreements Act (URAA)</HD1>
  <FP-DASH>1. Title:</FP-DASH>
  <P>(If this work does not have a title, state "No title.") OR</P>
  <P>Brief description of work (for untitled works only): \_\_\_\_</P>
  <FP-DASH></FP-DASH>
  <FP-DASH>2. English translation of title (if applicable):</FP-DASH>
  <FP-DASH>3. Alternative title(s) (if any):</FP-DASH>
  <FP-DASH>4. Type of work:</FP-DASH>
  <P>(e.g. painting, sculpture, music, motion picture, sound recording, book)</P>
  <FP-DASH>5. Name of author(s):</FP-DASH>
  <FP-DASH>6. Source country:</FP-DASH>
  <FP-DASH>7. Approximate year of publication:</FP-DASH>
  <FP-DASH>8. Additional identifying information:</FP-DASH>
  <FP1-2>(e.g. for movies; director, leading actors, screenwriter, animator, for photographs: subject matter; for books; editor, publisher, contributors, subject matter).</FP1-2>
  <FP-DASH>9. Name of copyright owner:</FP-DASH>
  <FP1-2>(Statements may be filed in the name of the owner of the restored copyright or the owner of an exclusive right therein.)</FP1-2>
  <FP-2>10. If you are not the owner of all rights, specify the rights you own:</FP-2>
  <FP-DASH></FP-DASH>
  <FP1-2>(e.g. the right to reproduce/distribute publicly display/publicly perform the work, or to prepare a derivative work based on the work)</FP1-2>
  <FP-2>11. Address at which copyright owner may be contacted:</FP-2>
  <FP-DASH></FP-DASH>
  <FP-DASH></FP-DASH>
  <FP1-2>(Give the complete address, including the country and an "attention" line, or "in care of" name, if necessary.)</FP1-2>
  <FP-DASH>12. Telephone number of owner:</FP-DASH>
  <FP-DASH>13. Telefax number of owner:</FP-DASH>
  <FP-2>14. Certification and Signature:</FP-2>
  <P>I hereby certify that, for each of the work(s) listed above, I am the copyright owner, or the owner of an exclusive right, or the owner's authorized agent, the agency relationship having been constituted in a writing signed by the owner before the filing of this notice, and that the information given herein is true and correct to the best of my knowledge.</P>
  <FP-DASH>Signature:</FP-DASH>
  <FP-DASH>Name (printed or typed):</FP-DASH>
  <FP-DASH>As agent for (if applicable):</FP-DASH>
  <FP-DASH>Date:</FP-DASH>
</EXTRACT>
```

## 3.47. FP1-2

This indicates a first-level indented paragraph with two-level turnovers. [T]


```
<EXTRACT>
  <HD1>Appendix A to § 201.33—Notice of Intent To Enforce a Copyright Restored under the Uruguay Round Agreements Act (URAA)</HD1>
  <FP-DASH>1. Title:</FP-DASH>
  <P>(If this work does not have a title, state "No title.") OR</P>
  <P>Brief description of work (for untitled works only): \_\_\_\_</P>
  <FP-DASH></FP-DASH>
  <FP-DASH>2. English translation of title (if applicable):</FP-DASH>
  <FP-DASH>3. Alternative title(s) (if any):</FP-DASH>
  <FP-DASH>4. Type of work:</FP-DASH>
  <P>(e.g. painting, sculpture, music, motion picture, sound recording, book)</P>
  <FP-DASH>5. Name of author(s):</FP-DASH>
  <FP-DASH>6. Source country:</FP-DASH>
  <FP-DASH>7. Approximate year of publication:</FP-DASH>
  <FP-DASH>8. Additional identifying information:</FP-DASH>
  <FP1-2>(e.g. for movies; director, leading actors, screenwriter, animator, for photographs: subject matter; for books; editor, publisher, contributors, subject matter).</FP1-2>
  <FP-DASH>9. Name of copyright owner:</FP-DASH>
  <FP1-2>(Statements may be filed in the name of the owner of the restored copyright or the owner of an exclusive right therein.)</FP1-2>
  <FP-2>10. If you are not the owner of all rights, specify the rights you own:</FP-2>
  <FP-DASH></FP-DASH>
  <FP1-2>(e.g. the right to reproduce/distribute publicly display/publicly perform the work, or to prepare a derivative work based on the work)</FP1-2>
  <FP-2>11. Address at which copyright owner may be contacted:</FP-2>
  <FP-DASH></FP-DASH>
  <FP-DASH></FP-DASH>
  <FP1-2>(Give the complete address, including the country and an "attention" line, or "in care of" name, if necessary.)</FP1-2>
  <FP-DASH>12. Telephone number of owner:</FP-DASH>
  <FP-DASH>13. Telefax number of owner:</FP-DASH>
  <FP-2>14. Certification and Signature:</FP-2>
  <P>I hereby certify that, for each of the work(s) listed above, I am the copyright owner, or the owner of an exclusive right, or the owner's authorized agent, the agency relationship having been constituted in a writing signed by the owner before the filing of this notice, and that the information given herein is true and correct to the best of my knowledge.</P>
  <FP-DASH>Signature:</FP-DASH>
  <FP-DASH>Name (printed or typed):</FP-DASH>
  <FP-DASH>As agent for (if applicable):</FP-DASH>
  <FP-DASH>Date:</FP-DASH>
</EXTRACT>
```

## 3.48. FP2

This denotes a flush paragraph with two-level turnovers.  [T]


```
<FP-2>MCF<E T="52">i</E> = Moisture correction factor for the measurement period, volumetric basis.</FP-2>
<FP2>= 1 when V<E T="52">i</E> and C<E T="52">i</E> are measured on a dry basis or if both are measured on a wet basis.</FP2>
<FP2>= 1-(f<E T="52">H2O</E>)<E T="52">I</E> when V<E T="52">i</E> is measured on a wet basis and C<E T="52">i</E> is measured on a dry basis.</FP2>
<FP2>= 1/[1-(f<E T="52">H2O</E>)<E T="52">i</E>] when V<E T="52">i</E> is measured on a dry basis and C<E T="52">i</E> is measured on a wet basis.</FP2>
<FP-2>(f<E T="52">H2O</E>) = Moisture content of the CH<E T="52">4</E> emitted during the measurement period, volumetric basis (cubic feet water per cubic feet emitted gas).                  </FP-2>
```

## 3.49. FP2-2

This is a second-level indented paragraph with two-level turnovers. [T]

```
<EXTRACT>
  <FP2-2>The FTC's Franchise Rule permits a franchisor to provide information about the actual or potential financial performance of its franchised and/or franchisor-owned outlets, if there is a reasonable basis for the information, and if the information is included in the disclosure document. Financial performance information that differs from that included in Item 19 may be given only if: (1) a franchisor provides the actual records of an existing outlet you are considering buying; or (2) a franchisor supplements the information provided in this Item 19, for example, by providing information about possible performance at a particular location or under particular circumstances.</FP2-2>
</EXTRACT>
```

## 3.50. FP2-3

This is a second-level indented paragraph with three-level turnovers. [T]

```
<EXTRACT>
  <P>Respectfully submitted,</P>
  <FRP>Harold R. Tyler, Jr.,</FRP>
  <FP2-3>Deputy Attorney General and Chairman of the Equal Employment Coordinating Council.</FP2-3>
  <FRP>Michael H. Moskow,</FRP>
  <FP2-3>Under Secretary of Labor.</FP2-3>
  <FRP>Ethel Bent Walsh,</FRP>
  <FP2-3>Acting Chairman, Equal Employment Opportunity Commission.</FP2-3>
  <FRP>Robert E. Hampton,</FRP>
  <FP2-3>Chairman, Civil Service Commission.</FP2-3>
  <FRP>Arthur E. Flemming,</FRP>
  <FP2-3>Chairman, Commission on Civil Rights.</FP2-3>
</EXTRACT>
```

## 3.51. FR

This indicates a fractional number.


```
<NOTE>
  <HED>Note:</HED>
  <P>Notices of Intent to Enforce must be in English, except for the original title, and either typed or printed by hand legibly in dark, preferably black, ink. They should be on 8<FR>1/2</FR>" by 11" white paper of good quality, with at least a 1-inch (or 3 cm) margin.</P>
</NOTE>
```

## 3.52. FRP

This denotes a flush right text (left is ragged), held one em from right margin. [T]


```
<EXTRACT>
  <P>Respectfully submitted,</P>
  <FRP>Harold R. Tyler, Jr.,</FRP>
  <FP2-3>Deputy Attorney General and Chairman of the Equal Employment Coordinating Council.</FP2-3>
  <FRP>Michael H. Moskow,</FRP>
  <FP2-3>Under Secretary of Labor.</FP2-3>
  <FRP>Ethel Bent Walsh,</FRP>
  <FP2-3>Acting Chairman, Equal Employment Opportunity Commission.</FP2-3>
  <FRP>Robert E. Hampton,</FRP>
  <FP2-3>Chairman, Civil Service Commission.</FP2-3>
  <FRP>Arthur E. Flemming,</FRP>
  <FP2-3>Chairman, Commission on Civil Rights.</FP2-3>
</EXTRACT>
```

## 3.53. FRP0

This denotes true flush right material where the left side is ragged.  [T]


```
<MATH BORDER="NODRAW" DEEP="31" HTYPE="CENTER" POSITION="NOFLOAT" ROTATION="P" SPAN="1" STRIP="YES">
  <img src="http://www.ecfr.gov/graphics/ec15no91.094.gif"/>
</MATH>
<FRP0>Equation 1</FRP0>
<FP>where:</FP>
<FP-2>A<E T="52">s</E>=Response for the parameter to be measured.</FP-2>
<FP-2>A<E T="52">is</E>=Response for the internal standard.</FP-2>
<FP-2>C<E T="52">is</E>=Concentration of the internal standard.</FP-2>
<FP-2>C<E T="52">s</E>=Concentration of the parameter to be measured.</FP-2>
```

## 3.54. FTNT

This marks footnote text, which is meant to be placed immediately after text containing `<FTREF>` tag.

```
<FTREF/>
</P>
<FTNT>
  <P>
    <SU>4</SU> An <I>author</I> includes an employer or other person for whom a work is "made for hire" under 17 U.S.C. 101. This paragraph does not permit an employee or other person working "for hire" under that section to make a later registration in his or her own name. In the case of authors of a joint work, this paragraph does permit a later registration by one author in his or her own name as copyright claimant, where an earlier registration identifies only another author as claimant.
  </P>
</FTNT>
```

## 3.55. FTREF

This is a footnote reference and should be followed by `<FTNT>`text`</FTNT>`.

```
<FTREF/>
</P>
<FTNT>
  <P>
    <SU>4</SU> An <I>author</I> includes an employer or other person for whom a work is "made for hire" under 17 U.S.C. 101. This paragraph does not permit an employee or other person working "for hire" under that section to make a later registration in his or her own name. In the case of authors of a joint work, this paragraph does permit a later registration by one author in his or her own name as copyright claimant, where an earlier registration identifies only another author as claimant.
  </P>
</FTNT>
```

## 3.56. HALFDASH

This means to write-in the line starting midway through the column.  [T]


```
<EXTRACT>
  <P>I certify that CBP baggage declaration requirements have been made known to incoming passengers; that any required CBP baggage declarations have been or will simultaneously herewith be filed as required by law and regulation with the proper CBP officer; and that the responsibilities devolving upon this vessel in connection therewith, if any, have been or will be discharged as required by law or regulation before the proper CBP officer. I further certify that there are no steerage passengers on board this vessel (46 U.S.C. 151-163).</P>
  <HALFDASH></HALFDASH>
  <FRP>Master</FRP>
</EXTRACT>
```

## 3.57. HD1 – HD6

These are headings that usually print centered (two lines or fewer) or flush left and hang (three or more lines).  Suggested styles for the various levels are given below:

```
<TEXT>:
<HD1> 8 pt. Ionic  Cap & Small Cap Roman
<HD2> 8 pt. Ionic  Cap & lower italic
<HD3> 8 pt. Ionic  Cap & lower Roman
<HD4> 8 pt. Ionic  Cap & Small Cap Roman
<HD5> 8 pt. Century Cap & lower bold Roman flush left (and hang)
<HD6> 8 pt. Ionic  Cap & lower italic

<EXTRACT>:
<HD1> 7 pt. Ionic  Cap & Small Cap Roman
<HD2> 7 pt. Ionic  Cap & lower italic
<HD3> 7 pt. Ionic  Cap & lower Roman
<HD4> 7 pt. Helvetica Cap & lower bold Roman
<HD5> 8 pt. Helvetica Cap & lower bold Roman
<HD6> 7 pt. Helvetica Cap & lower bold Roman
```

```
<EXTRACT>
  <HD1>Appendix B to § 201.39—Required Format for Continuation Sheet</HD1>
  <FP-2>NLA CON</FP-2>
  <FP-2>Page \_\_of \_\_Pages.</FP-2>
  <HD3>Continuation Sheet for NLA Notice to Libraries and Archives of Normal Commercial Exploitation or Availability at Reasonable Price</HD3>
  <P>1. Title of the work (or, if untitled, a brief description of the work): \_\_\_\_\_\_\_\_\_\_.</P>
  <P>2. Type of work (e.g. music, motion picture, book, photograph, illustration, map, article in a periodical, painting, sculpture, sound recording, etc.): \_\_\_\_\_\_\_\_\_\_.</P>
  <P>3. Edition, if any (e.g., first edition, second edition, teacher's edition) or version, if any (e.g., orchestral arrangement, English translation of French text). If there is no information available relating to the edition or version of the work, the Notice should state, "No information available": \_\_\_\_\_\_\_\_\_\_.</P>
  <P>4. Copyright renewal registration number (not required for foreign works restored under 17 U.S.C. 104A): \_\_\_\_\_\_\_\_\_\_.</P>
  <HD2>Additional Content (OPTIONAL):</HD2>
  <P>5. Original copyright registration number: \_\_\_\_\_\_\_\_\_\_.</P>
  <P>6. Additional information concerning the work's normal commercial exploitation or availability at a reasonable price: \_\_\_\_\_\_\_\_\_\_.</P>
</EXTRACT>
```

## 3.58. HEAD

This element provides a major heading/title for sections, i.e. `<DIV1>` – `<DIV9>` elements.


```
<DIV5 N="1" NODE="37:1.0.1.1.1" TYPE="PART">
  <HEAD>PART 1—RULES OF PRACTICE IN PATENT CASES</HEAD>
  <AUTH>
    <HED>Authority:</HED>
    <PSPACE>35 U.S.C. 2(b)(2), unless otherwise noted.</PSPACE>
  </AUTH>
  <SOURCE>
    <HED>Source:</HED>
    <PSPACE>24 FR 10332, Dec. 22, 1959, unless otherwise noted.</PSPACE>
  </SOURCE>
```

## 3.59. HEADER

This element contains the Header section of each XML document.  It occurs exactly once per XML document and it occurs immediately following the root element.  See [Section 2.1](#2.1.-Outer-XML-Structure)


## 3.60.HED

This marks text following other tags for special handling such as applying a style to offset the text from that which follows. [C, T, B]


```
<EDNOTE>
  <HED>Editorial Note:</HED>
  <PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE>
</EDNOTE>
```

## 3.61. HED1

This indicates a heading that is intended to be centered. [T]


```
<DIV4 N="A" NODE="37:1.0.1.1" TYPE="SUBCHAP">
  <HEAD>SUBCHAPTER A—GENERAL</HEAD>
  <TEXT>
    <HED1>
      <I>PATENTS</I>
    </HED1>
  </TEXT>
<DIV5 N="1" NODE="37:1.0.1.1.1" TYPE="PART">
```

## 3.62. I

This element defines a part of text in an alternate voice or mood. The content of the <i> tag is often rendered in italics.  The <i> tag can be used to indicate a technical term, a phrase from another language, a thought, or a name, etc.  This element is normally only used when there is not a more appropriate semantic element, such as:

- `<em>` (emphasized text)
- `<strong>` (important text)
- `<cite>` (the title of a work)

```
   <P><I>Regulation</I> and <I>rule</I> have the same meaning. </P>
```

## 3.63. IDNO

This element is used to specify the number of the CFR Title that the e-CFR XML document represents.

```
  <PUBLICATIONSTMT>
    <PUBLISHER></PUBLISHER>
    <PUBPLACE></PUBPLACE>
    <IDNO TYPE="title">1</IDNO>
    <DATE></DATE>
  </PUBLICATIONSTMT>
```

## 3.64. img

This element defines the location of an image within the document. It has one required attribute, namely, "src".  The "src" attribute specifies the URL of the image.

```
  <img src="http://www.ecfr.gov/graphics/er28mr12.000.gif"/>
```

## 3.65.KEYWORDS

This element is the only element found within the `<TEXTCLASS>` element and is always found to be empty so far. See [Section 2.2](#2.2.-Header-Content)

## 3.66.LDRFIG

This element contains a right column item in leaderwork text, i.e. `<LDRWK>`. [T]


```
<DIV8 N="§ 2.6" NODE="37:1.0.1.2.5.0.142.3" TYPE="SECTION">
  <HEAD>§ 2.6   Trademark fees.</HEAD>
  <P>The Patent and Trademark Office requires the following fees and charges:</P>
  <P>(a) Trademark process fees.</P>
  <LDRWK>
    <FL-2>(1) Application filing fees.</FL-2>
    <FL-2>(i) For filing an application on paper, per class </FL-2>
    <LDRFIG>$375.00</LDRFIG>
    <FL-2>(ii) For filing an application through TEAS, per class </FL-2>
    <LDRFIG>$325.00</LDRFIG>
```

## 3.67.LDRWK

This element encapsulates data at right and left ends of a line that are separated by leaders; usually preferable to using a table. [T]

```
<DIV8 N="§ 2.6" NODE="37:1.0.1.2.5.0.142.3" TYPE="SECTION">
  <HEAD>§ 2.6   Trademark fees.</HEAD>
  <P>The Patent and Trademark Office requires the following fees and charges:</P>
  <P>(a) Trademark process fees.</P>
  <LDRWK>
    <FL-2>(1) Application filing fees.</FL-2>
    <FL-2>(i) For filing an application on paper, per class </FL-2>
    <LDRFIG>$375.00</LDRFIG>
    <FL-2>(ii) For filing an application through TEAS, per class </FL-2>
    <LDRFIG>$325.00</LDRFIG>
    …
  </LDRWK>
```

## 3.68.LI

This is a list item that can be used in tables, but especially used with the `<SCOL2>` element.

```
<EXTRACT>
  <SCOL2>
    <LI>Gallon gal</LI>
    <LI>quart qt</LI>
    <LI>pint pt</LI>
    <LI>ounce oz</LI>
    <LI>pound lb</LI>
    <LI>grain gr</LI>
    <LI>kilogram kg</LI>
    <LI>gram g</LI>
    <LI>milligram mg</LI>
    <LI>microgram mcg</LI>
    <LI>liter l</LI>
    <LI>milliliter ml</LI>
    <LI>cubic centimeter cc</LI>
    <LI>yard yd</LI>
    <LI>feet or foot ft</LI>
    <LI>inch in</LI>
    <LI>meter m</LI>
    <LI>centimeter cm</LI>
    <LI>millimeter mm</LI>
    <LI>fluid fl</LI>
    <LI>square sq</LI>
    <LI>weight wt</LI>
  </SCOL2>
</EXTRACT>
```

## 3.69.MATH

This normally begins and ends location where MathType equations are supplied; a number of attributes can be indicated, such as column span, depth, indention, rotation, etc. (`<MATH SPAN='2' DEEP='250'>`).


```
<MATH BORDER="NODRAW" DEEP="26" HTYPE="CENTER" POSITION="NOFLOAT" ROTATION="P" SPAN="2" STRIP="YES">
<img src="http://www.access.gpo.gov/ecfr/graphics/er28fe00.001.gif"/>
</MATH>
```

## 3.70.NOTE

This element is used to contain a note. The `<HED>` element is meant to be displayed as Caps and Small Caps with space supplied above and below. [F, C, T, B]

```
<NOTE>
  <HED>Note to § 1.16:</HED>
  <P>See §§ 1.445, 1.482 and 1.492 for international application filing and processing fees.</P>
</NOTE>
```

## 3.71.P

This element defines a paragraph, that is, text that is set apart from the text before or after it.

```
<HEAD>§ 1.1   Definitions.</HEAD>
<P>As used in this chapter, unless the context requires otherwise—</P>
<P><I>Administrative Committee</I> means the Administrative Committee of the Federal Register established under section 1506 of title 44, United States Code; </P>
```

## 3.72.P-1

This is a first-level indented paragraph.

```
<P>2.1.3<I>Common evaluations.</I> Evaluations common to all four HRS pathways include:</P>
<P>• Characterizing sources.</P>
<P-1>-Identifying sources (and, for the soil exposure pathway, areas of observed contamination [see section 5.0.1]).</P-1>
<P-1>-Identifying hazardous substances associated with each source (or area of observed contamination).</P-1>
<P-1>-Identifying hazardous substances available to a pathway.</P-1>
```

## 3.73.P-2

This is a second-level indented paragraph.

```
<HD1>A.5.4Examples of Scientifically Validated Test Methods</HD1>
<FP-2>A.5.4.1Examples of <I>in vivo</I> heritable germ cell mutagenicity tests are:</FP-2>
<P-2>(a) Rodent dominant lethal mutation test (OECD 478)</P-2>
<P-2>(b) Mouse heritable translocation assay (OECD 485)</P-2>
<P-2>(c) Mouse specific locus test</P-2>
```

## 3.74.P-3

This is a first-level indented paragraph with three-level turnovers.  [T]

```
<DIV9 N="Appendix A" NODE="40:1.0.1.1.19.0.1.11.3" TYPE="APPENDIX">
  <HEAD>Appendix A to Part 20—Guidelines for Certification</HEAD>
  <FP-2>1. General.</FP-2>
  <FP-2>2. Air Pollution Control Facilities.</FP-2>
  <P-3>a. Pollution control or treatment facilities normally eligible for certification.</P-3>
  <P-3>b. Air pollution control facility boundaries.</P-3>
  <P-3>c. Examples of eligibility limits.</P-3>
  <P-3>d. Replacement of manufacturing process by another nonpolluting process.</P-3>
  <FP-2>3. Water Pollution Control Facilities.</FP-2>
<P-3>a. Pollution control or treatment facilities normally eligible for certification.</P-3>
```

## 3.75.P-DASH

This is a first-level indented phrase with the remainder of line composed of low-line dashes.  This is frequently used in forms.  [T]

```
<EXTRACT>
  <P-DASH>Product </P-DASH>
  <P2>(State whether raw milk, pasteurized milk, raw cream, or pasteurized cream.) </P2>
  <P-DASH>Permit number </P-DASH>
  <P2>Federal Import Milk Act, Department of Health and Human Services. </P2>
  <P-DASH>Shipper </P-DASH>
  <P-DASH>Address of shipper</P-DASH>
</EXTRACT>
```

## 3.76.P1

This is a first-level indented paragraph with one-level turnovers. [T]

```
<EXTRACT>
  <FRP>(Date)</FRP>
  <FP-DASH>Name of petitioner</FP-DASH>
  <FP-DASH>Post-office address</FP-DASH>
  <FP-DASH>Date</FP-DASH>
  <FP-DASH>Name of food additive and proposed use</FP-DASH>
  <FP-DASH></FP-DASH>
  <P>Office of Food Additive Safety (HFS-200), Center for Food Safety and Applied Nutrition, Food and Drug Administration, 5100 Paint Branch Pkwy., College Park, MD 20740.</P>
  <FP><E T="04">Dear Sirs:</E></FP>
  <P>The undersigned, \_\_\_\_\_ submits this petition pursuant to section 409(b)(1) of the Federal Food, Drug, and Cosmetic Act with respect to \_\_\_\_\_</P>
  …
  <P>H. The petitioner is required to submit either a claim for categorical exclusion under § 25.30 or 25.32 of this chapter or an environmental assessment under § 25.40 of this chapter. </P>
  <P1>Yours very truly,</P1>
  <FP-DASH>Petitioner</FP-DASH>
  <FP-DASH>By</FP-DASH>
  <FRP>(Indicate authority)</FRP>
</EXTRACT>
```

## 3.77.P2

This is a second-level indented paragraph. [T]

```
<EXTRACT>
  <P-DASH>Product </P-DASH>
  <P2>(State whether raw milk, pasteurized milk, raw cream, or pasteurized cream.) </P2>
  <P-DASH>Permit number </P-DASH>
  <P2>Federal Import Milk Act, Department of Health and Human Services. </P2>
  <P-DASH>Shipper </P-DASH>
  <P-DASH>Address of shipper</P-DASH>
</EXTRACT>
```

## 3.78.PARAUTH

This is used to indicate the paragraph authority (Authority: ...).  The editor should supply space above and below. [T]

```
<PARAUTH TYPE="N">(18 U.S.C., section 1001 (1986))</PARAUTH>
```

## 3.79.PARTHD

This is a part header that has special use in contents and regular text.  [C, T]

```
<PARTHD>Part 4—Preparation of the DD Form 250 and DD Form 250C</PARTHD>
<SECHD>F-401Preparation instructions.</SECHD>
<P>(a) <I>General.</I></P>
```

## 3.80.PG

This is used to supply page number data in lists, contents. [F, C, T, B]


```
<CFRTOC>
  <PTHD>Part</PTHD>
  <CHAPTI>
    <SUBJECT><E T="04">chapter i</E>—United States Patent and Trademark Office, Department of Commerce</SUBJECT>
    <PG>1</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter ii</E>—U.S. Copyright Office, Library of Congress</SUBJECT>
    <PG>201</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter iii</E>—Copyright Royalty Board, Library of Congress</SUBJECT>
    <PG>301</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter iv</E>—Assistant Secretary for Technology Policy, Department of Commerce</SUBJECT>
    <PG>401</PG>
  </CHAPTI>
  …
</CFRTOC>
```

## 3.81.PROFILEDESC

This element contains a profile description.  It is never observed to be populated. It is found inside the `<HEADER>` element. See [Section 2.2](#2.2.-Header-Content)

## 3.82.PSPACE

This is a special type of paragraph text that can follow an in-line heading, whereas the `<P>` element will normally cause undesired line breaks to occur before the text begins.


```
<EDNOTE>
  <HED>Editorial Note:</HED>
  <PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE>
</EDNOTE>
```

## 3.83.PT

This has special use in contents and indexes. [C, B]

```
<HED>INDEX I—RULES RELATING TO PATENTS</HED>
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
<SECHD>Section</SECHD>
<ALPHHD>A</ALPHHD>
<SUBJECT>Abandoned applications:</SUBJECT>
<SUBJ1L>Abandonment by failure to prosecute</SUBJ1L>
<PT>1.135</PT>
<SUBJ1L>Abandonment during interference</SUBJ1L>
<PT>41.127(b)</PT>
<SUBJ1L>Abandonment for failure to pay issue fee</SUBJ1L>
<PT>1.316</PT>
```

## 3.84.PTHD

This is a special use header for contents and indexes. [C, B]

```
<CFRTOC>
  <PTHD>Part</PTHD>
  <CHAPTI>
    <SUBJECT><E T="04">chapter i</E>—United States Patent and Trademark Office, Department of Commerce</SUBJECT>
    <PG>1</PG>
  </CHAPTI>
  <CHAPTI>
    <SUBJECT><E T="04">chapter ii</E>—U.S. Copyright Office, Library of Congress</SUBJECT>
    <PG>201</PG>
  </CHAPTI>
  …
</CFRTOC>
```

## 3.85.PUBLICATIONSTMT

This is a publication statement element that may be found in a couple of places inside the `<HEADER>` element.

```
<PUBLICATIONSTMT>
  <PUBLISHER></PUBLISHER>
  <PUBPLACE></PUBPLACE>
  <IDNO TYPE="title">37</IDNO>
  <DATE></DATE>
</PUBLICATIONSTMT>
```

## 3.86.PUBLISHER

This element gives the publisher's name and is found inside the `<PUBLICATIONSTMT>` element. It has not been found to contain a value so far.

```
<PUBLICATIONSTMT>
  <PUBLISHER></PUBLISHER>
  <PUBPLACE></PUBPLACE>
  <IDNO TYPE="title">37</IDNO>
  <DATE></DATE>
</PUBLICATIONSTMT>
```

## 3.87.PUBPLACE

This element gives the publisher's location and is found inside the `<PUBLICATIONSTMT>` element. It has not been found to contain a value so far.

```
<PUBLICATIONSTMT>
  <PUBLISHER></PUBLISHER>
  <PUBPLACE></PUBPLACE>
  <IDNO TYPE="title">37</IDNO>
  <DATE></DATE>
</PUBLICATIONSTMT>
```

## 3.88.RESERVED

This is used in place of `<SUBJECT>` or, after `<PART>`, in place of `<HED>`, where they are [Reserved].

```
<DIV2 N="" NODE="41:3.9" TYPE="SUBTITLE">
  <RESERVED>Subtitle D. Other Provisions Relating to Property Management [Reserved]
</RESERVED>
</DIV2>
```

## 3.89.REVTXT

This is used in editorial and effective date notes for text to be revised. [T]

```
<EFFDNOT>
  <HED>Effective Date Note:</HED>
  <PSPACE>At 67 FR 41823, June 20, 2002, § 352.20 was amended by revising paragraphs (a)(1) through (a)(2), effective Sept. 1, 2002. This amendment could not be incorporated because at 66 FR 67485, Dec. 31, 2001 the effective date was stayed until further notice. For the convenience of the user, the text is set forth as follows:</PSPACE>
  <REVTXT>
    <HEAD>§ 352.20   Permitted combinations of active ingredients.</HEAD><STARS/>
    <P>(a) <I>Combinations of sunscreen active ingredients.</I> (1) Two or more sunscreen active ingredients identified in § 352.10(a), (c), (e), (f), (g), and (i) through (r) may be combined with each other in a single product when used in the concentrations established for each ingredient in § 352.10. The concentration of each active ingredient must be sufficient to contribute a minimum SPF of not less than 2 to the finished product. The finished product must have a minimum SPF of not less than the number of sunscreen active ingredients used in the combination multiplied by 2.</P>
    <P>(2) Two or more sunscreen active ingredients identified in § 352.10(b), (c), (e), (g), (j) through (m), (o), and (q) may be combined with each other in a single product when used in the concentrations established for each ingredient in § 352.10. The concentration of each active ingredient must be sufficient to contribute a minimum SPF of not less than 2 to the finished product. The finished product must have a minimum SPF of not less than the number of sunscreen active ingredients used in the combination multiplied by 2.</P><STARS/>
  </REVTXT>
</EFFDNOT>
```

## 3.90.SCOL2

This is used for long lists of short terms with each on its own line, so that two narrow columns will appear in one text-width column (each entry is tagged with `<LI>`).

```
<EXTRACT>
  <SCOL2>
    <LI>Gallon gal</LI>
    <LI>quart qt</LI>
    <LI>pint pt</LI>
    <LI>ounce oz</LI>
    <LI>pound lb</LI>
    <LI>grain gr</LI>
    <LI>kilogram kg</LI>
    <LI>gram g</LI>
    <LI>milligram mg</LI>
    <LI>microgram mcg</LI>
    <LI>liter l</LI>
    <LI>milliliter ml</LI>
    <LI>cubic centimeter cc</LI>
    <LI>yard yd</LI>
    <LI>feet or foot ft</LI>
    <LI>inch in</LI>
    <LI>meter m</LI>
    <LI>centimeter cm</LI>
    <LI>millimeter mm</LI>
    <LI>fluid fl</LI>
    <LI>square sq</LI>
    <LI>weight wt</LI>
  </SCOL2>
</EXTRACT>
```

## 3.91.SECAUTH

This is used to indicate the section authority (Authority: ...).  This element should automatically supply space above and below. [T]

```
<SECAUTH TYPE="N">(Pub. L. 94-131, 89 Stat. 685; 35 U.S.C. 6, Pub. L. 97-247) </SECAUTH>
```

## 3.92.SECHD

This is used for the "Sec." appearing in the contents [C, T]

```
<HED>INDEX I—RULES RELATING TO PATENTS</HED>
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
<SECHD>Section</SECHD>
<ALPHHD>A</ALPHHD>
<SUBJECT>Abandoned applications:</SUBJECT>
<SUBJ1L>Abandonment by failure to prosecute</SUBJ1L>
<PT>1.135</PT>
<SUBJ1L>Abandonment during interference</SUBJ1L>
```

## 3.93.SECTNO

This is a section number: without "§" in contents; with "§" at section heading. [C, T, B]

```
<DIV6 N="D" NODE="21:8.0.1.1.15.4" TYPE="SUBPART">
  <HEAD>Subpart D—FDA as an Issuing Agency</HEAD>
  <SOURCE>
    <HED>Source:</HED>
    <PSPACE>78 FR 55826, Sept. 24, 2013, unless otherwise noted.</PSPACE>
  </SOURCE>
  <SECTNO>§ 830.200</SECTNO>
  <SUBJECT>When FDA will act as an issuing agency.</SUBJECT>
```

## 3.94.SERIESSTMT

This element contains a series statement. It is never observed to be populated with any meaningful data. It is found inside the `<FILEDESC>` element. [Section 2.2](#2.2.-Header-Content)

## 3.95.SOURCE

This is a source statement that usually contains a mini-header. Almost every `<DIV#>` element has one.

```
<DIV5 N="1" NODE="37:1.0.1.1.1" TYPE="PART">
<HEAD>PART 1—RULES OF PRACTICE IN PATENT CASES</HEAD>
<AUTH>
  <HED>Authority:</HED>
  <PSPACE>35 U.S.C. 2(b)(2), unless otherwise noted.</PSPACE>
</AUTH>
<SOURCE>
  <HED>Source:</HED>
  <PSPACE>24 FR 10332, Dec. 22, 1959, unless otherwise noted.</PSPACE>
</SOURCE>
```

## 3.96.STARS

This marks dropped text.

```
<EXTRACT>
  <P>(b) The provisions of section 7 shall not apply with respect to:</P>
</EXTRACT>
<STARS/>
<EXTRACT>
  <P>(11) any employee employed as a driver or driver's helper making local deliveries, who is compensated for such employment on the basis of trip rates, or other delivery payment plan, if the Secretary shall find that such plan has the general purpose and effect of reducing hours worked by such employees to, or below, the maximum workweek applicable to them under section 7(a).</P>
</EXTRACT>
```

## 3.97.strong

This element denotes that the enclosed text is important.

```
<P class="gpotbl\_note"><sup>a</sup> <strong>Note:</strong> These alternate standards for 2016 and later are the same as the otherwise applicable standards for 2017 and later.</P>
```

## 3.98.SU

This indicates superscript text.

```
<FTNT>
  <P>
    <SU>4</SU> An <I>author</I> includes an employer or other person for whom a work is "made for hire" under 17 U.S.C. 101. This paragraph does not permit an employee or other person working "for hire" under that section to make a later registration in his or her own name. In the case of authors of a joint work, this paragraph does permit a later registration by one author in his or her own name as copyright claimant, where an earlier registration identifies only another author as claimant.
  </P>
</FTNT>
```

## 3.99.sub

This indicates that the enclosed text is subscripted.

```
<P class="gpotbl\_note">Let <em>M</em><sub>2</sub>, <em>M</em><sub>3</sub> . . . <em>M</em><sub>n</sub> be donor masses to be combined.</P>
```

## 3.100.SUBCHIND

This element is used to hold an agency indexes in Title 37. [Text]

```
<SUBCHIND>
<HED>INDEX I—RULES RELATING TO PATENTS</HED>
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
<SECHD>Section</SECHD>
<ALPHHD>A</ALPHHD>
<SUBJECT>Abandoned applications:</SUBJECT>
<SUBJ1L>Abandonment by failure to prosecute</SUBJ1L>
<PT>1.135</PT>
<SUBJ1L>Abandonment during interference</SUBJ1L>
```

## 3.101.SUBJ1L

This has special use in indexes under second-level division head. It will usually be styled with leaders. [B]

```
<HED>INDEX I—RULES RELATING TO PATENTS</HED>
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
<SECHD>Section</SECHD>
<ALPHHD>A</ALPHHD>
<SUBJECT>Abandoned applications:</SUBJECT>
<SUBJ1L>Abandonment by failure to prosecute</SUBJ1L>
<PT>1.135</PT>
<SUBJ1L>Abandonment during interference</SUBJ1L>
```

## 3.102.SUBJ2L

This has special use in indexes under third-level division head. It will usually be styled with leaders. [B]

```
<SUBJECT>Extension of patent term. (See also Patent term adjustment):</SUBJECT>
<SUBJ1L>Due to examination delay under the URAA (35 U.S.C. 154)</SUBJ1L>
<PT>1.701</PT>
<SUBJECT1>Due to regulatory review period (35 U.S.C. 156):</SUBJECT1>
<SUBJ2L>Applicant for</SUBJ2L>
<PT>1.730</PT>
<SUBJ2L>Application for</SUBJ2L>
<PT>1.740</PT>
<SUBJECT2>Calculation of term:</SUBJECT2>
<SUBJ3L>Animal Drug Product</SUBJ3L>
<PT>1.778</PT>
<SUBJ3L>Food or color additive</SUBJ3L>
<PT>1.776</PT>
```

## 3.103.SUBJ3L

This has special use in indexes under fourth-level division head. It will usually be styled with leaders. [B]

```
<SUBJECT>Extension of patent term. (See also Patent term adjustment):</SUBJECT>
<SUBJ1L>Due to examination delay under the URAA (35 U.S.C. 154)</SUBJ1L>
<PT>1.701</PT>
<SUBJECT1>Due to regulatory review period (35 U.S.C. 156):</SUBJECT1>
<SUBJ2L>Applicant for</SUBJ2L>
<PT>1.730</PT>
<SUBJ2L>Application for</SUBJ2L>
<PT>1.740</PT>
<SUBJECT2>Calculation of term:</SUBJECT2>
<SUBJ3L>Animal Drug Product</SUBJ3L>
<PT>1.778</PT>
<SUBJ3L>Food or color additive</SUBJ3L>
<PT>1.776</PT>
```

## 3.104.SUBJECT

This is used in a table of contents and at section head levels to mark section heading text [F, C, T, B]

```
<HED>INDEX I—RULES RELATING TO PATENTS</HED>
<EDNOTE>
<HED>Editorial Note:</HED><PSPACE>This listing is provided for informational purposes only. It is compiled and kept current by the Department of Commerce. This index is updated as of July 1, 2012.</PSPACE></EDNOTE>
<SECHD>Section</SECHD>
<ALPHHD>A</ALPHHD>
<SUBJECT>Abandoned applications:</SUBJECT>
<SUBJ1L>Abandonment by failure to prosecute</SUBJ1L>
<PT>1.135</PT>
<SUBJ1L>Abandonment during interference</SUBJ1L>
```

## 3.105.SUBJECT1
This is a second-level division head in indexes. [B]

```
<SUBJECT>Extension of patent term. (See also Patent term adjustment):</SUBJECT>
<SUBJ1L>Due to examination delay under the URAA (35 U.S.C. 154)</SUBJ1L>
<PT>1.701</PT>
<SUBJECT1>Due to regulatory review period (35 U.S.C. 156):</SUBJECT1>
<SUBJ2L>Applicant for</SUBJ2L>
<PT>1.730</PT>
<SUBJ2L>Application for</SUBJ2L>
<PT>1.740</PT>
<SUBJECT2>Calculation of term:</SUBJECT2>
<SUBJ3L>Animal Drug Product</SUBJ3L>
<PT>1.778</PT>
<SUBJ3L>Food or color additive</SUBJ3L>
<PT>1.776</PT>
```

## 3.106.SUBJECT2

This is a third-level division head in indexes. [B]

```
<SUBJECT>Extension of patent term. (See also Patent term adjustment):</SUBJECT>
<SUBJ1L>Due to examination delay under the URAA (35 U.S.C. 154)</SUBJ1L>
<PT>1.701</PT>
<SUBJECT1>Due to regulatory review period (35 U.S.C. 156):</SUBJECT1>
<SUBJ2L>Applicant for</SUBJ2L>
<PT>1.730</PT>
<SUBJ2L>Application for</SUBJ2L>
<PT>1.740</PT>
<SUBJECT2>Calculation of term:</SUBJECT2>
<SUBJ3L>Animal Drug Product</SUBJ3L>
<PT>1.778</PT>
<SUBJ3L>Food or color additive</SUBJ3L>
<PT>1.776</PT>
```

## 3.107.SUBJL

This has special use in indexes under main division head, with leaders. [B]

```
<SUBJECT>Abandonment of application. (See Abandoned applications)</SUBJECT>
<SUBJL>Abstract of the disclosure.(content, physical requirements)</SUBJL>
<PT>1.72</PT>
<SUBJ1L>Separate sheet required for commencement of</SUBJ1L>
<PT>1.52(b)(4), 1.72(b)</PT>
```

## 3.108.SUBTI

This has special use in title page (page i) and the table of contents. [F, C]

```
<CFRTOC>
  <SUBTI>
    <HED>SUBTITLE B—<E T="04">Regulations Relating to Labor (Continued)</E></HED>
  </SUBTI>
  <PTHD>Part</PTHD>
  <CHAPTI>
    <SUBJECT><E T="04">chapter xvii</E>—Occupational Safety and Health Administration, Department of Labor (Continued)</SUBJECT>
    <PG>1910</PG>
  </CHAPTI>
</CFRTOC>
```

## 3.109.sup

This indicates text that should be rendered as superscript.


```
<DIV9 N="Appendix to" NODE="37:1.0.1.4.15.2.214.15.2" TYPE="APPENDIX">
  <HEAD>Appendix to Part 102—Systems of Records Noticed by Other Federal Agencies
<SU>1</SU> and Applicable to USPTO Records and Applicability of This Part Thereto</HEAD>
  <DIV width="100%">
    <DIV class="gpotbl\_div">
      <TABLE border="1" cellpadding="1" cellspacing="1" class="gpotbl\_table" frame="void" width="100%">
        <TR>
          <TH class="gpotbl\_colhed" scope="col">Category of records</TH>
          <TH class="gpotbl\_colhed" scope="col">Other federal agency</TH>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Federal Personnel Records</TD>
          <TD align="left" class="gpotbl\_cell">Office of Personnel Management.
<sup>2</sup></TD>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Federal Employee Compensation Act Program</TD>
          <TD align="left" class="gpotbl\_cell">Department of Labor.
<sup>3</sup></TD>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Equal Employment Opportunity Appeal Complaints</TD>
          <TD align="left" class="gpotbl\_cell">Equal Employment Opportunity Commission.
<sup>4</sup></TD>
        </TR>
        <TR>
          <TD align="left" class="gpotbl\_cell" scope="row">Formal Complaints/Appeals of Adverse Personnel Actions</TD>
          <TD align="left" class="gpotbl\_cell">Merit Systems Protection Board.
<sup>5</sup></TD>
        </TR>
      </TABLE>
    </DIV>
    <DIV class="table\_foot">
      <P class="gpotbl\_note">
        <sup>1</sup> Other than systems of records noticed by the Department of Commerce. Where the system of records applies only to USPTO, these regulations apply. Where the system of records applies generally to components of the Department of Commerce, the regulations of that department attach at the point of any denial for access or for correction or amendment.
      </P>
      <P class="gpotbl\_note">
        <sup>2</sup> The provisions of this part do not apply to these records covered by notices of systems of records published by the Office of Personnel Management for all agencies. The regulations of OPM alone apply.
      </P>
      <P class="gpotbl\_note">
        <sup>3</sup> The provisions of this part apply only initially to these records covered by notices of systems of records published by the U.S. Department of Labor for all agencies. The regulations of that department attach at the point of any denial for access or for correction or amendment.
      </P>
      <P class="gpotbl\_note">
        <sup>4</sup> The provisions of this part do not apply to these records covered by notices of systems of records published by the Equal Employment Opportunity Commission for all agencies. The regulations of the Commission alone apply.
      </P>
      <P class="gpotbl\_note">
        <sup>5</sup> The provisions of this part do not apply to these records covered by notices of systems of records published by the Merit Systems Protection Board for all agencies. The regulations of the Board alone apply.
      </P>
    </DIV>
  </DIV>
</DIV9>
```

## 3.110.SUPERSED

This is used in effective date notes to mark superseded text. [T]

```
<EFFDNOT>
  <HED>Effective Date Note:</HED>
  <PSPACE>At 44 FR 37467, June 26, 1979, § 202.1(e)(6) (ii) and (vii) were revised. At 44 FR 74817, Dec. 18, 1979, paragraphs (e)(6) (ii) and (vii) were stayed indefinitely. At 64 FR 400, Jan. 5, 1999, these paragraphs were amended. For the convenience of the user, paragraphs (e)(6) (ii) and (vii), published at 44 FR 37467, are set forth below:</PSPACE>
  <SUPERSED>
    <HEAD>§ 202.1   Prescription-drug advertisements.</HEAD><STARS/>
    <P>(e) \* \* \*</P>
    <P>(6) \* \* \*</P>
    <P>(ii) Represents or suggests that a prescription drug is safer
    ...
    </P><STARS/>
    <P>(vii) Suggests, on the basis of favorable data or conclusions 
    ...
    </P><STARS/>
  </SUPERSED>
</EFFDNOT>
```

## 3.111.TABLE

This element contains a table in text (used the same way as `<APPENDIX>`). [T]

```
<TABLE border="1" cellpadding="1" cellspacing="1" class="gpotbl\_table" frame="void" width="100%">
  <TR>
    <TH class="gpotbl\_colhed" scope="col">Category of records</TH>
    <TH class="gpotbl\_colhed" scope="col">Other federal agency</TH>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Personnel Records</TD>
    <TD align="left" class="gpotbl\_cell">Office of Personnel Management.
<sup>2</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Employee Compensation Act Program</TD>
    <TD align="left" class="gpotbl\_cell">Department of Labor.
<sup>3</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Equal Employment Opportunity Appeal Complaints</TD>
    <TD align="left" class="gpotbl\_cell">Equal Employment Opportunity Commission.
<sup>4</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Formal Complaints/Appeals of Adverse Personnel Actions</TD>
    <TD align="left" class="gpotbl\_cell">Merit Systems Protection Board.
<sup>5</sup></TD>
  </TR>
</TABLE>
```

## 3.112.TCAP

This is a top caption line for graphic or mathpac insert. [T]

```
<TCAP><E T="15">windchill chart in non-metric units</E></TCAP>
<img src="http://www.access.gpo.gov/ecfr/graphics/ec01se91.001.gif"/><P/>
<a href="http://www.access.gpo.gov/ecfr/graphics/pdfs/ec01se91.001.pdf">View or download PDF</a>
<P/><P/>
```

## 3.113.TD

This is a Table Data element.  It is a sub-element of `<TR>`.

```
<TABLE border="1" cellpadding="1" cellspacing="1" class="gpotbl\_table" frame="void" width="100%">
  <TR>
    <TH class="gpotbl\_colhed" scope="col">Category of records</TH>
    <TH class="gpotbl\_colhed" scope="col">Other federal agency</TH>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Personnel Records</TD>
    <TD align="left" class="gpotbl\_cell">Office of Personnel Management. <sup>2</sup> </TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Employee Compensation Act Program</TD>
    <TD align="left" class="gpotbl\_cell">Department of Labor. <sup>3</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Equal Employment Opportunity Appeal Complaints</TD>
    <TD align="left" class="gpotbl\_cell">Equal Employment Opportunity Commission.
<sup>4</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Formal Complaints/Appeals of Adverse Personnel Actions</TD>
    <TD align="left" class="gpotbl\_cell">Merit Systems Protection Board. <sup>5</sup> </TD>
  </TR>
</TABLE>
```

## 3.114.TEXT

This is used under `<DIV#>` elements where no `<DIV#>` element follows and other catchall situations. [T, B]


```
<DIV4 N="" NODE="37:1.0.1.2" TYPE="SUBCHAP">
  <HEAD></HEAD>
  <TEXT>
    <HED1>PART 1—RULES OF PRACTICE IN PATENT CASES</HED1>
    <EDNOTE>
      <HED>Editorial Note:</HED>
      <PSPACE>Part 1 is placed in the separate grouping of parts pertaining to patents regulations.</PSPACE>
    </EDNOTE>
  </TEXT>
  <TEXT>
    <HED1>
      <I>TRADEMARKS</I>
    </HED1>
  </TEXT>
```

## 3.115.TEXTCLASS

This element contains information relevant to the text class.  It is never observed to be populated.  It is found inside the `<PROFILEDESC>` element.  See [Section 2.2](#2.2.-Header-Content)

## 3.116.TH

This is a Table Header element.  It is a sub-element of `<TR>`.

```
<TABLE border="1" cellpadding="1" cellspacing="1" class="gpotbl\_table" frame="void" width="100%">
  <TR>
    <TH class="gpotbl\_colhed" scope="col">Category of records</TH>
    <TH class="gpotbl\_colhed" scope="col">Other federal agency</TH>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Personnel Records</TD>
    <TD align="left" class="gpotbl\_cell">Office of Personnel Management.
<sup>2</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Employee Compensation Act Program</TD>
    <TD align="left" class="gpotbl\_cell">Department of Labor.
<sup>3</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Equal Employment Opportunity Appeal Complaints</TD>
    <TD align="left" class="gpotbl\_cell">Equal Employment Opportunity Commission.
<sup>4</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Formal Complaints/Appeals of Adverse Personnel Actions</TD>
    <TD align="left" class="gpotbl\_cell">Merit Systems Protection Board.
<sup>5</sup></TD>
  </TR>
</TABLE>
```

## 3.117.TITLE

This element contains a title (not to be confused with a CFR Title, although it is normally the title of the CFR Title).  It is found within the `<TITLESTMT>`  or  `<SERIESSTMT>` elements.

```
<TITLESTMT>
  <TITLE>Title 37: Patents, Trademarks, and Copyrights</TITLE>
  <AUTHOR TYPE="nameinv"></AUTHOR>
</TITLESTMT>
```

## 3.118.TITLESTMT

This element groups title and author information.  It is normally found within the `<FILEDESC>` and `<BIBLFULL>` elements.

```
<TITLESTMT>
  <TITLE>Title 37: Patents, Trademarks, and Copyrights</TITLE>
  <AUTHOR TYPE="nameinv"></AUTHOR>
</TITLESTMT>
```

## 3.119. TR

This is a Table Row element.  It is a sub-element of `<TABLE>`.


```
<TABLE border="1" cellpadding="1" cellspacing="1" class="gpotbl\_table" frame="void" width="100%">
  <TR>
    <TH class="gpotbl\_colhed" scope="col">Category of records</TH>
    <TH class="gpotbl\_colhed" scope="col">Other federal agency</TH>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Personnel Records</TD>
    <TD align="left" class="gpotbl\_cell">Office of Personnel Management.
<sup>2</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Federal Employee Compensation Act Program</TD>
    <TD align="left" class="gpotbl\_cell">Department of Labor.
<sup>3</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Equal Employment Opportunity Appeal Complaints</TD>
    <TD align="left" class="gpotbl\_cell">Equal Employment Opportunity Commission.
<sup>4</sup></TD>
  </TR>
  <TR>
    <TD align="left" class="gpotbl\_cell" scope="row">Formal Complaints/Appeals of Adverse Personnel Actions</TD>
    <TD align="left" class="gpotbl\_cell">Merit Systems Protection Board.
<sup>5</sup></TD>
  </TR>
</TABLE>
```

## 3.120.XREF

This element is used to create cross references. It has both an identifier and a reference identifier.

```
<DIV8 N="§ 1.36" NODE="37:1.0.1.1.1.2.69.5" TYPE="SECTION">
  <HEAD>§ 1.36   Revocation of power of attorney; withdrawal of patent attorney or agent.</HEAD>
  <XREF ID="20140307" REFID="4">Link to an amendment published at 79 FR 12944, March 7, 2014.</XREF>
```


# 4.Resources Directory

The resources directory in the Electronic CFR Bulk Data Repository is found at [http://www.gpo.gov/fdsys/bulkdata/ECFR/resources](http://www.gpo.gov/fdsys/bulkdata/ECFR/resources) and contains the current version of this user guide.

