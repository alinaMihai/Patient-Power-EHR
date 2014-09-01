Patient-Power-EHR
=================

diploma project using Java EE

This project implements an Electronic Health Care Record System that allows the Patient to create Access Control
Lists on his medical electronic information. 

The chosen solution of privacy is a combination of the Discretionary Access Control that uses an Access Control List
and the Role-based Access Control. A healthcare provider can have access to the patient's medical information either 
based on a role assigned by the administrator or on user identity and authorization. 

The Patient Power EHR comprises 4 parts:
- the Server Application containing the business logic of the system and the database architecture
- the Patient Desktop Application which allows the Patient to view his EHR and manage ACLs
- the Admin Desktop Application for management of user accounts (Patients and Healthcare Providers)
- the Healthcare Provider Desktop Application offering functionality like Patient medical information management, 
based on the level of access, and of general care plans. 

The Server Application is hosted on an EJB complient Server like Glassfish, and uses two types of Enterprise beans: 
 - Stateless Session Beans: - use the Entity Manager to access and modify persistent data (CRUD); 
                            - are exposed through web services and accessed by the EJB application Clients
                            
 - Entity Beans: the persistent objects representing datastore records.
 
 On the Enterprise application Clients reside web service clients that communicate with the web services found on the server side.
 
 Technologies used:
 - Java EE 6: Enterprise JavaBeans (EJB), JAX-WS (Java API for XML web services), JPA (Java Persistence API)
 - Java SRE: Swing
 
 Working environment:
 - Netbeans IDE 7.2.1
 - EclipseLink
 - GlassFish

