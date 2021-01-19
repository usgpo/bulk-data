U.S. Government Publishing Office Federal Digital System (FDsys) User Guide Document
================================================================================



## Bill Summaries XML Bulk Data

Prepared by: Programs, Strategy, and Technology

U.S. Government Publishing Office

January 2015


## Revision

- 1.0 January 2014 Version 1.0
  House Bill Summaries
- 2.0 January 2015 Version 2.0
  House and Senate Bill Summaries


## 1. Introduction

At the direction of the Appropriations Committee within the United States House of
Representatives, in support of the Legislative Branch Bulk Data Task Force, the Government
Publishing Office (GPO), the Library of Congress (LOC), the Clerk of the House, and the Secretary
of the Senate are making Bill Summaries in XML format available through the GPO’s Federal
Digital System (FDsys) Bulk Data repository starting with the 113th Congress. The FDsys Bulk
Data repository for Bill Summaries is available at
<http://www.gpo.gov/fdsys/bulkdata/BILLSUM>.


### 1.1 Types of Bill Summaries

Bill summaries are summaries of bills or resolutions, as well as other document types associated
with the legislative history of a measure such as amendments, committee reports, conference
reports, or public laws (enacted bills or joint resolutions). A bill summary describes the most
significant provisions of a piece of legislation and details the effects the legislative text may have on
current law and Federal programs. Bill summaries are written as a result of a Congressional action
and may not always map to a printed bill version. Bill summaries are authored by the Congressional
Research Service (CRS) of the Library of Congress. As stated in Public Law 91-510 (2 USC 166
(d)(6)), one of the duties of CRS is "to prepare summaries and digests of bills and resolutions of a
public general nature introduced in the Senate or House of Representatives.”


#### Bills

- House Bill (HR)
- Senate Bill (S)

A bill is a legislative proposal before Congress. Bills from each house are assigned a number in
the order in which they are introduced, starting at the beginning of each Congress (first and
second sessions). Public bills pertain to matters that affect the general public or classes of
citizens, while private bills pertain to individual matters that affect individuals and organizations,
such as claims against the Government.


#### Joint Resolutions

 - House Joint Resolution (HJRES)
 - Senate Joint Resolution (SJRES)

A joint resolution is a legislative proposal that requires the approval of both houses and the
signature of the President, just as a bill does. Resolutions from each house are assigned a number
in the order in which they are introduced, starting at the beginning of each Congress (first and
second sessions). There is no real difference between a bill and a joint resolution. Joint
resolutions generally are used for limited matters, such as a single appropriation for a specific
purpose. They are also used to propose amendments to the Constitution.
1A joint resolution has the force of law, if approved. Joint resolutions become a part of the
Constitution when three-quarters of the states have ratified them; they do not require the
President's signature.


#### Concurrent Resolutions

- House Concurrent Resolution (HCONRES)
- Senate Concurrent Resolution (SCONRES)

A concurrent resolution is a legislative proposal that requires the approval of both houses but
does not require the signature of the President and does not have the force of law. Concurrent
resolutions generally are used to make or amend rules that apply to both houses. They are also
used to express the sentiments of both of the houses. For example, a concurrent resolution is used
to set the time of Congress' adjournment. It may also be used by Congress to convey
congratulations to another country on the anniversary of its independence.


#### Simple Resolutions

- House Simple Resolution (HRES)
- Senate Simple Resolution (SRES)

A simple resolution is a legislative proposal that addresses matters entirely within the prerogative
of one house or the other. It requires neither the approval of the other house nor the signature of
the President, and it does not have the force of law. Most simple resolutions concern the rules of
one house. They are also used to express the sentiments of a single house. For example, a simple
resolution may offer condolences to the family of a deceased member of Congress, or it may
express the sense of the Senate or House on foreign policy or other executive business.

Additional information about bill types can be found at
<http://www.gpo.gov/help/index.html#about_congressional_bills.htm>.


### 1.2 Scope of Bulk Data

The Bill Summaries bulk data collection on FDsys includes XML bills summaries from the 113 th
Congress forward.


### 1.3 Bulk Data Downloads

The Bulk Data repository is organized by Congress and bill type. A ZIP file is available for each
bill type and contains Bill Summaries XML files for that bill type within a specific Congress.
Each Bill Summaries XML file contains summaries of legislation under consideration for a
specific measure.


## 2. XML Descriptions

The following conventions are used in this document:

- XML element names are denoted with angled brackets and in courier. For example,
  `<title>` is an XML element.
- XML attribute names are denoted with a “@” prefix and in courier. For example, @href
  is an XML attribute.
 

