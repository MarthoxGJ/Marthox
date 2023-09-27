# Marthox

## Description

Marthox is a web portfolio that showcases my projects and skills. The idea behind it is to have a simple and clean design that is easy to navigate and understand. So everyone interested in my work can easily find what they are looking for and contact me.

## How to run the project

### Development

To build and run the project for the first time, use the following command:

```bash
docker-compose -f docker-compose.dev.yml up --build
```

To build the project without running it, use the following command:

```bash
docker-compose -f docker-compose.dev.yml build
```

Once the project has been built, you can run it using the following command:

```bash
docker-compose -f docker-compose.dev.yml up
```

### Production

To build and run the project for the first time, use the following command:

```bash
docker-compose -f docker-compose.prod.yml up --build
```

To build the project without running it, use the following command:

```bash
docker-compose -f docker-compose.prod.yml build
```

Once the project has been built, you can run it using the following command:

```bash
docker-compose -f docker-compose.prod.yml up
```
