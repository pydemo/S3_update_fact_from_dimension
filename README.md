# S3_update_fact_from_dimension
Updates large partitioned file from dimension file by one column join key.

```
C:\Users\alex_\mygit\dataworm>c:\tmp\Python\Python38-32\python.exe s3update.py
['campaign_00', 'video campaign "xvbcjfzlnhhtyxlzevjzyksnudzlciyzhqiofswxidsflfpfhldcqvytvluhxbgqrzutrmaefrbeobnqfgourqieoooahmqtttbs"', 'metadata 2']
{'campaign_00': ['campaign_00',
                 'video campaign '
                 '"xvbcjfzlnhhtyxlzevjzyksnudzlciyzhqiofswxidsflfpfhldcqvytvluhxbgqrzutrmaefrbeobnqfgourqieoooahmqtttbs"',
                 'metadata 2']}
tables/FACT_IMPRESSIONS/B_0/FACT_IMPRESSIONS.B_0.campaign_00.campaign.csv.gz
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_0', 'FACT_IMPRESSIONS_JOINED.B_0.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_0')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_1', 'FACT_IMPRESSIONS_JOINED.B_1.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_1')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_2', 'FACT_IMPRESSIONS_JOINED.B_2.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_2')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_3', 'FACT_IMPRESSIONS_JOINED.B_3.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_3')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_4', 'FACT_IMPRESSIONS_JOINED.B_4.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_4')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_5', 'FACT_IMPRESSIONS_JOINED.B_5.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_5')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_6', 'FACT_IMPRESSIONS_JOINED.B_6.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_6')
88888 ('tables/FACT_IMPRESSIONS_JOINED/B_7', 'FACT_IMPRESSIONS_JOINED.B_7.campaign_00.joined_fact_and_dim.csv.gz', 'campaign_00', 'B_7')
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
33333 tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
get_chunk 82 0
get_chunk 0 0
merging 82 0
s3update.py executed in 1.43 seconds.
```
