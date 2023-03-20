# Developing frontend

## Build environment
```
docker build -t gyoza_front .
```

If you want to create react app first
```
docker run --rm --name gyoza_front_run -it -v $PWD:/app gyoza_front /bin/bash
cd app
npx create-react-app react-app
```

## Start development server
```
docker run --rm --name gyoza_front_run -it -p 3000:3000 -v $PWD/react-app:/react-app gyoza_front /bin/bash
cd react-app
yarn start
```
Access: http://localhost:3000