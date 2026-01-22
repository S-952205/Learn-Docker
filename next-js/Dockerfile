# node kee image pull hogi docker-hub say node isliye qynke next app run
# npm say hoti and npm kayliye node chahiye.
FROM node:22-alpine


# workdir means hamara codebase docker main app directory mai hoga.
WORKDIR /app

# copy package and the rest of files jo start package say hotein and agay kuch bhee hai
# woo sb files copy krlo.
COPY  package*.json ./

# run means run hogi yeh command docker mai jissay dependendies install hongein.
RUN npm install

# copy means hamara sara codebase iss project ka copy kro.
COPY . .

# production main janay say pehlay yeh command run krtay.
RUN npm run build

# jis port pay chlaygee
EXPOSE 3000

# command production server run krnay kee
CMD [ "npm", "start" ]