### 2.1 Elements

- `<BillSummaries>` 

  Root element. 

- `<item>` 

  Parent container for a single legislative measure.
- `<title>` 

  The latest title for the measure.  It may be the official title or the short 
  title. It is contained within `<item>`. 

- `<summary>` 

  Parent container for a single summary.  It may appear one or more times in 
  the file. It is contained within `<item>`. 

- `<action-date>` 

  The date on which a particular action occurred. The format is YYYY‐MM‐DD. It 
  is contained within `<summary>`. 

- `<action-desc>` 

  The description of the action that took place to prompt the bill summary to 
  be written. It is contained within `<summary>`. This value is added by CRS.
 
  See Section 3 of this document for a list of possible values. 

- `<summary-text>` 

  This is the text of the summary written by the Congressional Research Service
  of the Library of Congress. It is contained within `<summary>`. Values are 
  enclosed in a CDATA tag and contain HTML elements.


### 2.2 Attributes

- `@congress` 

  The number of the Congress. This is an attribute of `<item>`. 

- `@measure-type`

  The type of measure. This is an attribute of `<item>`. The measure type 
  abbreviations that can be found in bill summaries are hr, hjres, hconres, 
  hres, s, sconres, sres, and sjres.
 
  See Section 1.1 of this document for a description of each measure type. 

- `@measure-number` 

  The number associated with the measure. This is commonly referred to as the 
  bill number. This is an attribute of `<item>`. 

- `@measure-id` 

  An ID assigned to the measure. This is an attribute of `<item>`.
 
  Convention: “id” + Congress number + measure type abbreviation + measure 
  number

  Example: id113hr910 
 
  The measure type abbreviations that can be found in bill summaries are 
  hr, hjres, hconres, hres, s, sconres, sres, and sjres.
 
  See Section 1.1 of this document for a description of each measure type. 

- `@originChamber` 

  The chamber in which the measure originated. This is an attribute of 
  `<item>`. Value will be HOUSE or SENATE.

- `@orig-publish-date` 

  The first date in which the bill summary file was published. The format is 
  YYYY‐MM‐DD. This is an attribute of `<item>`. 

- `@update-date` 

  The date in which the material in the container element was last updated. The
  format is YYYY‐MM‐DD. This is an attribute of `<item>` and `<summary>`. 

- `@summary-id` 

  An ID assigned to the individual summary. This is an attribute of `<summary>`. 
 
  Convention:  “id” + Congress number + measure type abbreviation + measure 
  cumber + the letter “v” for version + LOC action code for summaries 

  Example: id113hr910v28 
 
  The measure type abbreviations that can be found in bill summaries are hr, 
  hjres, hconres, hres, s, sconres, sres, and sjres. 
 
  See Section 3 of this document for a list of LOC action codes for summaries. 

- `@currentChamber`

  The chamber in which the action described in the `<action-desc>` element 
  occurred. This is an attribute of `<summary>`. Value will be HOUSE, SENATE, 
  or BOTH. 


### 2.3. Sample Bill Summaries XML File

```
<BillSummaries>
<item congress="113" measure-type="hr" measure-number="910" measure-
id="id113hr910" originChamber="HOUSE" orig-publish-date="2013-02-28"
update-date="2013-09-03">
<title>Sikes Act Reauthorization Act of 2013</title>
<summary summary-id="id113hr910v28" currentChamber="HOUSE" update-
date="2013-09-03">
<action-date>2013-06-24</action-date>
<action-desc>Reported to House without amendment, Part I</action-desc>
<summary-text><![CDATA[ <p><b>Sikes Act Reauthorization Act of 2013 - Reauthorizes title I
of the Sikes Act (conservation programs on military installations) for FY2015-
FY2019.</b></p>]]></summary-text>
</summary>
<summary summary-id="id113hr910v00" currentChamber="HOUSE" update-
date="2013-02-28">
<action-date>2013-02-28</action-date>
<action-desc>Introduced in House</action-desc>
<summary-text><![CDATA[<p><b>(This measure has not been amended since it was introduced.
The summary of that version is repeated here.)</b></p> <p>Sikes Act Reauthorization Act of 2013 -
Reauthorizes title I of the Sikes Act (conservation programs on military installations) for FY2015-
FY2019.</p>]]></summary-text>
</summary>
</item>
<dublinCore xmlns:dc=”http://purl.org/dc/elements/1.1/”>
<dc:format>text/xml</dc:format>
<dc:language>EN</dc:language>
<dc:rights>Pursuant to Title 17 Section 105 of the United States Code, this file is not subject to
copyright protection and is in the public domain.</dc:rights>
<dc:contributor>Congressional Research Service, Library of Congress</dc:contributor>
<dc:description>This file contains bill summaries for federal legislation. A bill summary describes
the most significant provisions of a piece of legislation and details the effects the legislative text may
have on current law and federal programs. Bill summaries are authored by the Congressional Research
Service (CRS) of the Library of Congress. As stated in Public Law 91-510 (2 USC 166 (d)(6)), one of the
duties of CRS is "to prepare summaries and digests of bills and resolutions of a public general nature
introduced in the Senate or House of Representatives". For more information, refer to the User Guide that
accompanies this file.</dc:description>
</dublinCore>
</BillSummaries>
```


