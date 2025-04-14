If you're stuck on the error:

`Rule named 'NOT NULL' not found for the user_id column in the data quality task. Please re-create the task including this rule as mentioned in the instructions.` 

in the **Build a Data Mesh with Dataplex: Challenge Lab**

when faced with this issue, ensure in your yml config file you use the actual values instead of variables as placeholders.

    projects: $PROJECT_ID        # instead replace with your actual project ID as shown below
    projects: qwiklabs-gcp-04-df41a3beb0d6
  
    locations: $REGION           # instead replace with your actual specified region as shown below
    locations: us-central1
    
    # lakes: Sales Lake        # use the auto populated lake ID just in case using the actual name fails
    lakes: sales-lake
    
    zones: curated-customer-zone`      # use the curated zone and NOT the raw zone
