# SW process

## Adopting_Agile_in_an_FDA_Regulated_Environment.pdf

### Agile process

In January of 2004, the m2000 software team put agile into practice. The process as initially defined by the team included the following practices:
    - Fixed and short duration iterations (4 to 10 weeks) delivering functional software.
    - Automated continuous build, unit test, and integration
    - Daily team meeting providing high visibility of status and promoting concept of collective ownership
    - Retrospective assessment at conclusion of each iteration by key stakeholders

The software development process as defined by the m2000 core team emphasized the concept of time- boxing. The overall project from inception to commercial launch was subdivided into increments.

Each increment resulted in delivery of executable software that was intended for distribution to one or more stakeholders outside of the software organization. Development of an increment consisted of completing one or more software iterations followed by a verification and validation phase. Each iteration delivered functional software. Additionally, an iteration generated key artifacts demonstrating compliance with design control processes imposed by various regulatory agencies. The verification and validation phase included formal execution of functional testing, formalized design reviews, approval of artifacts supporting the design control process, and update of the project’s design history file.

Other process modifications identified during retrospective stakeholder reviews and adopted over time included addition of weekly goals and a shift from scenario based planning to feature based planning.
Weekly goals were established for each week of a given iteration. These higher level objectives were reviewed at the end of each week during the daily meeting and provided additional focus on team objectives.

### Testing 

The updated practice focused the test case author on the intent of the test case. The detailed set of actions required to navigate the UI and complete a specific software function were replaced by a single bullet point or step in the test case. Although the resulting process required test cases to be executed by subject matter experts, the benefits were considerable:
    - Test case development was more efficient.
Authors were focused on the intent of the test case, not meticulously describing step-by-step process of running the application. The less prescriptive test cases were easier to understand and debug.
    - First pass acceptance of executed test cases by the auditing function increased reducing rework or reruns.
    - Alternate execution paths were much more likely to be exercised each time a test case was executed increasing code coverage.
    - Test cases were in many cases immune to UI centric application changes.

### Frequent integration

Additionally, frequent integration between software and hardware elements provided early identification of issues to the hardware team.


# FAQ_62304_Final_130804.pdf

### 2.3.11 What are the artifacts required by EN 62304?

The standard requires following documents:
    - Risk Management File (clause 4.2, 7)
    - Software Safety Classification (clause 4.3.c)
    - Software Development Plan (clause 5.1.1)
    - Software System requirements (5.2), including risk control measures (clause 5.2.3)
    - Software Architectural Design (clauses 5.3, 5.4)
    - Software Test Plan (clauses 5.5, 5.6, 5.7, especially 5.7.1 NOTE 1 and 2)
    - Traceability Overview (of test procedures to software requirements) (clause 5.7.4)
    - Software Test Report (clause 5.7.5)
    - Residual Anomalies (clause 5.8)
    - Configuration Management (clauses 5.8.4, 5.8.5, 8)

### 2.5.1 What is segregation?

Segregation is a way to ensure that software items do not influence each other in an unintended way.
Segregation means setting apart or separating things. Segregation is intended to avoid side- effects resulting from dependencies of control flow, data flow and shared resources.

It works on three different levels: functional, logical and physical.
    - Functional segregation can for example be established via middle ware or 'wrappers'. They prevent the use of SOUP (see chapter 2.7 of this FAQ) features you do not want your system to use.
    - Physical segregation can involve separate processors.
    - Logical segregation can involve separate memory allocation.
The type of segregation needed depends on the elements of your system that may pose a critical failure state.

Segregation aims to avoid unintended side-effects between software items from dependencies of control flow, data flow and shared resources. Your proof of segregation is effective by demonstrating that there are no significant side effects.

Common approach:
    1. Design and construction measures establish segregation
    2. Perform safety analytic techniques, like FTA (Fault tree analysis) and FMEA (Failure
    Mode and Effect Analysis).
    3. Verification will prove that segregation is effective.

Specify segregation so verification can demonstrate that (under foreseeable operation conditions) the verification segregation is effective. Consider specifying the following:
    - Data flow corruption is prevented: non-safety related software items cannot modify safety- related data
    - Control flow corruption is prevented: safety-related functions can always execute at the correct time, without being effected by the actions of the non-safety-related software items
    - Non-safety-related software items cannot modify the safety-related software items
    - Corruption of the execution environment is prevented: corruption of parts of the software system used by both safety-related and non-safety-related software items (e.g. processor registers, device registers and memory access privileges) cannot occur.”

