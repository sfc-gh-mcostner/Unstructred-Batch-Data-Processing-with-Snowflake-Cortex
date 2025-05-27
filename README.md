# Unstructured Batch Data Processing with Snowflake Cortex

Welcome to the Hands on Lab!

## What You'll Learn Today

Welcome to ArenaFlow Intelligence Hub!  Throughout this lab you'll see how easy it is to integrate Cortex AI into Snowflake's core data engineering features to batch process unstructured data.

We'll highlight several Snowflake features to throughout this lab:
- [Snowflake Cortex](https://docs.snowflake.com/en/user-guide/snowflake-cortex/llm-functions)
    - Task Specific Functions for analyzing sentiment and summarization
    - Cortex Complete to generate a prompt and response 
- [Snowflake Notebooks on Container Runtime](https://docs.snowflake.com/en/developer-guide/snowflake-ml/notebooks-on-spcs)
    - Execute the notebook on a GPU powered compute pool
    - Leverage a pre-built image containing hundreds of common Python packages
    - Create an external access integration to install additional 3rd party Python packages
- [Triggered tasks](https://docs.snowflake.com/en/user-guide/tasks-intro#triggered-tasks)
    - Process data based on specific data change events
- [Dynamic Tables](https://docs.snowflake.com/en/user-guide/dynamic-tables-intro)
    - Incrementally process changed data
- [Cortex Analyst](https://docs.snowflake.com/en/user-guide/snowflake-cortex/cortex-analyst)
    - Create a chat applications for a "talk to your data" experience
- [Streamlit in Snowflake](https://docs.snowflake.com/en/developer-guide/streamlit/about-streamlit)
    - Host your Cortex Analyst chat app directly within Snowsight

## Lab Setup

1. Execute the SQL script found in setup.sql
2. Upload the tweet_metrics.yaml file to an internal stage (`ARENAFLOW.AI_ML.SEMANTIC_MODELS` by default)
3. Create a new Streamlit in Snowflake app with `cortex_analyst_chat_app_script.py` as the main app file
4. Upload `ArenaFlow Snowflake Cortex Hands on Lab.ipynb` to Snowsight
- Choose "Run on Container" as the **Python Environment**
- Select "Snowflake ML Runtime GPU 1.0" as the **Runtime**
- Select "GPU_ARENAFLOW_M" as the **Compute Pool**
#### Note
Setup will require both `SYSADMIN` and `ACCOUNTADMIN` to create various objects and integrations

