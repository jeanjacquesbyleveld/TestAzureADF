Executive summary 

The Hyperspectral Cloud Data Ingestion project requires an Azure file structure that supports hyperspectral data from different projects and sites and complies with the existing Anglo-American governance and data policies and procedures while also removing the current dependency on local backup storage as the only location from which the data can be accessed.  

TerraCore confirmed that RAW represents L0, Extracted Image and RGB Extracted Image represented L1, and Feature Band Image represents L3. TerraCore also confirmed that changing the underlying source file structure would have significant implications and recommend that the existing complete file group structure remain. The project team assessed Azure blob storage containers to preserve or transform the TerraCore file structure downstream. 

During the investigation, it was discovered that L3 data (Feature Band Images) was also included in the local backup storage at the Sishen Demaneng. As such, provision has been made to cater for the data.  

The Anglo ACL team demonstrated a processing-level first blob storage pattern. This pattern aligns closely with Option 3 and supports blob storage for the projects needs.  

TerraCore has confirmed that historical data migration can be achieved by pushing the data to the Buffer Device and enabling projects sequentially. A concern the project team had was limited space on the Buffer Device itself. The historical data would take up 90% of the Buffer Device storage, leaving no space for transformation processes. As such, an approach to batch the migration data was discussed. TerraCore confirmed they cannot divide one project into configurable batches.  

Option 3 is currently the strongest candidate approach for the project team.  