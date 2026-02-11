# hamari application ka run time sbse upper ata.. python say humnay yeh code kiya tw
# pyhton add krdi... slim means light image sirf python or kuch zarori cheezein
FROM python:3.13-slim

# docker kay andr app naam ki directory bnao jahan hamara sara codebase hoga
WORKDIR /app

# ismain first wala dot root directory and second wala working directory
# jo iss image kay andr directory hogi. sara codebase files sb /app main copy krdo.
COPY . .

# pip say uv install. pip python kay andr ata hai.
RUN pip install uv

# jo code copy hua root say workdir mai usmain py.toml kee file ko dekh kr
# sb dependendies install krday gee yeh command.
RUN uv sync

# jispay run hoga yeh srf documentation hai..
EXPOSE 8000


# fastapi dev main.py yeh fastapi ka dev server start krrhi hai same jesay uv run uvicorn
# main:app say hum uvicorn chalatay fastapi dev fastapi kay new modern version man aya hai
# ismain humein sirf fastapi dev or filename dena nahee reload dena hai yeh by default hota hai.
# or 8000 port bhee by default hota hai.
CMD ["uv", "run", "fastapi", "dev", "main.py", "--host", "0.0.0.0"]

# host 0.0.0.0 yeh humny cmd mai isliye define kee qynke yeh hamaray system ka
# port hai hr devise ka yeh port hota hai means host machine ka... hum apnay system
# kay kis port pay apni application run krna chatay hain.