# Industrial-IoT-Root-Cause-Analysis-of-Industrial-Equipments

This is a simple GenAI application which will take the documentation of a motor and then
- Summarizes the specs from that documentation
- Identifies the anomalous data of the motor and
- Suggests troubleshooting actions.

This consists of two python files: one for the Streamlit front end, and one for the supporting library to make calls to AWS Bedrock.

## Requirements

- Python 3.12.x
- Ubunutu 24.x

## Commands

1. Install python dependecies

```pip3 install pip==24.0 && pip3 install -r setup/requirements.txt -U```

2. To configure Streamlit

```
mkdir -p /home/ubuntu/.streamlit
cat >/home/ubuntu/.streamlit/config.toml <<EOL
[server]
enableXsrfProtection = false
enableCORS = false
EOL
```

3. To run the app, type following command:

```streamlit run rca_app.py --server.port 8081```