### 2.5.4 How does the severity under the intended use relate to the software safety class?

If a chain of events can lead to serious injury, then the software is class C. If it cannot lead to serious injury (used in accordance with its intended use) then it is class B. If no injury can result, the safety class will be A.


### 2.5.7 Does a class B software generated by a compiler imply class B also to the compiler?

Tools need not be safety classified but must be validated (see ISO 13485 clause 7.5.2.1).
It has to be noted that re-distributable components of a compiler (e.g. runtime libraries) are SOUP of the MEDICAL DEVICE.

### 2.6.5 Requirements and Design Input

EN 62304 does not prescribe a certain granularity of requirements or software units. Requirements should be testable by criteria which produce "accepted" or "not accepted" results.

### 2.6.9 Unit detailed desing vs verification

According to 5.4.2, for Class B Software Units: Documented SDD are not required for all Units
    - 5.4.1 Refine SOFTWARE ARCHITECTURE into SOFTWARE UNITS
        + The MANUFACTURER shall refine the software ARCHITECTURE until it is represented by SOFTWARE UNITS. [Class B, C]
    - 5.4.2 Develop detailed design for each SOFTWARE UNIT
        + The MANUFACTURER shall develop and document a detailed design for each SOFTWARE UNIT of the SOFTWARE ITEM. [Class C]
However, § 5.5.5 states:
    - 5.5.5 SOFTWARE UNIT VERIFICATION
        + The MANUFACTURER shall perform the SOFTWARE UNIT VERIFICATION and document the results.[Class B, C]

Absence of documentation does not mean it does not exist. The detailed design specification is in the minds of the developers and testers. For class B items that is considered sufficient for a unit test. Testing against an undocumented specification implies that you would not report on the detailed steps performed during the unit test, but that you would merely list the software item and conclude with a pass or fail. 

### 2.6.10 Open source SOUP

The standard also applies to open source code. If you take the code it follows the requirements of a SOUP. If you make changes to the code, then you must consider it as a software item that you developed yourself. The level of control depends on the safety class of the code.


### Software configuration management

A configuration management must exist (versioning and reproduction of build environment and SOUP).

### Annex2 SOUP selection, assessment & qualification

The 'SOUP' flowchart (see Annex 2 Figure 2) provides an example of a process for the selection, assessment and qualification of SOUP suppliers. After searching (2) and identifying (3) a potential SOUP supplier that meets the specifications (4) you will designate the supplier as 'certified supplier'. The selection criteria may require a review if the supplier obtains the label 'critical'.

To determine whether the supplier is critical you must consider the potential impact of the SOUP on the safety (10) and efficacy (11) of your product. If the SOUP is intended for use as stand-alone software, i.e. as a product integrated into a system, you also need to determine who will take the manufacturer responsibility for the SOUP product (12). When answering these questions you should consider the changes you intend to make to the SOUP including any additional claims you may want to make with regards to the SOUP. Note that some companies may have additional criteria that could qualify a supplier as critical.

(10) If the SOUP has safety class B or C, then your supplier is automatically 'critical'.

(11) If you find that you do not have the capability to test yourself for the impact of the SOUP on your product's efficacy, then your supplier is 'critical'. E.g. an algorithm for the detection of clinical anomalies may involve costly or difficult clinical evaluations for which you want to rely on the evidence supplied by the manufacturer; similarly when you want to make changes to the SOUP or want to make new claims for which you rely on the supplier to provide the clinical evaluation.

(12) When you take manufacturer responsibility or act as authorized representative for a SOUP, also then your supplier is 'critical'.

If a supplier is designated as 'critical' you must perform an audit of the supplier. This can be an onsite audit or via a self-assessment questionnaire. Using your audit criteria you determine if a critical supplier can still be certified. You may, for example, accept the supplier if it has an established quality system (e.g. ISO 13485) or if it designs and tests its product according to your criteria. If the supplier does not meet your audit-criteria then the SOUP cannot be used. Note that audit criteria can be made dependent on the outcome of question 10 and 11. You may, for example, apply more stringent audit criteria if you rely on the manufacturer to test the effectiveness of the system, or you may request more stringent testing standards based on the safety impact of the SOUP.










