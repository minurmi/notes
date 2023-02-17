# IEC 62304 - Medical Device software - Sofware Life-cycle Processes

# Intro

Three terms identify the software decomposition. The top level is the SOFTWARE SYSTEM. The lowest level that is not further decomposed is the SOFTWARE UNIT. All levels of composition, including the top and bottom levels, can be called SOFTWARE ITEMS. A SOFTWARE SYSTEM, then, is composed of one or more SOFTWARE ITEMS, and each SOFTWARE ITEM is composed of one or more SOFTWARE UNITS or decomposable SOFTWARE ITEMS. The responsibility is left to the MANUFACTURER to provide the granularity of the SOFTWARE ITEMS and SOFTWARE UNITS.

## Table of contents

<!-- MarkdownTOC -->

- [5.3 Software ARCHITECTURAL design](#53-software-architectural-design)
    - [5.3.2 Develop an ARCHITECTURE for the interfaces of SOFTWARE ITEMS](#532-develop-an-architecture-for-the-interfaces-of-software-items)
    - [5.3.3 Specify functional and performance requirements of SOUP item](#533-specify-functional-and-performance-requirements-of-soup-item)
- [5.4 Software detailed design](#54-software-detailed-design)
    - [5.4.1 Subdivide software into SOFTWARE UNITS](#541-subdivide-software-into-software-units)
- [5.5 SOFTWARE UNIT implementation](#55-software-unit-implementation)
    - [5.5.3 SOFTWARE UNIT acceptance criteria](#553-software-unit-acceptance-criteria)
    - [5.5.4 Additional SOFTWARE UNIT acceptance criteria](#554-additional-software-unit-acceptance-criteria)
    - [5.5.5 SOFTWARE UNIT VERIFICATION](#555-software-unit-verification)
- [5.6 Software integration and integration testing](#56-software-integration-and-integration-testing)
    - [5.6.4 Software integration testing content](#564-software-integration-testing-content)
    - [5.6.5 EVALUATE software integration test procedures](#565-evaluate-software-integration-test-procedures)
    - [5.6.6 Conduct regression tests](#566-conduct-regression-tests)
    - [5.6.7 Integration test record contents](#567-integration-test-record-contents)
- [Steps for algorithm](#steps-for-algorithm)
- [Detail process for algorithm performance verification](#detail-process-for-algorithm-performance-verification)
- [Algorithm unit code verification](#algorithm-unit-code-verification)
- [Algorithm item integration](#algorithm-item-integration)

<!-- /MarkdownTOC -->

# 5.3 Software ARCHITECTURAL design

This ACTIVITY requires the MANUFACTURER to define the major structural components of the software and identify their key responsibilities, their externally visible properties and the relationship among them.

## 5.3.2 Develop an ARCHITECTURE for the interfaces of SOFTWARE ITEMS

>The MANUFACTURER shall develop and document an ARCHITECTURE for the interfaces between the SOFTWARE ITEMS and the components external to the SOFTWARE ITEMS (both software and hardware), and between the SOFTWARE ITEMS. [Class B, C]

## 5.3.3 Specify functional and performance requirements of SOUP item

>If a SOFTWARE ITEM is identified as SOUP, the MANUFACTURER shall specify functional and performance requirements for the SOUP item that are necessary for its intended use. [Class B, C]

# 5.4 Software detailed design

This ACTIVITY requires the MANUFACTURER to refine the SOFTWARE ITEMS and interfaces defined in the ARCHITECTURE to create SOFTWARE UNITS and their interfaces. Detailed design specifies algorithms, data representations, interfaces among different SOFTWARE UNITS, and interfaces between SOFTWARE UNITS and data structures.

When present in the design, the MANUFACTURER should verify design characteristics which the MANUFACTURER believes are important for SAFETY. Examples of these characteristics include:
- implementation of the intended events, inputs, outputs, interfaces, logic flow, allocation of CPU, allocation of memory resources, error and exception definition, error and exception isolation, and error recovery;
- definition of the default state, in which all faults that can result in a hazardous situation are addressed, with events and transitions;
- initialization of variables, memory management; and
- cold and warm resets, standby, and other state changes that can affect the RISK CONTROL measures.

## 5.4.1 Subdivide software into SOFTWARE UNITS

>The MANUFACTURER shall subdvide the software until it is represented by SOFTWARE UNITS. [Class B, C]

*NOTE* Some SOFTWARE SYSTEMS are not divided further.

# 5.5 SOFTWARE UNIT implementation

This ACTIVITY requires the MANUFACTURER to write and verify the code for the SOFTWARE UNITS.

## 5.5.3 SOFTWARE UNIT acceptance criteria

>The MANUFACTURER shall establish acceptance criteria for SOFTWARE UNITS prior to integration into larger SOFTWARE ITEMS as appropriate, and ensure that SOFTWARE UNITS meet acceptance criteria. [Class B, C]

*NOTE* Examples of acceptance criteria are:
- does the software code implement requirements including RISK CONTROL measures?
- is the software code free from contradiction with the interface design of the SOFTWARE UNIT?
- does the software code conform to programming procedures or coding standards?

## 5.5.4 Additional SOFTWARE UNIT acceptance criteria

>When present in the design, the MANUFACTURER shall include additional acceptance criteria as appropriate for:
>- a) proper event sequence;
>- b) data and control flow;
>- c) planned resource allocation;
>- d) fault handling (error definition, isolation, and recovery);
>- e) initialisation of variables;
>- f) self-diagnostics;
>- g) memory management and memory overflows; and
>- h) boundary conditions.
>[Class C]

## 5.5.5 SOFTWARE UNIT VERIFICATION

>The MANUFACTURER shall perform the SOFTWARE UNIT VERIFICATION and document the results. [Class B, C]

# 5.6 Software integration and integration testing

Software integration testing focuses on the transfer of data and control across a SOFTWARE ITEM’s internal and external interfaces. External interfaces are those with other software, including operating system software, and MEDICAL DEVICE hardware.

The rigor of integration testing and the level of detail of the documentation associated with integration testing should be commensurate with the RISK associated with the device, the device’s dependence on software for potentially hazardous functions, and the role of specific SOFTWARE ITEMS in higher RISK device functions. For example, although all SOFTWARE ITEMS should be tested, items that have an effect on SAFETY should be subject to more direct, thorough, and detailed tests.

As applicable, integration testing demonstrates program behaviour at the boundaries of its input and output domains and confirms program responses to invalid, unexpected, and special inputs. The program’s actions are revealed when given combinations of inputs or unexpected sequences of inputs, or when defined timing requirements are violated. The test requirements in the plan should include, as appropriate, the types of white box testing to be performed as part of integration testing.

White box testing, also known as glass box, structural, clear box and open box testing, is a testing technique where explicit knowledge of the internal workings of the SOFTWARE ITEM being tested are used to select the test data. White box testing uses specific knowledge of the SOFTWARE ITEM to examine outputs. The test is accurate only if the tester knows what the SOFTWARE ITEM is supposed to do. The tester can then see if the SOFTWARE ITEM diverges from its intended goal. White box testing cannot guarantee that the complete specification has been implemented since it is focused on testing the implementation of the SOFTWARE ITEM.

Black box testing, also known as behavioural, functional, opaque-box, and closed-box testing, is focused on testing the functional specification and it cannot guarantee that all parts of the implementation have been tested. Thus black box testing is testing against the specification and will discover faults of omission, indicating that part of the specification has not been fulfilled. White box testing is testing against the implementation and will discover faults of commission, indicating that part of the implementation is faulty. In order to fully test a SOFTWARE PRODUCT both black and white box testing might be required.

Software integration testing can be performed in a simulated environment, on actual target hardware, or on the full MEDICAL DEVICE.

## 5.6.4 Software integration testing content

>For software integration testing, the MANUFACTURER shall address whether the integrated SOFTWARE ITEM performs as intended. [Class B, C]

*NOTE* 1 Examples to be considered are:
- the required functionality of the software;
- implementation of RISK CONTROL measures;
- specified timing and other behaviour;
- specified functioning of internal and external interfaces; and
- testing under abnormal conditions including foreseeable misuse.


*NOTE* 2 It is acceptable to combine integration testing and SOFTWARE SYSTEM testing into a single plan and set of ACTIVITIES.

## 5.6.5 EVALUATE software integration test procedures

>The MANUFACTURER shall EVALUATE the integration test procedures for adequacy. [Class B, C]

## 5.6.6 Conduct regression tests

>When software items are integrated, the MANUFACTURER shall conduct REGRESSION TESTING appropriate to demonstrate that defects have not been introduced into previously integrated software. [Class B, C]

## 5.6.7 Integration test record contents

> The MANUFACTURER shall:
> - a) document the test result (pass/fail and a list of ANOMALIES);
> - b) retain sufficient records to permit the test to be repeated; and
> - c) identify the tester.
> [Class B, C]

*NOTE* Requirement b) could be implemented by retaining, for example:
- test case specifications showing required actions and expected results;
- records of the equipment;
- records of the test environment (including software tools) used for test.






# Steps for algorithm
- Identify SOUP items
- Specify functional and performance requirements for the SOUP item that are necessary for its intended use
- Create architecture description and identify SOFTWARE ITEMS
- Document interfaces of SOFTWARE ITEMS

# Detail process for algorithm performance verification
1. Perform study
    - Study descriptions
    - Algorithm verification and validation document
2. Acquire measurement data
    - How was the data delivered to us from all devices
3. Get annotations for MDT
    - Qualify supplier
4. Process data to correct format and sync
    - Describe steps
    - Verify scripts
5. Run scripts for each dataset
    - Describe steps
    - Verify scripts
    - Verify offline algorithm
6. Compile results to a report

# Algorithm unit code verification
1. Create acceptance criteria for units
2. Show that the criteria is met

# Algorithm item integration
1. Demonstrates program behaviour at the boundaries of its input and output domains and confirms program responses to invalid, unexpected, and special inputs.



















