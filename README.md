# s3-deploy
Github Workflow for S3 deployment

## Usage

```
- name: Deploy
  uses: wirecard/s3-deploy@master
  with:
    AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
    AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    AWS_REGION: ${{ secrets.AWS_REGION }}
    AWS_S3_BUCKET: ${{ secrets.AWS_S3_BUCKET }}
    SRC_DIR: out/
    DST_DIR: public/
```

### Variables

| Name                    | Required | Default |
|-------------------------|----------|---------|
| `AWS_ACCESS_KEY_ID`     | true     |         |
| `AWS_SECRET_ACCESS_KEY` | true     |         |
| `AWS_REGION`            | true     |         |
| `AWS_S3_BUCKET`         | true     |         |
| `SRC_DIR`               | false    | `.`     |
| `DST_DIR`               | false    | `/`     |
