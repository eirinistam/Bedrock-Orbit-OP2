# Agents for Amazon Bedrock UI

The use case  will demonstrate is a chatbot, with which we can talk with the Orbit OP2 documents for 2024 and also we can add on a table more OP2 projects.

# Prequisites

- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- [Python 3](https://www.python.org/downloads/)

# Running Locally

1. Run the following `pip` command to install the dependencies:

   ```
   pip install -r requirements.txt
   ```

2. Set the following environment variables:
   - `BEDROCK_AGENT_ID` - The ID of the agent
   - `BEDROCK_AGENT_ALIAS_ID` - The ID of the agent alias. The default `TSTALIASID` will be used if it is not set.
   - The [AWS environment variables](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html) that provides the credentials to your account. The principal must have the necessary permissions to invoke the Bedrock agent.
3. (Optional) Set the folliowing environment variables to customize the UI:
   - `BEDROCK_AGENT_TEST_UI_TITLE` - The page title. The default `Agents for Amazon Bedrock Test UI` will used if it is not set.
   - `BEDROCK_AGENT_TEST_UI_ICON` - The favicon, such as `:bar_chart:`. The default Streamlit icon will be used if it is not set.
4. Run the following command to start the Streamlit app:

   ```
   streamlit run app.py --server.port=8080 --server.address=localhost
   ```
