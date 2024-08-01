from pandasai import SmartDataframe
from pandasai.llm import OpenAI
from pandas as pd
data = {
    "restaurant": ["Mega", "Compose", "Angelinus", "PAIK'S", "Starbucks"],
    "sales": [100, 90, 30, 60, 140],
    "profit": [30, 15, 10, 200, 40],
}
df = pd.DataFrame(data)
print(df)

llm = OpenAI(api_token="<API_TOKEN>")

sdf = SmartDataframe(df, config={"llm": llm})

prompt = "<Ask question>"
sdf.chat(prompt)

