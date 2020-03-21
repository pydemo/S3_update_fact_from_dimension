# S3_update_fact_from_dimension
Updates large partitioned file from dimension file by one column join key.
## Fact was
    50000,campaign_00,video_0,0.5,metadata 1
    50080,campaign_00,video_0,0.1,metadata 1

## Fact now
    50000,campaign_00,video_0,0.5,metadata 2
    50080,campaign_00,video_0,0.1,metadata 2

## Dimension
    campaign_00,video campaign "xvbcjfz",metadata 2
    campaign_01,video campaign "cjzfybq",metadata 2

## Exec log
```
['campaign_00', 'video campaign "xvbcjfzln"', 'metadata 2']
{'campaign_00': ['campaign_00',
                 'video campaign '
                 '"xvbcjfzln"',
                 'metadata 2']}
tables/FACT_IMPRESSIONS/B_0/FACT_IMPRESSIONS.B_0.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_0/FACT_IMPRESSIONS_APPENDED.B_0.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_1/FACT_IMPRESSIONS_APPENDED.B_1.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_2/FACT_IMPRESSIONS_APPENDED.B_2.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_3/FACT_IMPRESSIONS_APPENDED.B_3.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_4/FACT_IMPRESSIONS_APPENDED.B_4.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_5/FACT_IMPRESSIONS_APPENDED.B_5.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_6/FACT_IMPRESSIONS_APPENDED.B_6.campaign_00.campaign.csv.gz
Fact file: tables/FACT_IMPRESSIONS_APPENDED/B_7/FACT_IMPRESSIONS_APPENDED.B_7.campaign_00.campaign.csv.gz
Total uploaded, bytes: 83
Total uploaded, bytes: 78
Total uploaded, bytes: 83
Total uploaded, bytes: 81
Total uploaded, bytes: 75
Total uploaded, bytes: 76
Total uploaded, bytes: 92
Total uploaded, bytes: 67
s3update.py executed in 1.73 seconds.
```
