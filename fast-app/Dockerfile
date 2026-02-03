# hamari application ka run time sbse upper ata.. python say humnay yeh code kiya tw
# pyhton add krdi... 
FROM python:3.13-slim

WORKDIR /app

# ismain first wala dot root directory and second wala working directory
# ji iss image kay andr directory hogi.
COPY . .

# pip say uv install. pip python kay andr ata hai.
RUN pip install uv

# jo code copy hua root say workdir mai usmain py.toml kee file ko dekh kr
# sb dependendies install krday gee yeh command.
RUN uv sync

# jispay run hoga
EXPOSE 8000

CMD ["uv", "run", "fastapi", "dev", "main.py", "--host", "0.0.0.0"]

# host 0.0.0.0 yeh humny cmd mai isliye define kee qynke yeh hamaray system ka
# port hai hr devise ka yeh port hota hai means host machine ka... hum apnay system
# kay kis port pay apni application run krna chatay hain.