# Data
# Deploy prefect cloud

1. Install uvx
   > powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

2. Login to prefect cloud
   > uvx prefect-cloud login

3. Deploy python code from Github
   > uvx prefect-cloud deploy etl_pipeline.py:main_flow --name my_etl --from https://github.com/ChonlatitMax/Data --with-requirements requirements.txt

4. Run main_flow function
   > uvx prefect-cloud run main_flow/my_etl

5. Schedule tasks
   > uvx prefect-cloud schedule main_flow/my_etl "*/1 * * * *"

## Google Bigquery
[เพิ่มลิงก์หรือรายละเอียดของคุณที่นี่]
