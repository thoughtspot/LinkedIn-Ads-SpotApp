
# LinkedIn Ads SpotApp

SpotApps are ThoughtSpot’s out-of-the-box solution templates built for specific use cases and data sources. They utilize ThoughtSpot Modeling Language (TML) Blocks, which are pre-built pieces of code that are easy to download and implement directly from the product.

The LinkedIn Ads SpotApp mimics the LinkedIn Ads data model. When deployed, it creates several Worksheets, Answers, and Liveboards based on your LinkedIn Ads data in your cloud data warehouse.

This is a sample Liveboard, created after you deploy the LinkedIn Ads SpotApp:
![LinkedIn Ads SpotApp Liveboard](https://github.com/thoughtspot/LinkedIn-Ads-SpotApp/assets/102629468/dd933ce6-bc3a-4832-a4bf-14c48e822825)

Use the LinkedIn Ads SpotApp to get invaluable insight into your LinkedIn Ads performance, from high-level usage to identifying popular campaigns.

## Prerequisites

Before you can deploy the LinkedIn Ads SpotApp, you must complete the following prerequisites:

- **Review Required Data**: Examine the required tables and columns for the SpotApp.
- **Ensure Column Compatibility**: Make sure that your columns match the required column type listed in the schema for your SpotApp.
- **Sync Data**: Synchronize all tables and columns from LinkedIn Ads to your cloud data warehouse. Though you can choose to sync only the required tables and columns, ThoughtSpot recommends syncing all tables and columns from LinkedIn Ads to ensure comprehensive data availability. This includes LinkedIn Ads’s out-of-the-box columns or any custom columns you are using.
- **Collaborate on Data Movement**: If you are using an ETL/ELT tool or working with another team within your organization, sync all columns from the tables listed in the SpotApp.
- **Obtain Credentials**: Acquire SYSADMIN privileges to connect to your cloud data warehouse. The cloud data warehouse must contain the data ThoughtSpot will use to create Answers, Liveboards, and Worksheets.
- **Unique Connection Name**: Each new SpotApp connection name must be unique.
- **Administrator Access to LinkedIn Ads**: Maintain administrator access to manage LinkedIn Ads.

Access the following LinkedIn Ads tables and Worksheets in your cloud data warehouse. Refer to the LinkedIn Ads SpotApp schema for more details:

- `AD_ANALYTICS_BY_CAMPAIGN`
- `CAMPAIGN_HISTORY`
- `CAMPAIGN_GROUP_HISTORY`

## Deploy the SpotApp

After you have downloaded the Zip file and verified its contents, follow these steps:

1. Log into your ThoughtSpot instance and create an Embrace connection to all of the relevant views.
2. Import the TML for the Worksheets and verify that it has all been imported without any errors.
3. Import the TML for the Liveboards and verify that it has all been imported without any errors.
4. You are ready to start searching your data!

For detailed instructions on how to import TML files, refer to the [ThoughtSpot documentation](https://docs.thoughtspot.com/software/latest/tml-import-export-multiple).


