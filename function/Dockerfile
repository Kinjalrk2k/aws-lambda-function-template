FROM public.ecr.aws/lambda/nodejs:14

COPY app.js package*.json ./
ADD aws ./aws

RUN npm install

CMD [ "app.handler" ]