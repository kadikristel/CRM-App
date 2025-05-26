# CRM Application

A manual testing project for a Customer Relationship Management (CRM) system, focusing on API testing and user management functionalities.

## Project Overview

This project involves testing various aspects of a CRM application, including user invitations, stage management, and API integrations.

## Testing Artifacts

- Postman collections for API testing
- Test case documents
- Bug reports

## Technologies Used

- Manual testing methodologies
- Postman
- PDF documentation

## Getting Started

Import the provided Postman collections to explore and test the CRM APIs.


## API documentation ##

**Sprint 1**

   **Magicuser API**
   
      Get the list of all magicusers
      URL: GET {baseUrl}/obj/magicuser
      
      The API must return a list of all previously created magic users 
      with some optional search constraints. It must retrieve 100 
      items at most at once.
  ![magicusers_get_API_documentation](https://github.com/user-attachments/assets/2af8482a-f06d-408a-bffd-c81e8b915374)

      Create a new magicuser
      URL: POST {baseUrl}/obj/magicuser
      
      This API allows to invite a new user to use the system.
  ![magicusers_post_API_documentation](https://github.com/user-attachments/assets/6996f5fc-44dd-4c16-8564-b2c250e92ddd)

  **Leads API**
      
      Get lead data by unique Id
      URL: GET {baseUrl}/obj/lead/:UniqueID
      
      The API must return the data of a lead by its unique Id.
  ![leads_API_documentation](https://github.com/user-attachments/assets/2d4f152a-7eb5-473d-bfab-29235c83ebf8)
      
      Replace lead data  
      URL: PUT {baseUrl}/obj/lead/:UniqueID
      
      Replaces a lead with a new lead by unique ID.
  ![leads_put_API_documentation](https://github.com/user-attachments/assets/a011f982-8134-44ec-b00a-6d3a8bacafc3)

  **Funnels API**
    
      Create a new funnel
      URL: POST {baseUrl}/obj/funnel
      
      This API allows the creation of a new funnel.
  ![funnels_post_API_documentation](https://github.com/user-attachments/assets/5889b4c9-c67a-433a-b0b1-4d898feb299b)

      Delete funnel 
      URL: DELETE {baseUrl}/obj/funnel/:UniqueID
      
      Deletes a thing of type funnel by unique ID.
  ![funnels_delete_API_documentation](https://github.com/user-attachments/assets/1586cc55-6839-485d-bd2e-b9d1f7de4772)

  **Stages API**
    
    Stages are required to create funnels. The funnel must have at least 1 stage.
    
    Get the list of all stages
    URL: GET {baseUrl}/obj/stage
    
    The API must return a list of stages with some optional search constraints. 
    It must retrieve at least 100 items at once.
  ![stages_getAll_API_documentation](https://github.com/user-attachments/assets/9aad5c9f-4892-4c4b-a38e-88a3ba7e3539)

    Mofidy stage data
    URL: PATCH {baseUrl}/obj/stage/:UniqueID
    
    Modifies a stage by unique ID.
  ![stages_patch_API_documentation](https://github.com/user-attachments/assets/1aaba225-d9c2-4228-b432-626026a99b88)


**Sprint 2**

  **Deals**
  
    Create a new deal
    URL: POST {baseUrl}/obj/deal
    
    This API allows the creation of a new deal.
  ![deal_post_API_documentation1](https://github.com/user-attachments/assets/f6ba1f0a-ac1b-4067-a962-c3de4af87fcb)
  ![deal_post_API_documentation2](https://github.com/user-attachments/assets/dee1e391-ddf9-4e91-bf84-b665de01db11)

    Delete deal
    URL: DELETE {baseUrl}/obj/deal/:UniqueID
    
    Deletes a thing of type deal by unique ID.
  ![deal_delete_API_documentation](https://github.com/user-attachments/assets/a9790b2a-8eaf-4cee-83df-11fdbaa6e774)

  **Notes**

    Notes can be attached to the deals to store additional information and comments.
    
    Get the list of all notes
    URL: GET {baseUrl}/obj/note
    
    The API must return a list of notes with some optional search constraints. 
    It must retrieve at least 100 items at once.
  ![notes_getAll_API_documentation](https://github.com/user-attachments/assets/07c5accf-8155-4d4d-901e-259eb0a4a366)

    Mofidy note data 
    URL: PATCH {baseUrl}/obj/note/:UniqueID
    Modifies a note by unique ID.
  ![notes_patch_API_documentation](https://github.com/user-attachments/assets/331370f7-ca73-4119-8af4-af520523b820)