## 3. Mapping of LOC Action Codes, Action Description Text, and Version Codes

LOC Action Code for Summaries| Chamber | Text in the `<action‐desc>` Element                             | LOC Version Code
-----------------------------|---------|-----------------------------------------------------------------|-----------------
00                           | HOUSE   | Introduced in House                                             | IH
00                           | SENATE  | Introduced in Senate                                            | IS
01                           | SENATE  | Reported to Senate amended                                      | RS
02                           | SENATE  | Reported to Senate amended, 1st committee reporting             | RS
03                           | SENATE  | Reported to Senate amended, 2nd committee reporting             | RS
04                           | SENATE  | Reported to Senate amended, 3rd committee reporting             | RS
05                           | SENATE  | Reported to Senate amended, 4th committee reporting             | RS
06                           | SENATE  | Reported to Senate amended, 5th committee reporting             | RS
07                           | SENATE  | Reported to Senate amended, 6th committee reporting             | RS
08                           | SENATE  | Reported to Senate amended, 7th committee reporting             | RS
09                           | SENATE  | Reported to Senate amended, 8th committee reporting             | RS
10                           | SENATE  | Reported to Senate amended, 9th committee reporting             | RS
11                           | SENATE  | Reported to Senate amended, 10th committee reporting            | RS
12                           | SENATE  | Reported to Senate without amendment, 1st committee reporting   | RS
13                           | SENATE  | Reported to Senate without amendment, 2nd committee reporting   | RS
14                           | SENATE  | Reported to Senate without amendment, 3rd committee reporting   | RS
15                           | SENATE  | Reported to Senate without amendment, 4th committee reporting   | RS
16                           | SENATE  | Reported to Senate without amendment, 5th committee reporting   | RS
17                           | HOUSE   | Reported to House amended                                       | RH
18                           | HOUSE   | Reported to House amended, Part I                               | RH
19                           | HOUSE   | Reported to House amended, Part II                              | RH
20                           | HOUSE   | Reported to House amended, Part III                             | RH
21                           | HOUSE   | Reported to House amended, Part IV                              | RH
22                           | HOUSE   | Reported to House amended, Part V                               | RH
23                           | HOUSE   | Reported to House amended, Part VI                              | RH
24                           | HOUSE   | Reported to House amended, Part VII                             | RH
25                           | HOUSE   | Reported to House amended, Part VIII                            | RH
26                           | HOUSE   | Reported to House amended, Part IX                              | RH
27                           | HOUSE   | Reported to House amended, Part X                               | RH
28                           | HOUSE   | Reported to House without amendment, Part I                     | RH
29                           | HOUSE   | Reported to House without amendment, Part II                    | RH
30                           | HOUSE   | Reported to House without amendment, Part III                   | RH
31                           | HOUSE   | Reported to House without amendment, Part IV                    | RH
32                           | HOUSE   | Reported to House without amendment, Part V                     | RH
33                           | HOUSE   | Laid on table in House                                          | LTH
34                           | SENATE  | Indefinitely postponed in Senate                                | IPS
35                           | SENATE  | Passed Senate amended                                           | ES
36                           | HOUSE   | Passed House amended                                            | EH
37                           | SENATE  | Failed of passage in Senate                                     | FPS
38                           | HOUSE   | Failed of passage in House                                      | FPH
39                           | HOUSE   | Senate agreed to House amendment with amendment                 | ATS
40                           | SENATE  | House agreed to Senate amendment with amendment                 | ATH
41                           | HOUSE   | Senate disagreed to House amendment with amendment              | NAT
42                           | SENATE  | House disagreed to Senate amendment with amendment              | NAT
43                           | HOUSE   | Senate disagreed to House amendment                             | NAT
44                           | SENATE  | House disagreed to Senate amendment                             | NAT
45                           | SENATE  | Senate receded and concurred with amendment                     | AES
46                           | HOUSE   | House receded and concurred with amendment                      | EAH
47                           | SENATE  | Conference report filed in Senate                               | CONF-S
48                           | HOUSE   | Conference report filed in House                                | CONF-H
49                           | BOTH    | Public Law                                                      | LAW
50                           | BOTH    | Private Law                                                     | LAW
51                           | BOTH    | Line item veto by President                                     | LINEITEMVETO
52                           | SENATE  | Passed Senate amended, 2nd occurrence                           | ES
53                           | SENATE  | Passed Senate amended, 3rd occurrence                           | ES
54                           | HOUSE   | Passed House amended, 2nd occurrence                            | EH
55                           | HOUSE   | Passed House amended, 3rd occurrence                            | EH
56                           | SENATE  | Senate vitiated passage of bill after amendment                 | PAV
57                           | HOUSE   | House vitiated passage of bill after amendment                  | PAV
58                           | SENATE  | Motion to recommit bill as amended in Senate                    | MOTION_R-S
59                           | HOUSE   | Motion to recommit bill as amended in House                     | MOTION_R-H
60                           | SENATE  | Senate agreed to House amendment with amendment, 2nd occurrence | ATS
61                           | SENATE  | Senate agreed to House amendment with amendment, 3rd occurrence | ATS
62                           | HOUSE   | House agreed to Senate amendment with amendment, 2nd occurrence | ATH
63                           | HOUSE   | House agreed to Senate amendment with amendment, 3rd occurrence | ATH
64                           | SENATE  | Senate receded and concurred with amendment, 2nd occurrence     | AES
65                           | SENATE  | Senate receded and concurred with amendment, 3rd occurrence     | AES
66                           | HOUSE   | House receded and concurred with amendment, 2nd occurrence      | EAH
67                           | HOUSE   | House receded and concurred with amendment, 3rd occurrence      | EAH
70                           | HOUSE   | Hearing scheduled in House                                      | HRG-SCD-H
71                           | SENATE  | Hearing scheduled in Senate                                     | HRG-SCD-S
72                           | HOUSE   | Hearing held in House                                           | HRG-H
73                           | SENATE  | Hearing held in Senate                                          | HRG-S
74                           | HOUSE   | Markup in House                                                 | MKUP-H
75                           | SENATE  | Markup in Senate                                                | MKUP-S
76                           | HOUSE   | Rule reported to House                                          | RULE-H
77                           | HOUSE   | Discharged from House committee                                 | CDH
78                           | SENATE  | Discharged from Senate committee                                | CDS
79                           | HOUSE   | Reported to House, without amendment                            | RH
80                           | SENATE  | Reported to Senate without amendment                            | RS
81                           | HOUSE   | Passed House, without amendment                                 | EH
82                           | SENATE  | Passed Senate, without amendment                                | ES
83                           | SENATE  | Conference report filed in Senate, 2nd conference report        | CONF-S
84                           | SENATE  | Conference report filed in Senate, 3rd conference report        | CONF-S
85                           | SENATE  | Conference report filed in Senate, 4th conference report        | CONF-S
86                           | HOUSE   | Conference report filed in House, 2nd conference report         | CONF-H
87                           | HOUSE   | Conference report filed in House, 3rd conference report         | CONF-H
88                           | HOUSE   | Conference report filed in House, 4th conference report         | CONF-H


