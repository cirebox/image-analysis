# Project AWS Lambda Image Analysis

### Config Dashboad

```
sls
```

### Deployment

```
sls deploy
```

### Invocation

After successful deployment, you can invoke the deployed function by using the following command:

```bash
sls invoke -f img-analysis --path request.json --l 
```

Which should result in response similar to the following:

```json
{
    "statusCode": 200,
    "body": "A imagem tem\n  99.68% de ser do tipo Cachorro\n 99.68% de ser do tipo cão\n 99.68% de ser do tipo animal de estimação\n 99.68% de ser do tipo canino\n 99.68% de ser do tipo animal\n 99.68% de ser do tipo mamífero\n 94.25% de ser do tipo cão"
}
```

### Local development

You can invoke your function locally by using the following command:

```bash
sls invoke local -f img-analysis --path request.json --l 
```

Which should result in response similar to the following:

```
{
    "statusCode": 200,
    "body": "A imagem tem\n  99.68% de ser do tipo Cachorro\n 99.68% de ser do tipo cão\n 99.68% de ser do tipo animal de estimação\n 99.68% de ser do tipo canino\n 99.68% de ser do tipo animal\n 99.68% de ser do tipo mamífero\n 94.25% de ser do tipo cão"
}
```
