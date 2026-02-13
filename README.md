# SAP-Application-Programming_Report
These projects showcase end-to-end development in **SAP ABAP**, covering Data Dictionary design, database modeling, modular report programming, and object-oriented architecture.

The first project focuses on backend data modeling and interactive reporting in SAP ERP .
Custom **Domains** and **Data Elements** were created in the ABAP Data Dictionary (SE11) to define reusable technical and semantic attributes. Two relational database tables, **Z018_PRODUCT** and **Z018_CUSTOMERS**, were designed with proper primary keys, foreign key relationships, currency/quantity references, technical settings (APPL0), and enhancement categories. Data integrity was ensured through consistent use of data elements and referential constraints.

On the application layer, a modular ABAP report was developed using **selection screens with radio buttons**, structured **INCLUDE programs**, and FORM routines to separate logic. The report dynamically retrieves and displays product and customer records using `SELECT`, `INNER JOIN`, and `MODIFY` statements. Advanced formatting techniques such as `POSITION`, `LEFT-JUSTIFIED`, `COLOR`, and structured headers were implemented to improve output readability. One module recalculates transactional values (quantity × price) and updates database records, demonstrating practical data manipulation and persistence handling.

The second project extends the solution into **Object-Oriented ABAP (ABAP Objects)** 
A local class (`LCL_PRODUCTS`) encapsulates product attributes with private members and public methods, including a constructor, setter/getter methods, and a class-level counter to track object instances. The architecture follows separation-of-concerns principles, with class logic isolated in an INCLUDE file and the main report managing object instantiation and output sequencing. Internal tables of object references simulate database-driven workflows while maintaining clean, maintainable code.

Across both projects, emphasis was placed on modularization, data encapsulation, referential integrity, formatted reporting, and scalable program structure. The work demonstrates practical SAP ERP development skills, including Data Dictionary configuration, relational database design, procedural and object-oriented ABAP programming, and structured output visualization within the SAP GUI environment.