## 4. Data Set

Bill Summaries data is provided to GPO by the Library of Congress, and XML files are available
for bulk data download on the FDsys Bulk Data repository starting with the 113th Congress
(2013-2014). Bill Summaries XML files are not available through FDsys search or browse; they
are only available in the FDsys Bulk Data repository.

In general, there are no restrictions on re-use of information in the Bill Summaries data set
because U.S. Government works are not subject to copyright protection and are in the public
domain. GPO and its legislative branch data partners do not restrict downstream uses of Bill
Summaries data, except that independent providers should be aware that only GPO and its
legislative branch data partners are entitled to represent that they are the providers of official Bill
Summaries data.

Bill Summaries XML files can be manipulated and enriched to operate in the various
applications that users may devise. GPO and its legislative branch data partners cannot vouch for
the authenticity of data that is not under GPO’s control. GPO is providing free access to Bill
Summaries XML files for display in various applications and mash-ups outside the FDsys
domain. GPO does not endorse third party applications, and does not evaluate how the original
legal content is displayed on other sites. Consumers should form their own conclusions as to
whether the downloaded data can be relied upon within an application or mash-up.


## 5. Resources Directory

The resources directory at <http://www.gpo.gov/fdsys/bulkdata/BILLSUM/resources> 
contains the *User Guide for Bill Summaries XML Bulk Data* in PDF form.
